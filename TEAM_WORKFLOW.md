# LabY 团队协作流程

这份文件是团队日常协作约定。新成员先看 [GitHub 新手协作指南](https://github.com/laby-ai/.github/blob/main/GITHUB_BEGINNER_GUIDE.md)，再看这里。

## 一句话规则

修改已有项目时：**不要直接改 `main`，新建分支，提交 Pull Request，等 review 后合并。**

## 任务流

1. 先确认任务属于哪个仓库。
2. 有明确问题就开 issue；已经有 issue 就在下面留言认领。
3. 从最新 `main` 新建分支。
4. 在自己的分支上修改。
5. 提交 PR，并写清楚改动、原因和检查方式。
6. 等 review；有意见就继续在同一个分支修改。
7. 通过后再合并。

## 分支命名

推荐：

```text
名字/任务简称
feature/功能简称
fix/问题简称
docs/文档简称
```

例子：

```text
mengwei/add-readme
feature/audio-summary
fix/upload-error
docs/setup-guide
```

## PR 要求

PR 还需要符合 [工程与交付规范](https://github.com/laby-ai/.github/blob/main/ENGINEERING_STANDARDS.md)，尤其是代码可维护性、用户交付体验和测试检查证据。

PR 不需要写长，但必须可判断：

- 改了什么
- 为什么改
- 怎么检查
- 有没有风险或后续工作

如果只是文档修改，也写一句“只改文档，未跑代码测试”。

## Review 规则

- 小改动：至少 1 人看过再合并。
- 影响运行、部署、数据、权限的改动：必须 Maintainer 看过。
- 不确定的设计选择：先在 issue 或 PR 里讨论，不要直接大改。

## 合并前检查

合并前至少确认：

- 没有提交密码、token、私钥、`.env` 等敏感文件。
- README 或文档是否需要同步更新。
- 能说明自己怎么检查过。
- PR 范围集中，没有混入无关重构。

## 新手遇到问题

卡住时优先把问题写清楚：

```text
我在哪个仓库 / 哪个分支
我想做什么
我执行了什么命令
出现了什么报错或截图
```

不要因为冲突、报错或看不懂提示就强行点合并。