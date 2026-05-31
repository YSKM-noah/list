# it knows you better 1.0.0 v1 正式版

日期：2026-05-31

## 版本定位

这是 `it knows you better` 的 v1 正式版。

## 新版本变化

- 项目正式更名为 `it knows you better`。
- 保留完整 TODO 基础能力：任务创建、编辑、完成、删除、计时、预计用时、实际用时。
- 新增任务卡片中的明确“结束”入口。
- 新增独立工作统计页面，支持自由选择时间段。
- 工作统计支持实际用时、预计用时、实际偏差、工作类型占比和关键词点云。
- Agent 模块独立成侧边栏入口，支持基础配置和连接测试。
- 新建任务支持手写模式和 Agent/LLM 创建模式。
- Agent/LLM 创建任务支持上传 PDF、DOCX、TXT、Markdown 文档作为上下文。
- 任务详情支持交给 Agent 一键拆分为子任务。
- 子任务会展示所属父任务来源。

## 下载

请在本版本 GitHub Release 附件中下载：

```text
it-knows-you-better-portable-1.0.0.zip
```

## 验证结果

- 前端构建通过。
- Rust 检查通过。
- Tauri release exe 构建通过。
- 便携包 exe 启动验证通过。
