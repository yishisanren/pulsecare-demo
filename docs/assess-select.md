---
title: "3.1 筛选与路由 (Screening & Routing)"
path: "功能三 > 问卷评估 > 筛选与路由"
---


## 3.1 筛选与路由

用户进入评估后的第一步，通过4个筛选选项确定需要激活哪些问卷模块。

### 筛选选项（A/B/C/D）

| 选项 | 文案 | 触发模块 |
|------|------|----------|
| A | "I experience involuntary urine leakage during daily activities, exercise, coughing, or sneezing" | 尿失禁模块 (3IQ + ICIQ-SF) |
| B | "I have persistent or recurring pain in the pelvic region, lower back, or hip area" | 疼痛模块 (NRS + 红旗筛查) |
| C | "I feel heaviness, pressure, or a bulging sensation in the vaginal or pelvic area" | 脱垂模块 (POP-SS) |
| D | "None of the above — I would like general pelvic floor training" | 跳过评估 |

### 交互逻辑
- A/B/C 支持多选（复选框行为）
- D 与 A/B/C 互斥：选中 D 自动取消 A/B/C，选中任何 A/B/C 自动取消 D
- 选中 D 时按钮文案变为 "Skip Assessment"，点击跳转主页
- 选中 A/B/C 任意组合时按钮文案为 "Start Assessment"，点击进入对应问卷

### 路由映射
| 选中组合 | 问卷流程 |
|----------|----------|
| A only | 3IQ → ICIQ-SF |
| B only | Red-flag screening → Pain NRS |
| A+B | 3IQ → ICIQ-SF → Red-flag → Pain NRS |
| A+B+C | 3IQ → ICIQ-SF → Red-flag → Pain NRS → POP-SS |
| D | 跳过，直接进入模式选择 |
