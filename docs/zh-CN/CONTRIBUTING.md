# 贡献指南

[English](../../CONTRIBUTING.md)

使用 Windows x64、Node.js 24 与 pnpm 11.25.0，在 `prototype` 目录依次执行：

```sh
pnpm install --frozen-lockfile
pnpm test
pnpm build
pnpm test:sites
pnpm release:check
pnpm desktop:smoke
pnpm desktop
```

`pnpm dev` 仅是浏览器预览，真实文件操作和启动需使用桌面版。`pnpm package:installer` 构建 x64 NSIS 安装包。删除等破坏性操作只能在临时测试实例上验证。


中英文文档同步更新。新增应用文案须加入翻译目录，保留稳定键与占位符。参见语言包指南。用户名称、文件名、项目介绍和执行参数不翻译。

保留事务回滚、路径校验、可信下载来源、哈希校验、渲染器权限隔离和凭据脱敏；行为改动应有回归覆盖。不提交账号库、个人原始日志、凭据、本地缓存或安装器。敏感漏洞按安全政策报告。

项目自有改动采用 MPL-2.0，保留依赖和素材声明。PR 说明用户可见变化、验证结果与限制，界面模拟检查不能表述为真实游戏验收。


## 1.3.5 platform builds / 平台构建

See [platform build inputs and verification limits](../../prototype/PLATFORMS-1.3.5.md). Publish the accepted package bytes unchanged. Keep architecture-specific native map engines and their source manifest; platform artifacts are not interchangeable. No signing credentials or private account data belong in source exports.

## 任务交付与正式发布

Dot 协调任务聊天并审核 PR。每个任务 PR 提供可下载的测试安装包、对应提交、验证结果与限制，由用户测试并决定是否合并。正式发布由用户另行要求，可汇总多个已合并 PR；从主分支构建正式包，同步发布说明、中英文文档及 GitHub Pages。

本仓库默认构建 AmberE；`pnpm package:installer` 生成独立安装包，`pnpm release:source` 导出源码。共用核心来自 AMBER，保留上游版权与许可证；同步功能改动时保留本项目的认证限制、应用身份、品牌和更新仓库。
