# it knows you better 0.2.0 试用版记录

日期：2026-05-31

## 已完成

- 项目可见名称更改为 `it knows you better`。
- 新增独立的工作统计页面。
- 工作统计支持自由选择开始日期和结束日期。
- 工作统计展示总计时长、记录任务数、日均时长和最高工作类型。
- 工作统计按工作类型展示实际计时时长占比，并提供环形图和横向占比条。
- 工作统计根据任务标题、项目、备注和标签生成关键词点云。
- 前端视觉风格调整为更克制的中性界面，并使用绿色、蓝色、金色、红色等功能色做区分。

## 产物

Release exe：
```text
D:\program\shiguang-list\src-tauri\target\release\it-knows-you-better.exe
```

便携试用包：
```text
D:\program\shiguang-list\release\it-knows-you-better-portable-0.2.0.zip
```

## 验证结果

- `npm.cmd run build`：通过。
- `cargo check --manifest-path src-tauri\Cargo.toml`：通过。
- `npm.cmd run tauri -- build --no-bundle`：通过。
- 便携包 exe 启动验证：进程保持运行。
