---
title: "5.5 撤销请假弹窗"
path: "功能五 > 训练日程管理 > 请假 > 撤销请假"
---


## 撤销请假弹窗

### 触发方式
点击日程主页中标记为 **Skipped** 的任务卡片

### 弹窗内容
- 标题："Undo skip?"
- 说明："This session will be restored to your schedule."
- 「Restore Session」→ 任务恢复 Pending 状态
- 「Cancel」→ 关闭弹窗

### 撤销时限

| 场景 | 时限 |
|------|------|
| 当天请假 | 当天 00:00 前可撤销 |
| 未来日期请假 | 该日期到来前可撤销 |
| 已过期日期 | 不可撤销 |

### 撤销后处理
- 任务恢复 Pending 状态
- 连续请假计数器 -1
- 日历标记恢复
- Toast 提示："Training restored"
