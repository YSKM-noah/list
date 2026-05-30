# 拾光清单 0.1.2 试用版记录

日期：2026-05-31

## 已完成

- 新建任务的 LLM 模式支持读取文档上下文，当前支持 PDF、DOCX、TXT 和 Markdown。
- 新增 `todo.split_task` Agent skill，用于把重大任务拆分为可执行子任务。
- 子任务会记录父任务来源，并在列表和详情里展示所属父任务。
- 拆分任务时会把父任务截止日期之前的未完成任务作为日程上下文，让 Agent 避免生成不现实的安排。
- 修复设置页打开后页面被拉宽的问题。
- 当日任务支持切换查看日期。
- 月历点击日期时展示该日任务的精简悬浮预览。
- LLM 创建任务发送消息后会清空输入框。

## 产物

Release exe：
```text
D:\program\shiguang-list\src-tauri\target\release\shiguang-list.exe
```

便携试用包：
```text
D:\program\shiguang-list\release\shiguang-list-portable-0.1.2.zip
```

## 验证结果

- `npm.cmd run build --prefix .\shiguang-list`：通过。
- `cargo check --manifest-path .\shiguang-list\src-tauri\Cargo.toml`：通过。
- `npm.cmd run tauri --prefix .\shiguang-list -- build --no-bundle`：通过。
- 便携包 exe 启动验证：进程保持运行。

## 后续建议

- 继续观察 `todo.split_task` 的拆分质量，补充更稳定的 JSON 输出校验和用户可编辑预览。
- 下一轮优先完善 Agent skill contract，让后续 TODO-Agent 功能可以按 skill 独立扩展。
- 后续补正式安装器打包流程。
