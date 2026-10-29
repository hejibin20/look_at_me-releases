# Mirror 安装包与更新源

这里只分发完整安装包与签名更新清单，不存放私有源码、用户数据、账号令牌或签名私钥。

## 下载

- [正式版本](https://github.com/hejibin20/look_at_me-releases/releases/latest)
- 初始 0.1.0 目前只提供 Linux amd64 DEB，包含日历、Python 后台和专注保护服务。
- Windows/macOS 安装包需要在对应系统构建；不要下载其他系统的包。

首次手动安装含更新功能的版本后，可在「设置 → 应用更新」使用更新。默认自动检查和下载，安装前仍须确认及必要的管理员授权。专注或主动屏蔽有效时不会安装更新。

## 测试主动更新

在「设置 → 应用更新 → 更新源」点击「填入 GitHub 测试源」并保存。保持自动检查下载开启，即可演练检查与下载。

测试源：`https://github.com/hejibin20/look_at_me-releases/releases/download/v0.1.1-demo/mirror-update.json`

演练 Release 为 prerelease，清单签名包含 test_only=true，前后端都禁止安装。文件只有占位文本，并非应用安装包。它不会成为正式 latest。演练结束后恢复「GitHub 更新源」。

正常更新源：`https://github.com/hejibin20/look_at_me-releases/releases/latest/download/mirror-update.json`

所有包都应验证签名、大小和 SHA-256；不允许降级，不清空个人数据或专注安全账本来升级。
