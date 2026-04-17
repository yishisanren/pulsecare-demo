---
title: "4.3.5 异常处理 - 电极片异常"
path: "功能四 > 训练执行 > 异常处理 > 电极片连接异常"
---


## 场景三：电极片连接异常（Electrode Issue）

### 触发条件
设备检测到电极片未正确贴合或脱落

### 弹窗内容
- **标题**："Electrode Connection Issue"
- **文案**："The electrode pads are not properly connected. Please check that the pads are firmly attached and try again."
- **按钮 1**：「Retry」→ 重新检测电极连接
- **按钮 2**：「End Session」→ 结束训练，进入训练完成页

### 交互逻辑
- 训练自动暂停
- 用户重新贴合电极片后点击 Retry
- 检测通过 → 恢复训练（强度恢复为暂停前的值）
- 检测未通过 → 弹窗保持，用户可再次 Retry 或选择结束
