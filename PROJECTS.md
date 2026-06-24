# LabY 项目目录

这个文件记录 `laby-ai` 组织里的项目入口和维护状态。新建仓库后建议同步更新这里，方便新成员快速知道每个仓库是做什么的。

## 项目列表

| 仓库 | 可见性 | 主要技术 | 当前定位 | 建议维护人 |
| --- | --- | --- | --- | --- |
| [knowtrail](https://github.com/laby-ai/knowtrail) | Public | TypeScript | NotebookLM-style source-grounded workspace：引用问答、音频摘要、slides、课堂流和知识路径。 | 待指定 |
| sceneweave | Private | TypeScript | AIGC short-film studio：分段视频生成、frame handoff、音频连续性和可恢复生产流。 | 待指定 |
| [.github](https://github.com/laby-ai/.github) | Public | Markdown | 组织主页、默认模板、新手指南和协作规范。 | Owners / Maintainers |

## 仓库状态建议

每个仓库 README 建议至少写清楚：

- 项目一句话说明
- 当前负责人或维护人
- 本地运行方式
- 测试或检查命令
- 常见问题
- 当前阶段：实验 / 内测 / 可展示 / 暂停维护

## 新建仓库命名

优先使用英文小写和短横线：

```text
course-demo
agent-notes
video-pipeline
ui-experiments
```

内部实验优先创建 private 仓库。确定要公开展示或开源时，再切换为 public，并先检查 README、许可证、敏感信息和演示说明。