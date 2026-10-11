# Harbor Yingji / 影记下载

此仓库仅公开安装包、更新清单及发行说明。应用源码单独维护，不在这里公开。

[下载最新版本](https://github.com/angrypandahu/harbor-releases/releases/latest)

支持 Mac Apple Silicon（M系列芯片）。首次安装下载 DMG，把 `Harbor Yingji.app` 放入本人可写的应用目录。v0.0.4 起使用完整临时签封并严格校验，但尚无 Apple Developer ID 签名/公证；系统要求时通过 macOS 提供的正常批准方式首次启动。

## 更新

v0.0.2 及更早需要手动安装最新版，保留原有资料和运行环境。v0.0.3 起，在「设置 → 通用 → 应用更新」主动检查、下载并重启安装；首次准备页也有更新入口。更新时保持默认应用名称，先结束正在运行的任务。

安装程序验证发行签名、完整性及候选应用签封；基线匹配时使用增量包，否则下载全包。资料、模型、Python运行环境保留；安装失败保留或恢复旧应用。ZIP及签名update.json是更新器使用的发行附件，不需要手动选择增量包。

每次发行提供 DMG、完整 ZIP、增量 ZIP、签名更新清单、SHA256SUMS及FFmpeg源码。FFmpeg采用LGPL，相关版权和许可包含在应用内。不要下载或使用未在本仓库稳定Release列出的更新包。

v0.0.4 明确应用/服务版本：application_version 是应用发行号（0.0.4），service_version 和旧 version 是服务号（0.1.0）。MCP initialize 使用服务号，SDK 1.28.1 仅是依赖版本。两个 Agent 原凭据和独立目录授权跨退出重启、实际增量升级与撤销隔离均有自动回归。首次补齐 Electron 框架签封，本版增量包比单纯业务差异大。
