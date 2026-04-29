---
title: "5.5 请假 - 连续≥3天提醒"
path: "功能五 > 训练日程管理 > 请假 > 连续请假提醒"
---


## 连续请假提醒（≥3 天时触发）

### 触发规则
- 每满 3 天触发一次（第 3、6、9 天...）
- 请假天数计算：当日**所有日程的所有任务**全部被请假，才计为 +1 天
- 即某个日程请假了但训练了其他日程 → 当天不算请假
- **双模式日程**：日程内 2 个任务必须**全部 Skip** 才视为"该日程当天已请假"；只 Skip 1 个则该日程未请假，当天不计入连续天数

### 弹窗文案
"You've taken a break for [N] days in a row. Consistency is key to making progress. Even one session today can help you get back on track."

### 按钮
- **"Let's train"** → 关闭提醒，进入当天训练
- **"I still need rest"** → 关闭提醒，进入正常请假确认弹窗

### 重置
完成一次训练后计数器归零
