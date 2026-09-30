# 领小鼠管理中台

本仓库是领小鼠管理中台的源码快照，包含公司资料、税务日历、团队协作、客户资源、产品研发协作、API / Bug、服务器与权限管理。

## 开发协作模块

- 多产品与多份 Markdown PRD 管理
- 需求评审和技术评审
- 4–5 人开发分工、验收人与任务状态看板
- Bug 复现、排查、根因、修复和验证闭环
- API、日志、开发任务、服务器资源关联
- 所有数据通过后端持久化，不包含业务 Mock 数据

主要入口：

- `src/components/StartupHubPage.tsx`
- `src/components/StartupProductCenter.tsx`
- `shared/startupHub.ts`
- `server/startupHub/store.ts`
- `server/routes/startupHub.ts`

## 本地运行

环境要求：Node.js 22、pnpm 11。

```bash
pnpm install --frozen-lockfile
pnpm run dev:preview:keepalive
```

打开 `http://localhost:5177/startup-hub-preview`。

此快照不包含本地业务数据、账号凭据和自动发布工作流。原始来源提交：`f811edd0719a70e59a4daa566ea294660e8b98d5`。
