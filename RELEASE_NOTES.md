# Anything Analyzer v3.3.4

## Bug 修复

- **修复界面白屏** — 恢复 v3.3.3 中被误删的窗口控制、指纹伪装、Shell 等 IPC handlers，修复应用启动后白屏无法使用的问题
- **修复追问对话消失** — 旧报告（v3.3.3 之前生成）打开后发送追问，消息和回答不可见的问题；现在会自动重建对话上下文并回写数据库
- **修复取消分析功能** — 恢复 AbortController 逻辑，分析过程中可正常取消
- **恢复 react-window 依赖** — 修复虚拟列表组件因缺少依赖导致的渲染异常

## 改进

- **网络错误诊断增强** — 提取 `err.cause` 展示真实错误原因，不再被 `fetch failed` 兜底信息吞掉细节
- **MCP Server 认证恢复** — 恢复 Bearer token 自动生成和认证开关功能

## 下载

| 平台 | 文件 |
|------|------|
| Windows | `Anything-Analyzer-Setup-3.3.4.exe` |
| macOS (Apple Silicon) | `Anything-Analyzer-3.3.4-arm64.dmg` |
| macOS (Intel) | `Anything-Analyzer-3.3.4-x64.dmg` |
| Linux | `Anything-Analyzer-3.3.4.AppImage` |
