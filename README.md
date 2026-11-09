# Moodflow 便携启动器

Windows 原生启动器，协调 Moodflow 核心、TSF、设置程序和 Hub。发布与开发变体使用 Moodflow 的 GUID、管道、目录和互斥锁。程序代码遵循 MIT，原作者与贡献者声明保留在 LICENSE。

`cargo build --release` 构建；主仓注入 `MOODFLOW_APP_VERSION`，随完整便携包分发。便携标记为 `portable_mode`，用户词库位于 `userdata/`，Hub 与本机工具数据位于 `localdata/`。复制部署跳过这两处；更新也不覆盖它们。

启动时拒绝接管另一目录的 Hub，停止时只结束本目录的 Hub 与设置程序。系统输入法注册和程序启动均由用户显式执行；单元测试只处理临时文件。

对应源码和历史出处见 [MOODFLOW-SOURCE.md](MOODFLOW-SOURCE.md)，原版使用说明保留在 UPSTREAM-README.md。
