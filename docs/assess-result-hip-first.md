---
title: "3.4 臀腿功能评估结果·首次"
path: "功能三 > 问卷评估 > 臀腿功能评估结果（首次）"
---

### 评估结果 · 臀腿功能（首次） / Assessment Result · Hip-Leg Function (First)

> 本页规则以《电疗坐垫问卷输出逻辑》为唯一真值源，与 PRD 3.4 保持一致。

---

### 题目数说明 / Item Count

根据合规意见，删除原问题 Q19（Have a normal sex life），**共 24 题**。
Per compliance guidance, Q19 (Have a normal sex life) is removed; **24 items total**.

PGQ 有效满分 = 24 × 3 = **72**

---

### 第一步：算三个维度得分 / Step 1 · Dimension Scores

| 维度 | 求和题号 | 标准化公式 | 受限阈值 |
|---|---|---|---|
| Control 控制力 | Q1 + Q16 + Q17 + Q18 + Q20 + Q23（共 **6 道题**，Q19 已删除）| 实际总得分 / **18** | ≥ 0.3 判定为受限 |
| Endurance 耐力 | Q2 + Q3 + Q5 + Q6 + Q7 + Q8 + Q9 + Q10 + Q12 + Q14 + Q16 + Q24（共 **12 道题**）| 实际总得分 / **36** | ≥ 0.3 判定为受限 |
| Strength 力量 | Q4 + Q9 + Q10 + Q11 + Q12 + Q13 + Q14 + Q15 + Q16 + Q20（共 **10 道题**）| 实际总得分 / **30** | ≥ 0.3 判定为受限 |

> NA 题目从分子分母同时去掉 / NA items removed from both numerator and denominator.
> 题号沿用 PGQ-25 原编号。Q19 删除后，Control 分母由 21 → **18**（B2 规则）。

---

### 第二步：按三维度组合定分型文案与推荐模式 / Step 2 · Classification (8 rows)

| 序号 | C | E | S | 特征 | 类型输出文案（中文） | Type Output (EN) | 映射设备模式 |
|---|---|---|---|---|---|---|---|
| 1 | ≥ 0.3 | ≥ 0.3 | ≥ 0.3 | Control/Endurance/Strength | 您的下肢在控制、耐力和力量方面有**明显受限**，建议针对性训练。 | Your lower limbs show clear limitations in control, endurance, and strength. Targeted training is recommended. | 04 Function Mode · 04 功能模式 |
| 2 | ≥ 0.3 | ≥ 0.3 | < 0.3 | Control/Endurance | 您的下肢在控制和耐力方面有**一定受限**，建议进行相关训练。 | Your lower limbs show some limitation in control and endurance. Related training is recommended. | 01 Activation Mode + 03 Endurance Mode |
| 3 | ≥ 0.3 | < 0.3 | ≥ 0.3 | Control/Strength | 您的下肢在控制和力量方面有**一定受限**，建议进行相关训练。 | Your lower limbs show some limitation in control and strength. Related training is recommended. | 01 Activation Mode + 02 Strength Mode |
| 4 | ≥ 0.3 | < 0.3 | < 0.3 | Control | 您的下肢在控制方面有**轻度受限**，建议激活训练。 | Your lower limbs show mild limitation in control. Activation training is recommended. | 01 Activation Mode · 01 激活模式 |
| 5 | < 0.3 | ≥ 0.3 | ≥ 0.3 | Endurance/Strength | 您的下肢在耐力和力量方面有**一定受限**，建议进行针对性训练。 | Your lower limbs show some limitation in endurance and strength. Targeted training is recommended. | 03 Endurance Mode + 02 Strength Mode |
| 6 | < 0.3 | ≥ 0.3 | < 0.3 | Endurance | 您的下肢在耐力方面有**轻度受限**，建议耐力训练。 | Your lower limbs show mild limitation in endurance. Endurance training is recommended. | 03 Endurance Mode · 03 耐力模式 |
| 7 | < 0.3 | < 0.3 | ≥ 0.3 | Strength | 您的下肢在力量方面有**轻度受限**，建议力量训练。 | Your lower limbs show mild limitation in strength. Strength training is recommended. | 02 Strength Mode · 02 力量模式 |
| 8 | < 0.3 | < 0.3 | < 0.3 | — | 您的下肢功能良好，无明显受限。 | Your lower-limb function is good, with no significant limitations. | 不推荐 / Not recommended |

> 措辞分档规则：序号 1 = "明显受限"；序号 2/3/5 = "一定受限"；序号 4/6/7 = "轻度受限"；序号 8 = 功能良好。

---

### 第三步：定影响程度 + 训练频次（PGQ 百分比） / Step 3 · Impact + Frequency

**PGQ% = 实际总分 ÷ 72 × 100%**

| PGQ% | 影响程度文案（中文） | Output Message (EN) | 训练频次 | 周数 |
|---|---|---|---|---|
| 0–20% | 很小影响 / 基本无功能受限 | Minimal impact / essentially no functional limitation | 不推荐 | — |
| 20–40% | 轻度影响 | Mild impact | 3 次/周 | 2 周 |
| 40–60% | 中度功能受限 | Moderate functional limitation | 4 次/周 | 3 周 |
| >60% | 重度影响，临床显著功能受限 | Severe impact; clinically significant functional limitation | 5 次/周 | 5 周 |

---

### 页面结构 / Page Structure

1. 评估得分（大字 PGQ% + PGQ 原始分 / 72）
2. 维度评估卡片（Control / Endurance / Strength 三条进度条 + 数值 + "受限/良好"标签）
3. 分型结果卡片（第二步 8 条中选中的 1 条输出文案）
4. 影响程度卡片（第三步 PGQ% 档位文案）
5. 推荐训练计划卡片（Mode 编号+中英名 · EMS · 单次时长 · 频次/周 · 周数 · 总次数）
6. 免责声明
7. 底部按钮：`Customize Training Plan` / `Skip for Now`

---

### 免责声明 / Disclaimer

**中文**：本评估及训练建议仅供个人健康管理参考，不构成医疗评估或医疗建议。个性化推荐基于您自行填写的问卷和使用数据，不代表临床改善证明。如症状持续、加重或出现异常，请及时咨询专业医疗人员。

**English**: This assessment and training recommendations are for personal wellness reference only. They do not constitute medical diagnosis or medical advice. Personalized suggestions are based on your self-reported data and do not represent clinical outcomes. If symptoms persist, worsen, or become unusual, please consult a qualified healthcare professional.
