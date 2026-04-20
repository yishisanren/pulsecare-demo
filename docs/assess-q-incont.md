---
title: "3.2 尿失禁问卷 (3IQ + ICIQ-UI SF + UDI-6 + IIQ-7)"
path: "功能三 > 问卷评估 > 尿失禁问卷"
---


## 3.2 尿失禁问卷

分为四个子量表：3IQ 分型筛查 → ICIQ-UI SF 严重度 → 情境多选 → UDI-6 主观严重度 → IIQ-7 生活质量影响。共 16 题（含跨子量表重编号）。

### 阶段一：3IQ（3 Incontinence Questions）分型

| 题号 | 问题题干 | 题型 | 选项 | 路由逻辑 |
|------|------|------|------|----------|
| Q1 | During the last 3 months, have you leaked urine (even a small amount)? | 单选 | yes / no | no → 跳转：模块1问卷结束 |
| Q2 | During the last 3 months, did you leak urine: (check all that apply.) | 多选 | a. When you were perfoming some physical activity, such as coughing, sneezing, lifting, or exercise?<br>b. When you had the urge or the feeling that you needed to empty your bladder, but you could not get to the toilet fast enough?<br>c. Without physical activity and without a sense of urgency? | 描述统计，不计分 |
| Q3 | During the last 3 months, did you leak urine most often: (check only one.) | 单选 | a. When you were performing some physical activitiy, such as coughing, sneezing, lifting, or exercise?<br>b. When you had the urge or the feeling that you needed to empty your bladder, but you could not get to the toilet fast enough?<br>c. Without physical activity and without a sense of urgency?<br>d. About equally as often with physical activity as with a sense of urgency? | 按选项决定分型：a—stress / b—urge / c—other（跳转结束）/ d—mixed |

### 阶段二：ICIQ-UI SF 严重度（Q4–Q6）

| 题号 | 问题题干 | 题型 | 选项 | 计分 |
|------|------|------|------|------|
| Q4 | How often do you leak urine? | 单选 | Never<br>About once a week or less often<br>2–3 times a week <br>About once a day <br>Several times a day<br>All The time | 0 / 1 / 2 / 3 / 4 / 5 |
| Q5 | How much urine do you usually leak? | 单选 | None<br>A small amount<br>A moderate amount<br>A large amount | 0 / 2 / 4 / 6 |
| Q6 | Overall, how much does leaking urine interfere with your everyday life? (Please circle a number between 0 and 10) | 11 分量表 | Not at all【 0 —— 1 —— 2 —— 3 —— 4 —— 5 —— 6 —— 7 —— 8 —— 9 —— 10 】A great deal | 0–10 |

**ICIQ-UI SF 总分范围**：0–21。临床分级：slight (0–5) / moderate (6–12) / severe (13–18) / very severe (19–21)

### 阶段三：情境多选（Q7）

| 题号 | 问题题干 | 题型 | 选项 |
|------|------|------|------|
| Q7 | When does urine leakage occur?<br>(You may select all that apply) | 多选 | Never<br>Before reaching the toilet<br>When coughing or sneezing<br>When physically active/exercising<br>After finishing urination and dressing<br>During sleep<br>For no obvious reason<br>All the time |

描述统计，不计分。

### 阶段四：UDI-6 主观严重程度（Q8–Q13）

**引导语**：Over the past month, how much have the following symptoms bothered you?
**选项（4 级量表，每题相同）**：0 = Not at all； 1 = A little bit； 2 = Moderately； 3 = Greatly

| 题号 | 问题题干 |
|------|------|
| Q8 | Frequent urination? |
| Q9 | Urine leakage related to a feeling of urgency?（**Urgency 阈值题**，≥2 标记 urgency-feature） |
| Q10 | Urine leakage related to physical activity, coughing, or sneezing?（**Stress 阈值题**，≥2 标记 stress-feature） |
| Q11 | Small amounts of urine leakage (drops)? |
| Q12 | Difficulty emptying your bladder? |
| Q13 | Pain or discomfort in the lower abdominal, pelvic, or genital area? |

**计分**：初始总分 0–18 → 标准化百分制 = 初始分 × 100 / 18。
**分级**：0–24 minimal / 25–32 mild / 33–49 moderate / 50–74 moderate-severe / ≥75 severe（临界点 33.3）

### 阶段五：IIQ-7 生活质量影响（Q10–Q16，沿用 Excel 题号）

**引导语**：How much does urine leakage affect the following activities or feelings?
**选项（4 级量表，每题相同）**：0 = Not at all； 1 = Slightly； 2 = Moderately； 3 = Greatly

| 题号 | 问题题干 |
|------|------|
| Q10 | Household chores (e.g., cleaning, shopping)? |
| Q11 | Physical recreation (e.g., walking, exercise)? |
| Q12 | Entertainment activities (e.g., movies, concerts)? |
| Q13 | Ability to travel more than 30 minutes from home? |
| Q14 | Social activities outside the home? |
| Q15 | Emotional health (nervousness, frustration, embarrassment)? |
| Q16 | Feeling frustrated or limited by urine leakage? |

**计分**：初始总分 0–21。IIQ-7 总分 ≥ 9.5 可视为存在显著生活质量影响。

---

### 计算逻辑总览 / Calculation Summary

- **分型（16 条文案）**：3IQ 主类型（Stress/Urge/Mixed/Other）× UDI-6 Q9 (≥2 / <2) × UDI-6 Q10 (≥2 / <2) → 16 条尿失禁类型输出文案
- **严重程度 + 训练频次（16 行）**：ICIQ 区间（0-5 / 6-12 / 13-18 / 19-21）× UDI-6 标准化（<33 / ≥33）× IIQ-7（<9.5 / ≥9.5）→ 16 条严重程度 + 训练频次组合
- **UDI-6 修正规则**：UDI-6 标准化 ≥33 → 严重度在 ICIQ 基础上升一级（最多升到 very severe）；<33 → 与 ICIQ 一致
- **模式映射**：
  - Stress → `08 SUI Mode`
  - Urge → `09 UUI Mode`
  - Mixed → `08 SUI Mode`（主），同时存在 Urgency 时训练计划可并入 `09 UUI Mode`
  - Other → 不推荐模式，建议转诊

---

> 题干与选项文案严格依据《问卷评估需求 20260129》Excel「模块 1：尿失禁+盆底肌」原文。详细分型映射、模式推荐、训练频次等结果计算见 PRD 3.4 模块 1（`assess-result-first.md`）。
