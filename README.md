# FunComics

FunComics 是一个面向独立作者的 AI 漫画创作与连载工作台首版原型，围绕一条主链路组织七个板块：

```text
故事项目 → 角色资产 → 分镜脚本 → 漫画编辑 → 连载版本 → 发布阅读 → 社区反馈
```

## 启动

```bash
npm install
npm run dev
```

## 验证

```bash
npm test
npm run build
```

## 当前边界

- 当前版本使用本地演示数据，图像生成通过 `GenerationAdapter` 接口预留接入位，不在前端暴露模型密钥。
- 作品、角色、分镜、章节和发布版本共享同一个项目状态，避免七个板块各自维护一套状态。
- 规格约束见 `docs/specs/2026-10-20-ai-comics-workbench.md`。
- 实施计划见 `docs/superpowers/plans/2026-10-20-ai-comics-workbench.md`。
