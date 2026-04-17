---
title: "4.3.5 异常处理 - 坐姿异常"
path: "功能四 > 训练执行 > 异常处理 > 坐姿异常"
---


## 场景二：坐姿异常（Posture Alert）

### 触发条件
设备检测到用户坐姿偏移，电极片接触面积不足

### 弹窗内容
- **标题**："Posture Alert"
- **文案**："Incorrect sitting posture detected. Please adjust your position to ensure the electrode pads are in full contact for the best results."
- **按钮**：「Got It」→ 关闭弹窗

### 交互逻辑
- 弹窗出现时，训练**自动暂停**
- 用户调整坐姿后，点击 Resume 继续训练
- 强度恢复为暂停前的值
