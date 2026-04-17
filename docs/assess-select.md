---
title: "3.1 筛选与路由 (Screening & Routing)"
path: "功能三 > 问卷评估 > 筛选与路由"
---

## 3.1 筛选与路由 / Screening & Routing

用户进入评估后的第一步，通过 4 个筛选选项确定需要激活哪些问卷模块。
Users select from 4 screening options to determine which assessment modules to activate.

### 筛选选项（A/B/C/D） / Screening Options

| 选项 | 中文 | English | 触发模块 |
|------|------|---------|----------|
| A | 尿液不自主漏出 / 憋不住尿 / 在咳嗽、运动、用力时漏尿 | Involuntary urine leakage, difficulty holding urine, or urine leakage during coughing, exercise, or physical effort | 模块 1 · 尿失禁 (3IQ + ICIQ-SF + UDI-6 + IIQ-7) |
| B | 臀部或大腿存在疼痛或不适 | Pain or discomfort in the hips or thighs | 模块 2 · 臀腿疼痛 (Red-flag + NRS + Descriptor + Duration) |
| C | 臀部、大腿或下肢力量、稳定性或活动能力方面的问题 | Problems with strength, stability, or movement in the hips, thighs, or lower limbs | 模块 3 · 臀腿功能 (PGQ-25) |
| D | 以上都不是 — 希望进行一般盆底训练 | None of the above — I would like general pelvic floor training | 跳过评估 / Skip assessment |

### 交互逻辑 / Interaction Logic

- A/B/C 支持多选（复选框行为） / A/B/C support multi-select (checkbox behavior)
- D 与 A/B/C 互斥：选中 D 自动取消 A/B/C，选中任何 A/B/C 自动取消 D / D is mutually exclusive with A/B/C
- 选中 D 时按钮文案变为 "Skip Assessment"，点击跳转主页 / When D is selected, button becomes "Skip Assessment"
- 选中 A/B/C 任意组合时按钮文案为 "Start Assessment"，点击进入对应问卷 / When A/B/C selected, button becomes "Start Assessment"

### 路由映射 / Routing Map

| 选中组合 / Selection | 问卷流程 / Questionnaire Flow |
|----------|----------|
| A only | 3IQ → ICIQ-SF → UDI-6 → IIQ-7 |
| B only | Red-flag screening → NRS → Descriptor → Duration |
| C only | PGQ-25 |
| A+B | 尿失禁 → 疼痛 |
| A+C | 尿失禁 → 臀腿功能 |
| B+C | 疼痛 → 臀腿功能 |
| A+B+C | 尿失禁 → 疼痛 → 臀腿功能 |
| D | 跳过，直接进入模式选择 / Skip to mode selection |
