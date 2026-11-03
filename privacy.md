# 隐私政策 · Privacy Policy

[中文](#中文版) · [English](#english)

- **生效日期 / Effective:** 2026-11-01
- **适用产品 / Product:** 映库 Pictorium(iOS 26+)
- **联系 / Contact:** [GitHub Issues](https://github.com/Kn0688/pictorium-site/issues)

---

## 中文版

### 一句话

映库是一个**完全在设备端运行**的照片与文件知识库。你的照片、文件和搜索内容不会离开这台设备。

### 我们收集什么

**什么都不收集。**

- 没有账号系统,不需要登录,不收集姓名、邮箱、手机号等任何身份信息
- 没有第三方 SDK:无广告、无统计、无崩溃上报、无埋点
- 不做跨 App 追踪,不请求广告标识符(ATT 不适用)

### 你的数据在哪里

- 照片、截图、文件的索引(文字识别、语义向量、备注)全部在**本机**生成并保存在 App 的沙盒内
- 不上传、不云同步、不备份到我们的服务器
- 删除 App 即删除本机全部索引数据

### 网络请求

映库在正常使用中有**两种**出网行为,都与「地点」有关:

**1. 地点名称反编码。** 当你在「地点」中浏览尚未命名的位置簇时,App 会通过 iOS 系统的地理编码服务,把**精度约 500 米的簇锚点**发给 Apple 以换取可读地名。

**2. 地图瓦片。** 「地点」页顶部的地图由 Apple 地图服务渲染,会请求当前可见区域的地图图片。请求只包含地图区域,不包含你的照片、文件或搜索内容。

- 发送的是簇的近似中心点,**不是**照片的精确坐标
- 不发送照片、文件内容、搜索关键词或任何设备标识
- 反编码结果会缓存在本机,后续不再重复请求
- 若你不使用「地点」功能,App 不产生任何出网请求

此外:

- 1.0 版本**不包含**模型下载入口,不会下载任何模型文件
- 小组件、系统搜索(Spotlight)、索引、搜索全部在本机完成

### 权限用途

| 权限 | 用途 | 数据流向 |
|---|---|---|
| 相册(读) | 在本机为照片建立索引(文字识别 + 语义理解),支持搜索、截图归档、「历史上的今天」 | 仅本机;若选择「选中的照片」,只处理你选中的部分 |
| 文件(系统选择器) | 你主动添加的 PDF / Markdown / 文本,在本机建立全文索引 | 仅本机 |
| 面容 ID / 设备密码 | 仅用于解锁「加密分区」 | 由 iOS 校验,App 拿不到生物特征或密码 |

### 加密分区

- 移入加密分区的内容使用系统级文件加密,独立密码保存在 iOS Keychain
- 加密分区的内容不参与默认搜索,不出现在小组件与系统搜索中

### 数据删除

- 删除 App:设备上的索引与本机数据一并删除
- 整理页的删除建议需要你二次确认;照片进入系统「最近删除」,30 天内可恢复
- 文件书签可在「我的 → 文件」中逐个移除

### 儿童隐私

映库不收集任何个人信息,因此也不存在针对儿童的数据收集行为。App 分级为 4+。

### 政策变更

若隐私实践发生实质变化,我们会更新本页并修改顶部「生效日期」。重大变更会在 App 更新说明中提示。

### 联系我们

`YOUR_EMAIL@example.com` <!-- TODO: 换成真实邮箱 -->

---

## English

### In one sentence

Pictorium is a photo and file knowledge base that runs **entirely on your device**. Your photos, files and searches never leave this iPhone.

### What we collect

**Nothing.**

- No account, no sign-in, and no collection of names, email addresses, or phone numbers
- No third-party SDKs: no ads, no analytics, no crash reporting, no telemetry
- No cross-app tracking, and no advertising identifier is requested

### Where your data lives

- Indexes of photos, screenshots and files (text recognition, semantic vectors, notes) are created and stored **locally** inside the app's sandbox
- Nothing is uploaded, synced, or backed up to our servers
- Deleting the app deletes all of its local data

### Network requests

In normal use Pictorium makes **two kinds** of outbound request, both related to Places:

**1. Reverse geocoding of place names.** When you browse unnamed location clusters under Places, the app sends a **~500 m-precision cluster anchor** to Apple's system geocoding service to obtain a readable place name.

**2. Map tiles.** The map shown at the top of the Places screen is rendered by Apple Maps, which requests map imagery for the visible region. The request contains only the map region — never your photos, files, or searches.

- Only the approximate cluster center is sent — never a photo's precise coordinates
- No photos, file contents, search queries, or device identifiers are sent
- Results are cached locally, so the same cluster is not requested again
- If you never open Places, the app makes no outbound requests at all

In addition:

- Version 1.0 **has no model-download entry** and downloads no model files
- Widgets, Spotlight indexing, indexing and search all run on device

### Permissions

| Permission | Purpose | Data flow |
|---|---|---|
| Photo Library (read) | Build a local index (text recognition + semantic understanding) for search, screenshot organization, and On This Day | On device only; with "Selected Photos" only your selection is processed |
| Files (system picker) | Full-text index of PDF / Markdown / text you explicitly add | On device only |
| Face ID / Passcode | Unlock the Vault only | Verified by iOS; the app never sees biometrics or your passcode |

### The Vault

- Content moved into the Vault uses system-level file encryption; the separate password is stored in the iOS Keychain
- Vault content is excluded from default search and never appears in widgets or system search

### Deleting your data

- Deleting the app removes all local indexes and data
- Cleanup suggestions require your confirmation; deleted photos go to Recently Deleted and can be restored within 30 days
- File bookmarks can be removed individually under Me → Files

### Children's privacy

Pictorium collects no personal data, so there is no data collection from children. The app is rated 4+.

### Changes

If our practices change materially, we will update this page and the "Effective" date above. Significant changes will be noted in the app's release notes.

### Contact

`YOUR_EMAIL@example.com` <!-- TODO: 换成真实邮箱 -->
