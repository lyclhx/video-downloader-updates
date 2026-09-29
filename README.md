# video-downloader-updates

视频抓取下载器更新说明与 Windows x64 安装包。

## 最新版本：v4.8.9（2026-09-30）

相对 v4.8.8，本版修复 Windows 启动时写入机器级根证书需要管理员权限的问题：应用根证书改装到当前用户的受信任根证书库；旧机器级证书因权限无法清理时记录警告并继续启动，重置或卸载仍会报告清理失败。

验证：全量 Go 测试、`go vet`、前端类型检查与生产构建、Windows x64 Wails 构建及 ZIP 七文件清单校验通过。

边界：Instagram 页面加载/登录、旧机器级证书清理和其他电脑验收尚未完成；本版不代表所有平台功能均已无故障。

下载：[res-downloader-windows-amd64.zip](https://github.com/lyclhx/video-downloader-updates/releases/download/v4.8.9/res-downloader-windows-amd64.zip)

SHA-256：`bc6b576f2ec8956324c274a15c865fb78400260e630e519c6b1652da78dc3371`