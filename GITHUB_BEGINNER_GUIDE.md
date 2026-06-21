# LabY GitHub 新手协作指南

这份指南给刚开始用 GitHub 的同学。先记住一句话：**不要直接改 `main` 分支。改已有项目时，先新建自己的分支，再提交 Pull Request。**

## 1. 接受组织邀请

1. 打开 GitHub 发到邮箱里的邀请邮件。
2. 登录或注册 GitHub 账号。
3. 点接受邀请，加入 `laby-ai` 组织。
4. 加入后打开组织主页：https://github.com/laby-ai

## 2. 修改已有项目的标准流程

不要直接在 `main` 上改代码。推荐流程是：

1. 打开要修改的仓库。
2. 先看 `README.md`，确认项目怎么运行、怎么测试。
3. 从 `main` 新建一个分支。
4. 在自己的分支上修改。
5. 提交 commit。
6. push 到 GitHub。
7. 创建 Pull Request，等别人 review。
8. review 通过后再合并到 `main`。

## 3. 分支命名怎么写

分支名用英文、数字和短横线，尽量看得出是谁在做什么。

推荐格式：

```text
你的名字/任务简称
```

例子：

```text
yanjiajia/fix-login-page
mengwei/add-readme
feature/data-cleaning
bugfix/upload-error
```

如果不会英文，可以先用拼音和简单词：

```text
xiaoming/update-doc
jiaojiao/fix-bug
```

## 4. 常用命令

第一次下载项目：

```bash
git clone https://github.com/laby-ai/仓库名.git
cd 仓库名
```

开始改之前，先拉最新代码：

```bash
git checkout main
git pull
```

新建自己的分支：

```bash
git checkout -b 你的名字/任务简称
```

查看改了哪些文件：

```bash
git status
```

提交修改：

```bash
git add .
git commit -m "简单说明这次改了什么"
```

上传分支：

```bash
git push -u origin 你的名字/任务简称
```

然后去 GitHub 页面创建 Pull Request。

## 5. Pull Request 怎么写

PR 标题要短，说明这次做了什么。

PR 内容建议写三块：

```text
## 改了什么
- 

## 为什么改
- 

## 怎么检查
- 
```

如果没有测试，也要写清楚自己怎么手动看过。

## 6. 不要做这些事

- 不要直接 push 到 `main`。
- 不要把密码、API Key、token、个人隐私文件提交到仓库。
- 不要一次 PR 改很多不相关的东西。
- 不要删除别人正在用的文件，除非已经确认。
- 不确定时先开 issue 或在群里问。

## 7. 自己新建项目时

可以自己在 `laby-ai` 组织下创建仓库。建议：

- 仓库名用英文小写和短横线，例如 `course-demo`、`ai-agent-notes`。
- 先创建 `README.md`，写清楚项目是做什么的。
- 如果只是内部实验，优先建 private 仓库。
- 如果要公开展示，再建 public 仓库。

## 8. 遇到冲突怎么办

如果 GitHub 提示 conflict，不要乱点。先在群里说：

```text
我这个 PR 和 main 冲突了，谁能帮我看一下？
```

也可以先执行：

```bash
git checkout main
git pull
git checkout 你的分支
git merge main
```

如果看不懂冲突内容，先停下来，不要强行提交。

## 9. 最简单记忆版

改已有项目：

```text
拉最新 main -> 新建分支 -> 修改 -> commit -> push -> Pull Request -> review -> merge
```

只要遵守“不直接改 main”，大部分问题都可以安全修回来。
