# ding-yong.com 访问数据分析操作清单

> 这份文档解决一个问题：**打开三个后台，照着点，看懂数字，知道下一步该改什么。**
>
> 三个后台各有分工，缺一不可：
> **GSC** 答「有没有人搜到我」→ **GA4** 答「谁来了、从哪来」→ **Clarity** 答「来了之后干了什么」。

---

## 第 0 步：开始前先设置代理（最容易卡住的地方）

Google 的两个后台需要走代理，微软的 Clarity 反过来必须关代理。**顺序错了就打不开或看到旧缓存。**

| 顺序 | 后台 | 网址 | 账号 / 属性 | Clash |
|---|---|---|---|---|
| 1 | Google Search Console | https://search.google.com/search-console | 属性 `ding-yong.com` | **必须开启** |
| 2 | Google Analytics 4 | https://analytics.google.com | 数据流 `G-ZF0WEH06MP` | **必须开启** |
| 3 | Microsoft Clarity | https://clarity.microsoft.com | 项目 `ykn7d1093k` | **必须关闭** |

**推荐操作节奏（避免来回切代理切错）：**

```
开 Clash  → 看 GSC（5 分钟）→ 看 GA4（6 分钟）
关 Clash  → 看 Clarity（5 分钟）
```

总计约 15-20 分钟。整套流程每周做一次，同时把数字抄进 `snapshots/` 快照。

---

## 第 1 步：Google Search Console —「有没有人搜到我」

**打开报告：左侧 `Performance` → 选 `Search results`，右上时间范围选 `Last 28 days`。**

站上线才三周多，这个报告是**目前最有价值的数据源**——因为它是唯一能告诉你「Google 有没有开始给你流量」的地方。

### 要看的数字

| 指标 | 在页面哪里 | 怎么读 |
|---|---|---|
| **Total impressions**（曝光） | 顶部四个数字块 | 环比上升 = 收录和排名在改善。**若 28 天曝光长期 < 100，等于基本没被搜到**，问题在收录或关键词，不在页面设计 |
| **Total clicks**（点击） | 顶部 | 曝光涨了点击没涨 → 排名上不去或标题不吸引 |
| **Average CTR** | 顶部 | **必须结合排名一起看**：<br>· 平均排名进首页（<10）但 CTR < 1-2% → 标题/描述写得不行<br>· B2B 行业长尾词 CTR 3-5% 属正常 |
| **Average position** | 顶部 | < 10 = 首页；**11-20 = 第二页，这是最值得优化的区间**（改标题、加内容就能进首页）；> 20 = 实际等于没排名，此时看 CTR 没有意义 |

### 关键动作：点开 `Queries` 标签

这是整个 GSC 最有用的一个表。**必须区分两类词：**

- **品牌词**（dingyong、ding-yong、ding-yong.com）——有人搜说明品牌开始被记住，但这是你自己带来的流量
- **非品牌词**（例如 `410 stainless steel cutlery manufacturer`、`wholesale flatware supplier`）——**只有非品牌词的曝光在增长，才说明 SEO 真的起量了**

> 排查思路：如果曝光全来自品牌词，说明 Google 还没认可你的产品页。回去看 `Indexing → Pages`。

### 另外两个必看的地方

**`Indexing` → `Pages`**（收录状况）

| 状态 | 含义 | 怎么办 |
|---|---|---|
| Indexed（已编入索引） | 正常 | 站点约 20 个页面（15 个产品页 + 5 个主页面），收录数应逐步接近这个数 |
| `Discovered – currently not indexed` | Google 知道有这页但还没抓 | 页数多属正常；**持续偏多**说明内容偏薄或站点权重不够 |
| `Crawled – currently not indexed` | 抓了但判断不值得收录 | 需要补内容或内链 |
| `Duplicate without user-selected canonical` | 重复内容 | 需要加 canonical |

**`Indexing` → `Sitemaps`**（站点地图）

确认 `sitemap.xml` 状态是 `Success`，没有 error，`Discovered URLs` 数量跟站点页数接近。这是 Google 的入口，出问题会导致全站不被收录。

---

## 第 2 步：Google Analytics 4 —「谁来了、从哪来」

**打开 `Reports`，右上时间范围选 `Last 28 days`。**

### 报告一：`Acquisition` → `Traffic acquisition`（流量来源）

看渠道构成，B2B 外贸站的健康结构：

| 渠道 | 含义 | 健康标准 |
|---|---|---|
| **Organic Search** | 自然搜索来的 | **最终目标 > 40%**。现在上线 3 周，很低是正常的；但**连续 4 周没增长**就要回 GSC 查收录 |
| **Direct** | 直接输入网址 / 邮件点击 / 无法归因 | 偏高要警惕——可能是你自己测试、或老客户直接访问，不代表新客获取能力 |
| **Referral** | 其他网站引荐 | 反映外链和 B2B 平台的效果，值得看是哪些站 |
| **Organic Social** | 社媒来的 | 对应你的 Facebook / LinkedIn / Instagram 矩阵 |

### 报告二：`User attributes` → `Demographics` / `Geography`（地域）

**这是验证目标市场是否打对的关键。**

你要看到的是：**非洲、印度、东南亚（菲律宾、印尼优先）、南美**。

> ⚠️ 警惕信号：如果 **China / United States 占比异常高**，先排查是不是自己的测试流量、机房 IP 或爬虫，不要当成真实客户。必要时在 `Admin → Data settings → Data filters` 加一条排除 localhost 的过滤器。

### 报告三：`Engagement` → `Pages and screens`（页面表现）

重点看 **`Average engagement time`**（平均互动时长）：

| 数值 | 判读 |
|---|---|
| 产品页 > 60 秒 | 良好，内容有吸引力 |
| 产品页 30-60 秒 | 尚可 |
| 产品页 < 15 秒 | **有问题**——首屏没抓住人，或者落地页与搜索意图不匹配 |

配套看 `Landing page`（落地页）：哪些页面是访客的第一站，决定了第一印象。

### 报告四：`Engagement` → `Events`（事件漏斗）— 这是新埋点上线后才能用的

埋点上线后（本仓库已补），这里能看到完整漏斗。**逐级递减是正常的，关键是看掉在哪一级：**

```
product_card_click   产品列表被点
    ↓
view_product         进入产品详情页       ← 掉太多 = 卡片不吸引
    ↓
form_start           开始填联系表单       ← 掉太多 = 页面没有说服力
    ↓
form_submit          提交表单             ← 掉太多 = 表单太长/字段太多
    ↓
inquiry_submitted    询盘真正成功
```

**事件字典**（详情见本文档最后一节）：

| 事件 | 含义 |
|---|---|
| `view_product` | 有人打开了产品详情页 |
| `product_card_click` | 有人在产品列表点了卡片（参数含产品名、分类、点的是哪块） |
| `whatsapp_click` | 有人点了 WhatsApp（参数 `link_location` 区分是浮动按钮/联系页/页脚/感谢页） |
| `form_start` | 有人开始填联系表单 |
| `form_submit` | 提交了表单 |
| `template_copy` | 复制了邮件模板 |
| `inquiry_submitted` | **询盘成功**（参数含国家、数量、来源产品） |

> 📌 **有个现成的替代信号**：GA4 的 Enhanced Measurement 默认已经在记录**外链点击**（事件名叫 `click`，带 `outbound: true`）。WhatsApp 链接（wa.me）属于外链，所以**在你看到上面这些自定义事件之前，这里已经有一部分 WhatsApp 点击数据可查了**。可以先看这个。

---

## 第 3 步：Microsoft Clarity —「来了之后干了什么」

**记得先关 Clash。**

Clarity 不看流量大小，看**行为质量**：访客是不是在看、卡在哪、哪里让人误点。

### 要看的数字

| 指标 | 位置 | 怎么读 |
|---|---|---|
| **Scroll depth**（滚动深度） | Dashboard | 产品页平均 **< 50%** → 首屏不够吸引，或页面太长。**对策：把核心卖点、规格表前置** |
| **Rage clicks**（愤怒点击） | Dashboard | 同一个地方被反复快速点击 → 有东西看起来能点但其实没反应（例如产品卡图片、筛选按钮） |
| **Dead clicks**（无效点击） | Dashboard | 偏高 → 交互误导，需要加可点反馈或视觉区分 |
| **Quick backs**（快速返回） | Dashboard | **> 10-15%** → 落地页与搜索/广告的预期不匹配（标题党，或跳到了不相关的页面） |
| **JavaScript errors** | Dashboard | **出现就必须查**——可能连带影响表单提交和埋点，会让数据凭空变少 |
| **Bounce rate** | Dashboard | B2B 站 50-70% 属正常，**不要套用 C 端电商的标准** |
| **Sessions / Unique users** | Dashboard | 跟 GA4 大致对得上即可，不必纠结小数差异（两者算法不同） |

### 最有价值的用法：看录屏

点 `Recordings`，筛出 **Top 落地页**，每个页面**抽看 3-5 条录屏**。这是唯一能让你「亲眼看客户怎么用你网站」的地方。

看的时候问自己三个问题：
1. 他第一眼看的是什么？是不是你最想让他看的？
2. 他在哪里停下来了、滚回上去了？
3. 他有没有找联系方式？找了多久才找到？

**`Heatmaps`（热力图）**：重点看「Get Quote」按钮和价格区域（现在没有价格，显示 `Contact Us`）有没有被注意到。

---

## 第 4 步：早期数据怎么读（重要，避免误判）

你现在站点才上线 3 周多，**数据量很小，比率类指标的噪声极大**。

- **会话数 < 100/周时，所有百分比都会剧烈波动**。这周 50%、下周 20% 可能只是 2 个人和 1 个人的区别
- **优先看绝对数和趋势方向，不要看比率**
- **不要因为一周数据就下结论改版**。GSC 的排名和收录要 **2-8 周**才稳定
- 广告拦截器会挡住 GA4 和 Clarity，导致数据偏低——这是行业常态，不要把「数据少」直接解读成「没人来」

**什么时候可以开始看比率：** 周会话数稳定超过 100 之后。

---

## 第 5 步：把数字抄进快照（每周必做）

### 为什么必须手抄

**Microsoft Clarity 免费版的数据只保留约 30 天**，滚删后**永久丢失**。你 9/19 起的行为数据，大约 **10/19 就会消失**。

GA4 保留 14 个月，GSC 保留 16 个月，但**只有抄成表格，三者才能放在同一个时间轴上对比**。

### 怎么做

1. 复制 `snapshots/TEMPLATE.md`
2. 重命名为当天的日期，例如 `snapshots/2026-10-05.md`
3. 照着本文档前四步，把数字填进表格
4. 填完「本周观察与动作」那两行——**这两行才是最值钱的**，其他都是原始素材

**频率**：每周一上午，15-20 分钟。

**额外触发**：每次大批量上新产品或发外链后，**48 小时内补一次 GSC 快照**，能看出收录有没有反应。

---

## 第 6 步：上线后必须做的一次性配置（开 Clash）

埋点已经改进代码，但**GA4 后台不注册参数的话，标准报告里看不到这些参数**（只能在 DebugView / Realtime 看到）。

### 1. 注册自定义维度

`Admin` → `Custom definitions` → `Create custom dimension`，**作用域（Scope）全部选 `Event`**，逐个添加：

| 维度名称 | 事件参数 |
|---|---|
| Product name | `product_name` |
| Product category | `product_category` |
| Product series | `product_series` |
| Click target | `click_target` |
| Link location | `link_location` |
| Form name | `form_name` |
| Inquiry country | `inquiry_country` |
| Inquiry quantity | `inquiry_quantity` |
| Product context | `product_context` |

### 2. 标记关键事件

`Admin` → `Events` → 找到下面三个事件 → 打开 `Mark as key event`：

- `inquiry_submitted`（最重要）
- `form_submit`
- `whatsapp_click`

### 3. 建议加一条数据过滤器

`Admin` → `Data settings` → `Data filters` → 排除 `localhost`，避免你自己的本地测试流量污染数据。

---

## 附录：埋点事件完整字典

| 事件名 | 触发时机 | 参数 |
|---|---|---|
| `view_product` | 打开产品详情页 | `product_name`、`product_category`、`product_series` |
| `product_card_click` | 点击产品列表卡片 | `product_name`、`product_category`、`click_target`（`quote` / `view_details` / `image_or_title`） |
| `whatsapp_click` | 点击任意 WhatsApp 链接 | `link_location`（`float_button` / `contact_page_button` / `footer_icon` / `thank_you_button` / `inline_link`）、`page_path` |
| `form_start` | 联系表单首次输入 | `form_name` |
| `form_submit` | 提交联系表单 | `form_name` |
| `template_copy` | 复制邮件模板成功 | `page_path` |
| `inquiry_submitted` | 到达 `/thank-you/` 页 | `inquiry_country`、`inquiry_quantity`、`product_context`、`inquiry_referrer` |

**技术说明（供以后维护参考）**

- 埋点实现在 `_includes/analytics-events.html`，通过 `document` 捕获阶段做**事件委托**，一处覆盖全站，**不要在具体 include 里再加内联 `onclick`，会重复计数**
- 数据同时发往 GA4（`gtag`）和 Clarity（`clarity('event', ...)`），Clarity 只同步 4 个业务事件，避免事件刷屏
- 会引发页面跳转的事件都带 `transport_type: 'beacon'`，保证跳转前数据发出
- 询盘的国家/数量通过 `sessionStorage` 的 `dy_inquiry_ctx` 从联系页传到感谢页（Web3Forms 是整页 POST 跳转，URL 带不过去）
- Clarity 的自定义事件在后台有**数分钟到数小时**的处理延迟，刚部署完看不到不是失败
