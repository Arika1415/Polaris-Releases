# Polaris — Downloads

Polaris 是原生 macOS Agent 任务面板，提供悬浮球、对话与任务管理，目前支持本机 Codex。

[下载安装包](https://github.com/Arika1415/Polaris-Releases/releases)

## 当前预览版

- 版本：1.10.32（72）
- 架构：Apple Silicon（M 系列芯片），不支持 Intel Mac。
- 构建目标：macOS 14.0 及以上；目前仅在开发机 macOS 26.5.2 验证，未完成各旧系统版本实机测试。
- 需要另行安装并登录本机 Codex；不包含模型服务或订阅。
- 下载 DMG，将 Polaris.app 拖入 Applications 后启动。
- 已安装旧版的用户请使用程序内“更新与版本”选择 DMG 中的应用，以保留原安装路径。

## 分发状态

当前为预览测试包，使用 ad-hoc 本地签名，尚未完成 Apple Developer ID 签名及公证；下载后可能被 macOS Gatekeeper 拦截。不是 App Store 发行版。

本仓库仅用于安装包与版本说明，不提供 Polaris 源码，也不授予开源许可。包内保留第三方运行资源及其许可证。安装包不含开发源码、测试文件、账号凭据或聊天历史。

## 完整性校验

每个 DMG 附有 `.sha256` 文件，将两者下载到同一目录后运行：

```sh
shasum -a 256 -c Polaris-1.10.32-72-arm64-release.dmg.sha256
```
