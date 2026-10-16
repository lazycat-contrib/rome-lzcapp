# Rome for LazyCat

上游：https://github.com/rome-os/rome

包名：community.lazycat.app.rome（前缀来源 default）

Mirror 模式，跟踪镜像稳定 SemVer，目标 linux/amd64；只发布喵喵商店。

保留上游 Guardian 会话认证及首次初始化流程。首次启动需复制内置运行时到持久目录，可能较慢。包含浏览器运行环境，依照上游需要 SYS_ADMIN、1GB共享内存和 FUSE 权限；只授予可信用户。禁用宿主执行助手及个人微信集成。不暴露独立 CDP/noVNC 端口。未配置可选的集中式 OTEL 日志收集服务。

public_path / 按用户要求开放，保留上游自身认证。文件操作接入懒猫网盘选择器。图标为上游组织 GitHub 头像。

GitHub Action 默认 dry-run；手动将 dry-run=false 才会正式发布。组织配置 APPSTORE_URL、APPSTORE_TOKEN、可选 PRIVATE_STORE_GROUP_CODES。
