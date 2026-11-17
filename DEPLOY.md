# 公开部署（待完成的一小步）— ML Empowerment Build Challenge 4.0

作品本身已完成并本地验证通过（`index.html` HTTP 200、4 张截图已拍好）。
公开链接还没拿到，原因不是技术问题，而是下面三个免费渠道都需要一次用户/主 agent 的操作
（助手这边没有 Cloudflare 凭证、Vercel/Replit 未连接、GitHub App 不能新建仓库）。
三选一，都是免费、不用绑卡：

## 选项 A（推荐）：GitHub Pages — 新建一个空公开仓库

1. 在 GitHub 上新建一个**公开**空仓库，名字建议 `cet4-wrongbook-explainer`
   （https://github.com/new ，不勾选 README，不花钱）。
2. 把本目录的全部文件推上去（`index.html`、`README.md`、`.github/workflows/pages.yml` 已备好）。
   推送后工作流会自动跑，第一次运行会自动开通 Pages。
3. 等 1–2 分钟，打开 `https://kornztt.github.io/cet4-wrongbook-explainer/` 验证 200。
4. 把这个链接填进 `SUBMISSION.md` 的 Demo URL，再去 Devpost 提交。

为什么助手没直接做：GitHub App 的 `create_repository` 返回
`403 Resource not accessible by integration`——GitHub App 本来就不能代建个人仓库，
只能等用户（或主 agent 用浏览器）建好空仓库。

## 选项 B：Vercel — 连接一次即可部署

1. 打开 Vercel 连接页完成授权（免费 Hobby 档，不用绑卡）：
   https://agent.meta.ai/connectors/connect/vercel
2. 连接成功后助手可用 `create_deployment` 直接部署，拿到 `*.vercel.app` 链接并验证。

## 选项 C：Qoder Sites — 用户在 Qoder 里发布

按 `~/workspace/tianchi-qoder-2026/QODER.md` 的方式 A：
在 Qoder 里用 `@sites`，把本目录 `index.html` 作为附件发过去，
预览确认后点「发布」，访问范围设为「任何人都可访问」，复制公开链接。

## 明确不做的事

- 不碰用户已有的 Cloudflare Workers 账号（里面有 R2、hello-test、static-site，
  动它有连带风险，且助手没有它的凭证；也不会覆盖已有的 static-site）。
- 不开新 Devpost 账号（绕过封禁会被当成违规，连累申诉和 Codegeist）。
- 不花钱、不绑卡、不注册新付费账号。
