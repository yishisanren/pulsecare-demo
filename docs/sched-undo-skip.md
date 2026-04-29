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

### <span class="v14-add">双模式日程的任务粒度撤销</span>
<span class="v14-add">撤销按单任务粒度处理：</span>
- <span class="v14-add">撤销双模式中已 Skip 的 1 个任务，**不影响另 1 个任务**的状态（仍可独立 Skip 或完成）</span>
- <span class="v14-add">连续请假计数器仅在"该日程当天 2 任务原本全部被 Skip"才会 -1（撤销 1 个后该日程当天不再算请假）</span>
