# Contributing to LabY

LabY 使用 issue + branch + Pull Request 作为默认协作方式。中文说明优先；英文可以补充，但不强制。

## 开始前

- 改已有项目时，不要直接改 `main`。
- 先确认任务是否已有 issue，避免重复工作。
- 改动涉及 API、部署、数据结构、权限或依赖时，先让 Maintainer 知道。
- 尽量让每个 PR 只解决一个明确问题。

## 标准流程

```text
拉最新 main -> 新建分支 -> 修改 -> commit -> push -> Pull Request -> review -> merge
```

推荐分支名：

```text
你的名字/任务简称
feature/功能简称
fix/问题简称
docs/文档简称
```

## PR 内容

PR 至少说明：

- 改了什么
- 为什么改
- 怎么检查
- 风险和后续工作

没有自动测试也没关系，但要写清楚手动检查方式。

## 不要提交

- 密码、token、API Key、私钥
- `.env`、本地缓存、个人数据
- 大型生成文件，除非仓库明确需要
- 和当前任务无关的大范围重构

## Review

Review 重点看：正确性、可维护性、安全风险、是否容易验证。评论要具体，能让作者知道下一步怎么改。