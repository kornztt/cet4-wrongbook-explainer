# ML Empowerment Build Challenge 4.0 — Submission Notes

> 状态（2026-11-17 21:26）：作品已完成、已推上 GitHub、GitHub Pages 已开，公开链接已实测能打开。
> 还差一步：Devpost 提交（Devpost 账号仍在暂停申诉中，**不要开新号**，等解封后提交）。

## Suggested project title（最终版，直接粘贴）

**CET-4 Wrong-Question Explainer — Rule-Based CET-4 MCQ Tutor**

## Suggested description（最终版，直接粘贴）

CET-4 Wrong-Question Explainer is a tiny, free, offline-first web app for Chinese university students preparing for CET-4. Paste a multiple-choice question and it gives a structured breakdown — the tested grammar point, key vocabulary, distractor traps, and a step-by-step method — using a transparent rule-based engine (no API, no fake AI claims). It ships with 10 built-in sample questions and a wrong-question book saved in the browser with 1/3/7-day spaced review reminders, so students stop repeating the same mistakes.

## Demo URL

- 公开链接（已实测 2026-11-17 21:26 能打开，标题和讲解、例题、错题本都显示正常）：https://kornztt.github.io/cet4-wrongbook-explainer/
- 仓库：https://github.com/kornztt/cet4-wrongbook-explainer ，公开仓库，文件：`index.html`、`README.md`、`SUBMISSION.md`、`DEPLOY.md`（`.github/workflows/pages.yml` 因 GitHub App 无 workflows 权限推不上去，改用 Settings > Pages > Deploy from a branch 部署，不影响使用）

## Track / category

- Education / AI for learning (rule-based explanation engine)
- Solo project, free entry, no cash prize expected — the goal is the participation certificate and a usable study tool.

## Screenshots（已拍好，在 `screenshots/`，2026-11-17 实机渲染验证过）

1. `screenshots/1-home.png` — 首页：输入框 + “讲解这道题”按钮。
2. `screenshots/2-explain-result.png` — 例题 2 的讲解结果：参考答案 B、考点 not until…that…、生词、干扰项陷阱、正确思路全部可见。
3. `screenshots/3-sample-questions.png` — 10 道内置例题完整列表。
4. `screenshots/4-wrongbook-review.png` — 错题本：已加入例题 2，答案 B，加入 2026-11-17，复习日 2026-11-18 / 2026-11-20 / 2026-11-24，下次复习 2026-11-18。

## What to submit on Devpost

- Project title + description（见上，已定稿）。
- Demo URL（待 `DEPLOY.md` 完成后填）。
- Repository link（与演示站同仓库）。
- 4 张截图（已备好，直接上传）。

## Checklist before submitting

- [x] 作品完成：`index.html` 单文件静态站，无后端、无 API、无外部依赖。
- [x] 本地验证：`python3 -m http.server` 返回 HTTP 200，标题正确；Firefox 实机渲染 4 张截图全部验证过。
- [x] 4 张截图已拍好（见上）。
- [x] 手机适配：CSS 有 max-width 600px 适配；localStorage 只存本机。
- [x] Host `index.html` 到公开链接：https://kornztt.github.io/cet4-wrongbook-explainer/ ，2026-11-17 21:26 实测能打开。
- [x] 在公开链接上复测一遍：标题、粘贴讲解、错题本 1/3/7 天复习都显示正常。
- [ ] 确认 Devpost 账号解封，再提交。截止：2026-12-02 02:45 EST（2026-12-02 15:45 北京时间）——至少提前一天交。
- [ ] Do not claim it is generative AI; the README already says “rule-based” honestly.
