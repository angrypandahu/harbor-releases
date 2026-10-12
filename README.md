<p align="center">
  <img src="assets/icon.png" alt="影记图标" width="96" />
</p>
<h1 align="center">影记 · Yingji</h1>
<p align="center"><strong>你的收藏夹，还在吃灰吗？</strong></p>
<p align="center">抖音 · B 站 · 小红书收藏，一键带回家，变成能搜、能看、能用的笔记。</p>
<p align="center">
  <a href="https://github.com/angrypandahu/yingji-releases/releases/latest">👉 免费下载最新版</a> ·
  <a href="#三步上手">三步上手</a> ·
  <a href="https://github.com/angrypandahu/yingji-releases/releases">更新记录</a> ·
  <a href="https://github.com/angrypandahu/yingji-releases/issues">反馈问题</a>
</p>

---

刷到干货，先点个收藏，“回头再看”。

然后呢？收藏夹越攒越多，真想找的时候翻半天找不到；视频下架了，内容直接没了；三个平台各收各的，根本串不起来。

**收藏了 ≠ 学会了。** 影记就是来解决这件事的。

> 收藏 → 下载到本地 → 自动转文字 → AI 帮你整理成笔记

![影记媒体库：查看媒体、下载状态与关联内容](assets/media.png)

*截图来自真实界面，使用演示账号和示例内容，不含个人收藏。*

## 它能帮你做什么？

### ✅ 三个平台的收藏夹，一个地方全看完

连上你的抖音、小红书、B 站账号，收藏夹原样搬过来。按收藏夹翻，按标题搜，按“下没下载、转没转写、整没整理”一键筛选。想刷新就刷新，全部由你说了算。

![收藏夹：按来源账号和收藏分类浏览作品](assets/collections.png)

### ✅ 下载到自己电脑，再也不怕视频没了

喜欢的内容直接存到本机，已有的音视频也能导进来。播放、提取音轨、截图，一个界面搞定。

- **本地语音转文字**：视频里说了啥，直接变成文字稿，在你自己电脑上跑。
- **视频和笔记自动关联**：哪条笔记来自哪个视频，一点就回去。
- **进度一目了然**：下载、转写进行到哪了，失败了为什么，清清楚楚。

### ✅ 交给你常用的 AI，整理成真正能用的笔记

通过 API / MCP 接上你自己在用的 AI Agent，让它根据视频、文字稿和截图帮你写笔记。产出的是标准 Markdown 文件，想用什么编辑器继续改都行。

*说明：笔记内容由你接入的外部 Agent 生成，影记负责管资料、做关联，不是内置的一键写作服务。*

![文档库：查看已登记的 Markdown 笔记](assets/documents.png)

## 🔒 资料全在你自己手里

| 你关心的 | 影记的做法 |
| --- | --- |
| 资料放哪？ | 一个本地主文件夹，媒体、笔记、图片都在里面 |
| 转写要上传吗？ | 不用。只有首次准备环境和模型需要联网，识别在本机完成 |
| AI 能随便看我的资料吗？ | 不能。你核对并批准后才能访问，随时可以撤销 |
| 有云同步吗？ | 当前版本只在本地使用，暂不开放云端登录与同步 |

账号凭据、资料和模型都只存在你的电脑上。外部 Agent 怎么处理资料，取决于你选的工具和服务。

## 📥 下载

| 平台 | 安装包 | 说明 |
| --- | --- | --- |
| macOS · Apple Silicon | [下载 DMG](https://github.com/angrypandahu/yingji-releases/releases/download/v0.0.7/Yingji-0.0.7-macOS-arm64.dmg) | 适用于 M 系列芯片的 Mac |
| Windows · x64 | v0.0.7 安装包另行提供 | 请等待对应版本的 Windows 附件 |

当前版本 **v0.0.7**。每次更新的详情见 [Release 页面](https://github.com/angrypandahu/yingji-releases/releases/latest)。暂不提供 Intel Mac 和 Windows ARM 安装包。

## 三步上手

1. **装上**：Mac 下载 DMG，把 `Yingji.app` 拖进“应用程序”。如果第一次打不开，打开「终端」，复制下面这行执行：

   ```bash
   xattr -cr /Applications/Yingji.app
   ```

   Windows 运行 EXE 安装。
2. **准备一下**：选好资料文件夹，按提示准备运行环境；要转文字的话，顺手装上模型。
3. **开始用**：在「设置 → 来源账号」连上账号，去收藏夹点刷新；想生成笔记，到「设置 → Agent 接入」接上你的 AI。

首次准备需要联网，耗时看网速、模型大小和电脑性能。平台内容能否读取或下载，也取决于账号状态、内容权限和平台限制。

v0.0.6 用户可以在应用内直接升级到 v0.0.7（支持完整和增量更新）。之后 Mac 版本继续走应用内更新，Windows 仍通过完整安装包覆盖更新。

## 常见问题

<details>
<summary><strong>升级后提示“环境尚未准备”，怎么办？</strong></summary>

点「开始准备」重新检查一下就好。运行环境或资源清单变化时会出现这一步，不用清空资料，也不用重新配对 Agent。

</details>

<details>
<summary><strong>更新会删掉我的资料吗？</strong></summary>

不会。安装包和本地资料、模型、运行环境是分开存的，正常覆盖安装都会保留。只要别手动删资料文件夹就行。Mac 的更新入口在「设置 → 通用 → 应用更新」，更新前请先结束正在跑的任务。Windows 本版通过安装程序更新，不提供增量更新。

</details>

<details>
<summary><strong>Mac 第一次打开弹出系统提示？</strong></summary>

当前 macOS 安装包还没有 Apple Developer ID 公证。确认文件来自本仓库的正式 Release 后，把应用拖进“应用程序”，再在终端执行：

```bash
xattr -cr /Applications/Yingji.app
```

这条命令会清掉下载带来的隔离标记。也可以在 macOS「隐私与安全性」里按正常方式允许打开，不需要关闭系统安全保护。

</details>

<details>
<summary><strong>Release 里附件好多，下哪个？</strong></summary>

第一次安装，下上面对应平台的 DMG 或 EXE 就行。名字带 `update`、`delta` 的 ZIP 和 `update.json` 是给应用自动更新用的，不用手动下载解压。校验文件用来核对下载完整性，FFmpeg 源码包用于履行相关许可证要求。

</details>

## 反馈

遇到问题，欢迎在 [Issues](https://github.com/angrypandahu/yingji-releases/issues) 里告诉我：应用版本、系统版本、怎么复现、报错提示。截图或日志记得去掉账号凭据和私人内容。

此仓库只提供影记的公开安装包、更新附件和发行说明，**不是源码仓库**。FFmpeg 等第三方组件的版权与许可随应用分发，对应源码见各版本的 Release 附件。

---

<p align="center"><strong>别让好内容烂在收藏夹里。</strong><br/>👉 <a href="https://github.com/angrypandahu/yingji-releases/releases/latest">现在下载影记</a></p>
