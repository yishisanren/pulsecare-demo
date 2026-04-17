---
title: "4.3 训练执行 - 停止确认"
path: "功能四 > 训练执行 > 停止确认"
---


## 训练停止确认弹窗

用户在训练过程中点击"Stop"按钮时的二次确认机制。

### 弹窗内容
**标题**："Stop Training?"
**描述**：根据当前进度显示不同文案

**进度 < 50%**
"You've completed less than 50% of this session. Are you sure you want to stop?"

**进度 ≥ 50%**
"You've made good progress! Are you sure you want to stop now?"

### 操作选项
**"Yes, Stop"** - 红色按钮
- 停止当前训练
- 记录实际训练时长和进度
- 进入训练完成激励页面

**"Continue"** - 主色调按钮
- 关闭弹窗
- 返回训练执行页面
- 保持训练暂停状态（如果之前是暂停的）

### 交互逻辑
- 弹窗背景模糊处理
- 点击弹窗外区域不关闭（避免误操作）
- 必须明确选择才能关闭弹窗
