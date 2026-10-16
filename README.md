# Polaris 下载

Polaris 是桌面 Agent 任务面板，提供悬浮球、会话管理及任务执行进度，目前适配本机 Codex。本仓库仅提供安装包与发行说明。

## 可下载版本

| 平台 | 当前状态 | 下载 |
|---|---|---|
| macOS · Apple Silicon（M 系列） | 1.10.39（79）预览版 | [版本说明与附件](https://github.com/Arika1415/Polaris-Releases/releases/tag/v1.10.39) |
| macOS · Intel | 尚无已验收安装包 | 暂未发布 |
| Windows | 开发中，尚未达到验收标准 | 暂未公开发布 |

本版新增 GitHub 在线更新：在 `… → 更新与版本…` 中检测新版，点击安装后自动下载、校验、替换并正常退出重启。保留发送键旁模型切换、滚动修复、中英文界面与原生输入框。当前适配 Codex。

**1.10.38 及更早版本需要先手动安装一次 1.10.39，之后才能使用应用内在线更新。** 更新无需 GitHub 账号或开发工具；运行中的任务仍有退出确认，取消重启后可稍后启用新版。

## Mac 安装

1. 在上面的版本页面下载 `Polaris-1.10.39-79-arm64-release.dmg`；不要将 GitHub 自动生成的 Source code ZIP 当成安装包。
2. 需要校验时，同时下载同名 `.sha256` 文件。
3. 打开 DMG，将应用复制到自己的 Applications 目录。已有旧版时保留原安装位置；先保存任务并正常退出旧版，再替换该位置的应用。
4. 安装并登录本机 Codex。Polaris 安装包不包含模型服务或订阅。

构建目标为 macOS 13.0 及以上、Apple Silicon（arm64）。macOS 13.6.7 已完成编译兼容检查，尚未在该系统实机验收；请按预览测试版使用。

## 分发说明

当前为预览包，使用 ad-hoc 本地签名，尚未完成 Apple Developer ID 签名和公证，可能被 Gatekeeper 拦截；不是 App Store 发行版。

发布安装包不等于开源。本仓库不提供 Polaris 源码或开源授权。包内保留必要的第三方运行资源和许可证，不包含开发源码、测试、账号凭据或聊天历史。

## 校验下载文件

将 DMG 和 `.sha256` 放到同一目录，在该目录执行：

```sh
shasum -a 256 -c Polaris-1.10.39-79-arm64-release.dmg.sha256
```

更多历史版本见 [Releases](https://github.com/Arika1415/Polaris-Releases/releases)。
