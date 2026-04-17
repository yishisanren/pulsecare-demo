---
title: "3.2 尿失禁问卷 (3IQ + ICIQ-UI SF + UDI-6 + IIQ-7)"
path: "功能三 > 问卷评估 > 尿失禁问卷"
---


## 3.2 尿失禁问卷（共 20 题）

> 与 PRD 3.3 模块 1 保持一致。由 4 个部分组成：3IQ 分型 → ICIQ-UI SF 客观评分区间 → UDI-6 主观评分区间 → IIQ-7 生活质量影响。

---

### Part 1：3IQ 分型（Q1-Q3）— 确定尿失禁类型

| 题号 | 问题 / Question | 类型 | 选项 / Options | 规则 |
|---|---|---|---|---|
| Q1 | During the last 3 months, have you leaked urine (even a small amount)? | 单选 | Yes / No | No → 跳过整个模块 1 |
| Q2 | Did you leak urine: (check all that apply) | 多选 | a. physical activity / b. urge / c. without both | 仅记录，不计分 |
| Q3 | Did you leak urine most often: | 单选 | a. physical activity → **Stress** / b. urge → **Urge** / c. without both → **Other** / d. equally → **Mixed** | **决定主类型** |

---

### Part 2：ICIQ-UI SF（Q4-Q7）— 客观评分区间

| 题号 | 问题 | 选项 | 计分 |
|---|---|---|---|
| Q4 | How often do you leak urine? | Never(0) / Once a week(1) / 2-3 times(2) / Once a day(3) / Several times(4) / All the time(5) | 0-5 |
| Q5 | How much urine do you usually leak? | None(0) / Small(2) / Moderate(4) / Large(6) | 0-6 |
| Q6 | How much does leaking interfere with your life? | 滑块 0-10，Not at all(0) — A great deal(10) | 0-10 |
| Q7 | When does urine leakage occur? | 多选：Never / Before reaching toilet / Coughing or sneezing / Physically active / After finishing urination / During sleep / No obvious reason / All the time | 仅记录 |

**ICIQ 总分** = Q4 + Q5 + Q6，范围 **0–21**

---

### Part 3：UDI-6（Q8-Q13）— 主观评分区间

"Over the past month, how much have the following symptoms bothered you?"
选项与计分：Not at all = 0 / A little bit = 1 / Moderately = 2 / Greatly = 3

| 题号 | 问题 |
|---|---|
| Q8 | Frequent urination? |
| Q9 | Urine leakage related to a feeling of urgency?（Urgency 阈值题，≥2 表示次级 Urgency 特征）|
| Q10 | Urine leakage related to physical activity, coughing, or sneezing?（Stress 阈值题，≥2 表示次级 Stress 特征）|
| Q11 | Small amounts of urine leakage (drops)? |
| Q12 | Difficulty emptying your bladder? |
| Q13 | Pain or discomfort in the lower abdominal, pelvic, or genital area? |

**UDI-6 原始总分** = 0–18
**标准化百分制** = 原始总分 × 100 / 18，范围 **0–100**
**阈值**：标准化 ≥ 33 视为 UDI-6 高值

---

### Part 4：IIQ-7（Q14-Q20）— 生活质量影响

"How much does urine leakage affect the following?"
选项与计分：Not at all = 0 / Slightly = 1 / Moderately = 2 / Greatly = 3

| 题号 | 问题 |
|---|---|
| Q14 | Household chores (e.g., cleaning, shopping)? |
| Q15 | Physical recreation (e.g., walking, exercise)? |
| Q16 | Entertainment activities (e.g., movies, concerts)? |
| Q17 | Ability to travel more than 30 minutes from home? |
| Q18 | Social activities outside the home? |
| Q19 | Emotional health (nervousness, frustration, embarrassment)? |
| Q20 | Feeling frustrated or limited by urine leakage? |

**IIQ-7 总分** = 0–21
**阈值**：≥ 9.5 视为 QoL 受影响

---

### 计算逻辑总览 / Calculation Summary

- **分型（16 条）**：3IQ 结果（Stress/Urge/Mixed/Other）× UDI-6 Q9 ≥2 × UDI-6 Q10 ≥2 → 16 条分型文案
- **严重程度 + 训练频次（16 行）**：ICIQ 区间（0-5 / 6-12 / 13-18 / 19-21）× UDI-6 标准化（<33 / ≥33）× IIQ-7（<9.5 / ≥9.5）→ 16 条严重程度 + 训练频次
- **模式映射**：
  - Stress → `08 SUI Mode`
  - Urge → `09 UUI Mode`
  - Mixed → `08 SUI Mode`（主），同时存在 Urgency 时训练计划可并入 `09 UUI Mode`
  - Other → 不推荐模式，建议转诊

详见 PRD 3.4 模块 1 结果计算（`assess-result-first.md`）。
