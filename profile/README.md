# LabY

LabY 是一个面向 AI 产品实验、工程协作和研究原型的团队组织。这里放团队正在推进的项目、共享文档和协作规范。

## 快速入口

| 入口 | 用途 |
| --- | --- |
| [新成员 GitHub 指南](https://github.com/laby-ai/.github/blob/main/GITHUB_BEGINNER_GUIDE.md) | 第一次加入 GitHub / 不熟悉分支和 PR 的同学先看这里。 |
| [团队协作流程](https://github.com/laby-ai/.github/blob/main/TEAM_WORKFLOW.md) | 约定怎么开 issue、建分支、提 PR、review 和合并。 |
| [项目目录](https://github.com/laby-ai/.github/blob/main/PROJECTS.md) | 查看当前组织里的项目、可见性和维护状态。 |
| [Contributing](https://github.com/laby-ai/.github/blob/main/CONTRIBUTING.md) | 默认贡献说明，适用于组织下大多数仓库。 |

## 当前项目

| 项目 | 状态 | 说明 |
| --- | --- | --- |
| [knowtrail](https://github.com/laby-ai/knowtrail) | Public | NotebookLM 风格的 source-grounded workspace，包含引用问答、音频摘要、slides、虚拟课堂和知识路径。 |
| sceneweave | Private | AIGC 短片生产工作流，关注分段视频生成、镜头衔接、音频连续性和可恢复生产。 |
| [.github](https://github.com/laby-ai/.github) | Public | 组织主页、默认模板和成员协作说明。 |

## 基本协作约定

- 不直接改 `main`。修改已有项目时，先新建分支，再提交 Pull Request。
- 新任务先开 issue 或在已有 issue 下认领，避免多人做重复工作。
- 每个 PR 都要写清楚：改了什么、为什么改、怎么检查。
- 重要仓库由 Maintainers review 后再合并。
- 密码、API Key、token、个人隐私文件不能提交到仓库。

## 团队权限

- `Owners`：组织设置、成员管理、关键权限。
- `Maintainers`：仓库维护、review、release 和合并决策。
- `Contributors`：日常开发、文档、实验和 PR 协作。

## 新仓库建议

新建仓库时，至少补齐：

- `README.md`：项目目标、运行方式、检查方式。
- Issue/PR 流程：用 issue 记录任务，用 PR 合并改动。
- 可见性：内部实验优先 private；准备公开展示再 public。
- 维护人：README 里写清楚谁负责当前仓库。