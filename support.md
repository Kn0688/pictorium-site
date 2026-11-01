# 支持 · Support

**映库 Pictorium** · iOS 26 及以上
**联系 / Contact:** [GitHub Issues](https://github.com/Kn0688/pictorium-site/issues)
通常在 2 个工作日内回复。反馈 bug 时请附上:机型号、iOS 版本、复现步骤。

---

## 中文

### 首次索引为什么这么久?

所有照片都要在本机做文字识别和语义向量计算,大约 **每张 1 秒**。一万张照片的首次索引可能需要数小时。

- 期间**可以退出 App**,索引会暂停,下次打开自动从断点继续
- 建议:首次使用时接上电源、连 Wi-Fi、放在一边

### 搜索不到照片怎么办?

1. 确认首页顶部显示「已索引 x/y」且 x 接近 y
2. 换个说法再试:语义搜索理解**意思**,不必和照片里的文字完全一致
3. 中文语义搜索依赖随包的中英文模型,通常开箱可用
4. 仍然搜不到 → 邮件反馈,附上你搜的词和照片的大致内容

### 只授权了「选中的照片」怎么办?

在「设置 → 映库 → 照片」里改为「完全访问」,或重新在 App 内授权。只授权部分照片时,索引与搜索仅覆盖你选中的那些。

### 我的人脸 / 密码安全吗?

加密分区使用系统级文件加密,密码保存在 iOS Keychain,App 从不接触你的生物特征。**忘记密码无法找回**,请务必记住。

### 删除照片会影响相册吗?

整理页只给建议,删除必须你二次确认,且照片会先进系统「最近删除」,30 天内可恢复。

### App 需要联网吗?

几乎不需要。唯一出网行为是「地点」页把**约 500 米精度的锚点**发给系统地理编码服务换取地名。搜索、索引、问答全部离线。

### 怎么彻底删除我的数据?

删除 App 即可,本机索引会一并删除。我们没有任何服务器副本。

---

## English

### Why does the first index take so long?

Every photo is processed on device (text recognition + semantic embeddings) at roughly **one second per photo**. 10,000 photos can take hours.

- You can leave the app; indexing pauses and resumes where it stopped next time
- Tip: plug in, use Wi-Fi, and let it run

### A photo I expect doesn't show up

1. Check the header shows "Indexed x/y" and that x is close to y
2. Try a different phrasing — semantic search matches *meaning*, not exact text
3. If it still fails, email us with the query and a rough description of the photo

### I only granted "Selected Photos"

Change it in Settings → Pictorium → Photos → "Full Access". With partial access, indexing and search cover only the selected photos.

### Is my passcode safe?

The Vault uses system-level file encryption and the password lives in the iOS Keychain. The app never sees your biometrics. **A forgotten Vault password cannot be recovered.**

### Do deleted photos disappear from my library?

Organize only suggests; deletion requires your confirmation and photos go to Recently Deleted first (30-day recovery).

### Does the app need the internet?

Barely. The only outbound request is the ~500 m place-name anchor on the Places screen. Search, indexing and Q&A are fully offline.

### How do I delete all my data?

Delete the app. Local indexes are removed with it. We keep no server-side copy.

---

## 反馈模板 / Bug report template

```
机型 / Device:
iOS 版本 / iOS version:
App 版本 / App version:1.0.0 (1)
问题描述 / What happened:
复现步骤 / Steps:
截图或录屏 / Screenshot or recording:
```
