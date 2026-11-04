# 1.3.6 验证

407 项回归测试、2398 条双语文案检查通过。Windows 双产品通过打包启动、通信、地图、五套主题普通/大窗口账号展开、联机分页回顶与日志导入检查；模拟日志覆盖依赖、多原因、正常/未知输出及旧报告排除。两个 GitHub Windows 构建与测试流程均已通过。本轮未新增 macOS/Linux/FreeBSD 1.3.6 包或验证。参见[版本验证](../../prototype/RELEASE-ACCEPTANCE.md)。

# 测试

[English](../TESTING.md)

参见 [版本验证说明](../../prototype/RELEASE-ACCEPTANCE.md)。在此仓库运行 `pnpm test`、`pnpm build`、`pnpm test:sites`、`pnpm release:check` 及 `pnpm desktop:smoke`。微软流程只作为共用核心的模拟回归存在，AmberE 产品不暴露微软登录。第三方真实服务需分别验收。
