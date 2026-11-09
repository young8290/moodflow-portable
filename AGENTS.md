# Moodflow 便携启动器

本分支采用已公开的 MIT 源码，保留 LICENSE 和原始署名；不合并上游改为其他许可后的代码。GUID、RPC 和文件名须与 Moodflow 主仓对应。

测试只使用临时目录，不注册输入法、杀真实进程或写系统自启。复制部署不携带 userdata/localdata，拒绝重解析点；程序生命周期仅操作用户明确选择的本目录实例。运行 cargo fmt、cargo test、cargo clippy --all-targets，使用显式路径提交。
