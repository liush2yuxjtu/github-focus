# GitHub Focus

中文 GitHub 活动解读应用，使用 [baoyu-design](https://github.com/JimLiu/baoyu-design) 的设计方法制作。

**[打开应用](https://liush2yuxjtu.github.io/github-focus/)**

- 三条焦点主线：Atelier、my-release-skills、A Dark Room。
- 六个公开仓库的 commit / PR 快照，可按仓库、类型和关键词过滤。
- 分开展示已核实记录、编辑解读、建议和待验证项。
- 按需检查主线默认分支的新提交；没有定时任务，没有密钥。

## Development

Buildless HTML / CSS / JavaScript. Run `python3 -m http.server 4311`, then open the served URL. GitHub Pages serves the repository root from `main`. No Actions workflow is required.

`data.json` contains only selected public GitHub API fields. The snapshot reads at most 8 default-branch commits and 8 recently updated PRs per repository, so it must not be interpreted as total activity or a productivity score. PR merge status is not deployment verification. The app's manual check does not rewrite editorial analysis.

Design provenance: JimLiu/baoyu-design, commit `6530033592bf7fa58bc1a5a2a2ad278da45213a9` (MIT). This app is independently authored; no hosted Claude Design service is used.
