---
title: "4.3.6 累计使用提醒"
path: "功能四 > 训练执行 > Rest Reminder"
---


## 累计使用提醒（Rest Reminder）

### 触发条件
- 当日累计训练时长 ≥ 60 分钟时触发
- 累计计时规则：中间休息 ≤ 5 分钟按连续计算，> 5 分钟重新计时
- 触发时机：用户点击「Start」开始新一次训练时检测

### 弹窗内容
- **标题**："Time for a Break"
- **描述**："You have been training for over 60 minutes today. We recommend taking a rest to avoid muscle fatigue. You can continue if you feel comfortable."
- **累计时长展示**：显示当日总训练时长（如 62 min）

### 操作按钮
- **"Take a Break"**（主按钮）→ 关闭弹窗，返回日程主页
- **"Continue Anyway"**（次按钮）→ 关闭弹窗，正常开始训练

### 规则
- **非强制性**：用户可选择继续训练
- **每日仅提醒一次**：选择 Continue Anyway 后当日不再弹出
- **次日重置**：00:00 重置累计时长
- **全模式累计**：所有训练模式的时间都计入
