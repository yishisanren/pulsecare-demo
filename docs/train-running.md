---
title: "4.3 训练进行中"
path: "训练执行 › 控制页 · 进行中"
---

## 训练进行中（控制页 · Running 态）

### 功能目的
训练任务执行中的核心交互页面。实时展示倒计时、当前强度、设备状态，并提供暂停 / 停止 / 强度调节能力。

### 触发时机
准备页点击 **Start** 后立即进入。

### 页面结构

| 区块 | 内容 | 说明 |
|---|---|---|
| 顶部导航 | `<` Training | 点击返回触发**停止确认弹窗** |
| 中央圆形进度环 | `19:59` + `Remaining Time` | 实时倒计时（精度到秒），外环动画 |
| 设备状态 | 🔋67% · 🔵 | 实时电量 + 蓝牙连接状态 |
| 状态文案 | `Running...` | 当前状态描述 |
| Mode 卡片 | `01 Activation · EMS · 24mins` ⓘ | 当前训练模式（不可修改） |
| Current Level | `−  1 / 100  +` | 实时强度（1–99 可调） |
| 底部按钮 | ⏹ Stop / ⏸ Pause | 黑色圆形按钮，左右排列 |

### 状态机（PRD §4.3 核心真值）

| 状态 | 显示按钮 | 关键规则 |
|---|---|---|
| **训练中** | Pause + Stop | 用户可随时调节 1–99；**强度调回 0 时自动进入暂停**（等同于点击 Pause） |
| **已暂停** | Resume + Stop | 暂停时强度显示为 0；Resume 前先判断电极连接，**正常则强度恢复到暂停前的值**，异常则弹电极异常提示 |

### 强度调节规则
- **范围**：1–99，每次点击 ± 1
- **下限触发**：调到 0 = 自动暂停（Pause）
- **上限**：99，达到上限不再 +
- **响应延迟**：调节实时生效，无确认步骤

### Stop 按钮（停止确认弹窗，PRD §4.3）

| 进度 | 标题 | 文案 | 按钮 |
|---|---|---|---|
| **<50%** | Session Too Short | "You have only completed X% of this session. Sessions under 50% will not be saved. Are you sure you want to stop?" | Keep Going（主）/ End Session（次） |
| **≥50%** | End Session Early? | "You have completed X% of this session. Your progress will be saved. Are you sure you want to end early?" | Continue Training（主）/ End Session（次） |

### Pause 按钮
- 强度立刻显示为 0，计时停止
- 按钮变为 **Resume + Stop**
- Resume 前自动检测电极连接：正常 → 强度恢复到暂停前值；异常 → 弹**电极片异常**提示

### 异常处理（PRD §4.4）

| 场景 | 行为 |
|---|---|
| **蓝牙断联** | 弹窗 `Connection Lost` → 数据保存在设备端，下次连接自动上报 |
| **坐姿异常** | 弹窗 `Posture Alert` + 训练自动暂停 → 用户调整后 Resume 继续 |
| **电极片异常** | 弹窗 `Electrode Connection Issue` → Retry / End Session |

### 累计使用提醒（PRD §4.5）
- 当日累计训练时长 ≥60 分钟时，下次点击 Start 触发提醒（非强制）
- 提醒展示当日累计（如 `62 min`）+ `Take a Break` / `Continue Anyway`
- 中间休息 ≤5 分钟按连续计算；>5 分钟则重新开始计时；次日 00:00 重置

### 倒计时归零行为
计时器到 0 → 自动跳转 **训练完成 · 100%** 页面（不需要用户手动操作）。

### 双模式当天衔接（PRD v1.4）
当天双模式日程下，完成第 1 个任务（如 08 SUI 20min）→ 跳转完成页 → 用户点击 Continue 回到日程主页 → 看到第 2 个任务卡（09 UUI 20min）→ 点击进入第 2 次训练准备页。
