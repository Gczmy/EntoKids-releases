# EntoKids 安卓测试版

本仓库只用于发布安卓安装包、更新清单和版本说明。EntoKids 源码保留在私有仓库，下载安装及应用内更新无需登录 GitHub。

当前版本：**0.1.0-dev.7**（Pre-release，Android 8.0 及以上）。包含现有全部课程图片和配音，可离线阅读；内容仍属开发草案，最终人工审校和真机验收尚未完成。

| 当前情况 | 安装入口 |
| --- | --- |
| 新设备，或已安装公开 v5/v6 | [下载标准安装包](https://github.com/Gczmy/EntoKids-releases/releases/download/dev-v7/EntoKids-7.apk) · [版本说明](https://github.com/Gczmy/EntoKids-releases/releases/tag/dev-v7) |
| 已安装原私有 v3 测试版 | [下载 v3 兼容安装包](https://github.com/Gczmy/EntoKids-releases/releases/download/dev-legacy-v7/EntoKids-7.apk) · [版本说明](https://github.com/Gczmy/EntoKids-releases/releases/tag/dev-legacy-v7) |

旧 v3 设备使用兼容包覆盖安装一次，请保留原应用，避免卸载清除学习记录。兼容包沿用原 v3 签名，课程内容与标准包相同；学习记录保留仍需在实际设备上验收。其他来源的旧安装包不能据此保证覆盖安装。

安装后进入家长区，选择“检查更新”。之后下载和安装更新均由家长主动确认；应用会核对清单签名、完整文件及当前安装签名，再打开 Android 系统安装器。更新是完整 APK，系统可能要求允许 EntoKids 安装未知应用。

首次安装最新版时，“已是最新版本”是正常结果；下次发布更高版本才会出现更新。更新失败不影响现有课程的离线阅读。

目前分发地址为 GitHub，尚无国内镜像；国内网络可达性和真机更新流程待测试。

## 公开发布内容

每个 Pre-release 仅包含 APK、签名 `update.json`、版本说明和 SHA-256 校验文件。`channels/development/update.json` 为标准版本清单，`channels/development-legacy/update.json` 为原 v3 兼容清单。两者采用同一清单公钥，应用只接受与自身 APK 签名一致的版本。私钥、仓库凭据和源码不会进入本仓库。

正式 stable 渠道尚未启用。
