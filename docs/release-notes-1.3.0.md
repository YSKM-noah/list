# it knows you better 1.3.0

本版本把知识库接入独立 Agent skill 体系，让知识条目可以反向驱动 TODO。

## 新增

- 新增 `knowledge.summarize` skill：根据知识条目生成结构化 Markdown 总结。
- 新增 `knowledge.extract_tasks` skill：从知识条目提取可执行任务草稿。
- 知识库预览区新增 `Agent 总结` 和 `提取任务` 操作。
- Agent 总结结果支持先预览，再写入当前知识草稿。
- 提取出的任务支持先预览，再批量写入 TODO。
- 从知识条目写入 TODO 后，会自动把新任务关联回当前知识草稿。

## 说明

- 本版本继续保持 Agent、TODO、Knowledge Base 三个模块的职责边界：Agent 只生成结构化建议，TODO 和知识库负责最终保存。
- 本公开仓库只用于下载页和 Release 说明。GitHub 自动生成的 `Source code` 压缩包不是应用源码。
- 语义搜索和相似知识推荐放到后续版本继续做。
