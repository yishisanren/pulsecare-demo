---
title: "4.3.5 异常处理 - 蓝牙断联"
path: "功能四 > 训练执行 > 异常处理 > 蓝牙断联"
---


## 场景一：蓝牙断联（Bluetooth Disconnection）

### 触发条件
训练过程中蓝牙连接中断

### 弹窗内容
- **标题**："Connection Lost"
- **文案**："Bluetooth connection has been lost. Your training data is saved on the device and will sync automatically when reconnected."
- **按钮**：「OK」→ 关闭弹窗，返回设备主页

### 数据处理
- 训练数据保存在设备端
- 下次蓝牙连接后自动上报到 App
- 已完成的训练时长记录在训练记录中
