# 数据自动抓取的授权配置（一次性，约 20 分钟）

配完之后，GA4 / GSC / Clarity 的数据由脚本自动读取，每周一晚自动出一份解读周报——**不需要再手动截图**。

> 本文件只有操作步骤，不含任何密码。真正的凭据存在**仓库外**的
> `C:\Users\Administrator\.workbuddy\secrets\ding-yong\`，因为本仓库是公开的。

## 你要产出的东西（一共两个文件 + 一个数字）

| 产出物 | 放在哪 | 怎么来 |
|---|---|---|
| `service-account.json` | 上面那个 secrets 目录 | 从 Google Cloud 下载 |
| `clarity-token.txt` | 上面那个 secrets 目录 | 从 Clarity 后台复制 |
| `ga4_property_id` | 上面那个 secrets 目录的 `config.json` 里 | 从 GA4 后台抄一个纯数字 |

全程**不需要绑银行卡**，这两个 Google API 都是免费的。

---

## 第 1 部分：Google 服务账号

### 1.1 进入控制台

1. 先开 Clash（系统代理模式）——`console.cloud.google.com` 国内直连打不开
2. 浏览器右上角头像确认登录的是**平时看 GA4 / GSC 的同一个 Google 账号**（账号错了后面加权限全白做）
3. 打开 https://console.cloud.google.com
4. 首次进入会弹服务条款：Country 选 `China` → 勾选同意 → `AGREE`
   - 万一没选 China 也没关系，这个选项只影响适用哪一版服务条款，不影响任何功能，**不用回头改**

### 1.2 新建项目

1. 页面左上角 `Google Cloud` 标志右边有个下拉框（`Select a project` / 中文：`选择项目`）→ 点它
2. 弹窗右上角点 **`NEW PROJECT`** / 中文：**`新建项目`**
3. Project name / 项目名称填 `ding-yong-analytics`
4. Organization / 组织保持 `No organization` / `无组织` **不动**
5. 点 **`CREATE`** / `创建` → 等约 10 秒，右上角铃铛出现「项目创建成功」通知
6. **点通知里的 `SELECT PROJECT` / `选择项目`** —— 不点会停留在无项目状态，后面 API 就建错项目了
7. 自检：顶栏下拉框现在应显示 `ding-yong-analytics`，**后面每一步操作前都瞄一眼它**

### 1.3 启用两个 API

左上角 ☰ 汉堡菜单 → `APIs & Services` / 中文：`API 和服务` → `Library` / 中文：`库`，分别搜索并点 `ENABLE` / `启用`：

- **Google Analytics Data API**
- **Search Console API**

### 1.4 建服务账号并下载密钥

1. `APIs & Services` / `API 和服务` → `Credentials` / `凭据` → `+ CREATE CREDENTIALS` / `+ 创建凭据` → `Service account` / `服务账号`
2. 名字填 `analytics-reader` → `CREATE AND CONTINUE` / `创建并继续`
3. 角色**直接跳过**（点 `CONTINUE` → `DONE`）
4. 在服务账号列表里点进刚建的这个 → 上方 `KEYS` / `密钥` 标签 → `ADD KEY` / `添加密钥` → `Create new key` / `创建新密钥` → 选 **JSON** → `CREATE`
5. 浏览器会自动下载一个 json 文件 —— ⚠️ **Google 只允许下载这一次**，丢了就得删掉重建
6. 把下载的 json 改名成 `service-account.json`，放进 `C:\Users\Administrator\.workbuddy\secrets\ding-yong\`
7. 用记事本打开这个 json，找到 `client_email` 字段，值形如
   `analytics-reader@你的项目名.iam.gserviceaccount.com` —— **下一步要用**

### 1.5 把这个邮箱加进两个后台

- **GA4**：https://analytics.google.com → 左下角齿轮 `Admin` → 顶部确认选对 **Property**（关键，选错就白加）→ **Property 列**里点 `Property access management` → 右上角蓝色 `+` → `Add users` → 粘贴上面的邮箱 → **取消勾选** `Notify new users by email` → 角色选 **`Viewer`** → `Add`
- **GSC**：https://search.google.com/search-console → 选中属性 `ding-yong.com` → 左侧 `Settings` → `Users and permissions` → `Add user` → 同一个邮箱 → 权限选 **`Restricted`** → `Add`

### 1.6 抄 GA4 Property ID

GA4 `Admin` → **Property 列** → `Property settings` → 右上角 `PROPERTY ID`，是一个**纯数字**。

把它填进 `C:\Users\Administrator\.workbuddy\secrets\ding-yong\config.json` 的 `ga4_property_id`。

> ⚠️ **这个不是 `G-ZF0WEH06MP`**。`G-` 开头那个是测量 ID（往 GA4 送数据用的），
> 纯数字那个才是资源 ID（从 GA4 读数据用的），两者不能互换。

### 这一段最常见的三个坑

| 坑 | 后果 | 避法 |
|---|---|---|
| 在错误项目里启用了 API / 建了密钥 | 凭据连不上，预检报错 | 每次操作前瞄顶栏下拉框是否显示 `ding-yong-analytics` |
| 同意条款时用的不是 GA4/GSC 那个账号 | 加权限时邮箱对不上 | 进控制台前先看右上角头像 |
| 以为要绑银行卡，卡住不敢点 | 白白中断 | 这两个 API **完全免费**，遇到 Billing / 结算提示直接跳过 |

---

## 第 2 部分：Clarity token

1. 打开 https://clarity.microsoft.com ，选项目 `ykn7d1093k`
2. 左侧 `Settings` → `Data Export` → `Generate new API token`
3. 起个名字（4-32 字符，只能用字母数字和 `-` `_` `.`，不能有空格）
4. 复制生成的 token，粘贴进 `C:\Users\Administrator\.workbuddy\secrets\ding-yong\clarity-token.txt`
   （一行，前后不要有空格）

> 注意：Clarity 官方 API **只能取最近 1-3 天**的数据，取不到上周某一天。
> 所以本项目配了「每天 21:00 自动抓一次、累积成本地历史」的任务。

---

## 第 3 部分：验证

填完之后跑一次预检：

```
cd F:\code\Albert-XR\Supply
scripts\analytics\run_preflight.bat
```

它会依次检查：配置文件是否填全、两个凭据是否存在、Clash 代理端口是否通、Clarity 能否直连。

**全绿 = 授权通了。** 之后：

- 每周一 20:00 自动生成周报（结果在 `_analytics/snapshots/`，只有本地有，不进 Git）
- 每天 21:00 自动累积 Clarity 行为数据
- 读数据的通用方法见 [`GUIDE.md`](GUIDE.md)
