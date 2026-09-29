# 网站数据快照 · YYYY-MM-DD

> 使用方式：复制本文件到同目录，重命名为日期（如 `2026-10-05.md`），然后照着 `../GUIDE.md` 填数字。
> 每周一次，15-20 分钟。**Clarity 只保留 30 天，不抄就会永久丢失。**

- 采集时间：
- 采集人：
- 代理状态：GSC/GA4 已开 Clash ｜ Clarity 已关 Clash

---

## 一、Google Search Console — 自然搜索表现

> 报告：`Performance` → `Search results` ｜ 时间范围：`Last 28 days`

| 指标 | 报告位置 | 本期 | 上期 | 变化 | 备注 |
|---|---|---|---|---|---|
| Total clicks | Performance 顶部 | | | | |
| Total impressions | Performance 顶部 | | | | |
| Average CTR | Performance 顶部 | | | | |
| Average position | Performance 顶部 | | | | |

**Top 5 搜索词**（`Performance` → `Queries` 标签）

| # | 查询词 | 点击 | 曝光 | CTR | 平均排名 | 品牌词？ |
|---|---|---|---|---|---|---|
| 1 | | | | | | |
| 2 | | | | | | |
| 3 | | | | | | |
| 4 | | | | | | |
| 5 | | | | | | |

> **判读重点：非品牌词的曝光有没有增长？** 只有非品牌词起量，才说明 SEO 真的在起作用。

**Top 5 落地页**（`Performance` → `Pages` 标签）

| # | 页面 | 点击 | 曝光 | 平均排名 |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |
| 5 | | | | |

**Top 5 国家**（`Performance` → `Countries` 标签）

| # | 国家 | 点击 | 曝光 |
|---|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |
| 4 | | | |
| 5 | | | |

> **判读重点：是否命中目标市场（非洲 / 印度 / 东南亚 / 南美）？**

**收录与站点地图**

| 指标 | 报告位置 | 本期 | 上期 | 备注 |
|---|---|---|---|---|
| 已编入索引页数 | `Indexing` → `Pages` | | | 站点约 20 页 |
| 未编入索引页数 | `Indexing` → `Pages` | | | |
| 主要原因 1（数量） | `Indexing` → `Pages` → 展开 | | | 如 `Discovered – currently not indexed` |
| 主要原因 2（数量） | 同上 | | | |
| Sitemap 状态 | `Indexing` → `Sitemaps` | | | 应为 Success、无 error |
| Sitemap 发现 URL 数 | `Indexing` → `Sitemaps` | | | 应接近站点页数 |

---

## 二、Google Analytics 4 — 流量来源与地域

> 报告：`Reports` ｜ 时间范围：`Last 28 days`

**总量**

| 指标 | 报告位置 | 本期 | 上期 | 备注 |
|---|---|---|---|---|
| Sessions | Acquisition 概览 | | | |
| Users | Acquisition 概览 | | | |
| Avg engagement time | Acquisition 概览 | | | |

**渠道构成**（`Acquisition` → `Traffic acquisition`）

| 渠道 | 会话数 | 占比 | 上期会话 | 备注 |
|---|---|---|---|---|
| Organic Search | | | | 目标 > 40% |
| Direct | | | | 偏高要警惕自测流量 |
| Referral | | | | 看是哪些站引荐 |
| Organic Social | | | | 对应 FB / LinkedIn / IG |
| Unassigned / 其他 | | | | |

**国家分布**（`User attributes` → `Demographics` → `Geography`，按 Users 排 Top 5）

| # | 国家 | Users | 会话 | 是否目标市场 |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |
| 5 | | | | |

> ⚠️ 若 China / United States 异常高，排查是否自测流量或爬虫。

**落地页**（`Engagement` → `Landing page`，Top 5）

| # | 落地页 | 会话 | 平均互动时长 |
|---|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |
| 4 | | | |
| 5 | | | |

**事件漏斗**（`Engagement` → `Events`）

| 事件 | 事件计数 | 上期 | 备注 |
|---|---|---|---|
| `product_card_click` | | | 产品列表被点 |
| `view_product` | | | 进产品详情页 |
| `form_start` | | | 开始填表单 |
| `form_submit` | | | 提交表单 |
| `inquiry_submitted` | | | **询盘成功（最关键）** |
| `whatsapp_click` | | | 含 link_location 分布 |
| `template_copy` | | | 复制邮件模板 |
| `click`（outbound，Enhanced Measurement 自带） | | | 外链点击，含 wa.me |

**关键事件**（`Engagement` → `Conversions`）

| 关键事件 | 次数 | 上期 |
|---|---|---|
| `inquiry_submitted` | | |
| `form_submit` | | |
| `whatsapp_click` | | |

---

## 三、Microsoft Clarity — 用户行为

> 时间范围：`Last 7 days` / `Last 30 days` ｜ **30 天滚动，务必每周抄**

| 指标 | 报告位置 | 本期 | 上期 | 备注 |
|---|---|---|---|---|
| Sessions | Dashboard | | | |
| Unique users | Dashboard | | | |
| Avg. session duration | Dashboard | | | |
| Bounce rate | Dashboard | | | B2B 50-70% 正常 |
| Scroll depth | Dashboard | | | < 50% 需前置卖点 |
| Rage clicks | Dashboard | | | 有聚集就要查 |
| Dead clicks | Dashboard | | | |
| Quick backs | Dashboard | | | > 10-15% 需查 |
| JavaScript errors | Dashboard | | | > 0 必查 |

**Top 页面**（`Dashboard` → `Insights` / `Top pages`）

| # | 页面 | Sessions | 备注 |
|---|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |
| 4 | | | |
| 5 | | | |

**自定义事件**（`Dashboard` → `Custom events`）

| 事件 | 计数 | 备注 |
|---|---|---|
| `whatsapp_click` | | |
| `product_card_click` | | |
| `form_submit` | | |
| `inquiry_submitted` | | |

**录屏抽看记录**（`Recordings`，每个 Top 页抽看 3-5 条）

| 页面 | 看了几条 | 发现的问题 |
|---|---|---|
| | | |
| | | |

**热力图观察**（`Heatmaps`）

- 「Get Quote」按钮是否被注意到：
- 产品列表卡片点击分布：
- 其他：

---

## 四、本周观察与动作

> **这两行才是最值钱的**，其他都是原始素材。

**一个发现**（本周数据里最值得注意的一件事）：


**一个动作**（下周要改的一个具体东西）：


---

## 五、待确认的异常

| 异常现象 | 可能原因 | 是否需要处理 |
|---|---|---|
| | | |
| | | |
