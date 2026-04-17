---
title: "3.4 臀腿功能评估结果·非首次"
path: "功能三 > 问卷评估 > 臀腿功能评估结果（非首次）"
---

### 评估结果 · 臀腿功能（非首次） / Assessment Result · Hip-Leg Function (Follow-up)

> 本页规则以《电疗坐垫问卷输出逻辑》为唯一真值源，与 PRD 3.4 保持一致。
> 维度公式 / 分型文案 / 影响程度 / 训练频次 / 模式映射逻辑与首次评估完全相同，详见 `assess-result-hip-first.md`。

---

### 趋势图 / Trend Chart

- 始终展示，最多显示最近 7 次评估 / Always visible, shows up to 7 most recent assessments
- 纵轴为 PGQ%（0–100%） / Y-axis: PGQ%
- 横轴为评估次序 / X-axis: assessment index
- 1 次数据显示 1 个点 / A single data point if only one assessment exists

---

### 题目数说明 / Item Count

根据合规意见，删除原问题 Q19（Have a normal sex life），**共 24 题**。PGQ 有效满分 = 24 × 3 = **72**。

---

### 维度得分公式 / Dimension Scores

| 维度 | 求和题号 | 标准化公式 | 受限阈值 |
|---|---|---|---|
| Control 控制力 | Q1 + Q16 + Q17 + Q18 + Q20 + Q23（**6 道题**，Q19 已删除）| 实际总得分 / **18** | ≥ 0.3 |
| Endurance 耐力 | Q2 + Q3 + Q5 + Q6 + Q7 + Q8 + Q9 + Q10 + Q12 + Q14 + Q16 + Q24（**12 道题**）| 实际总得分 / **36** | ≥ 0.3 |
| Strength 力量 | Q4 + Q9 + Q10 + Q11 + Q12 + Q13 + Q14 + Q15 + Q16 + Q20（**10 道题**）| 实际总得分 / **30** | ≥ 0.3 |

---

### 分型文案（8 条）+ PGQ% 影响程度（4 档）

详见首次评估结果页：[`assess-result-hip-first.md`](./assess-result-hip-first.md)。非首次评估沿用相同规则。

See first-assessment page for the full 8-row classification + PGQ% impact table. Follow-up assessment uses the same rules.

---

### 模式映射 / Mode Mapping

| 组合 | 推荐模式 |
|---|---|
| C+E+S | 04 Function Mode |
| C+E | 01 Activation Mode + 03 Endurance Mode |
| C+S | 01 Activation Mode + 02 Strength Mode |
| C 单一 | 01 Activation Mode |
| E+S | 03 Endurance Mode + 02 Strength Mode |
| E 单一 | 03 Endurance Mode |
| S 单一 | 02 Strength Mode |
| 三维全 < 0.3 | 不推荐 |

---

### 页面结构 / Page Structure

1. 趋势图（PGQ% 单条曲线）
2. 评估得分（大字 PGQ% + PGQ 原始分 / 72）
3. 维度评估卡片（Control / Endurance / Strength）
4. 分型结果卡片
5. 影响程度卡片
6. 推荐训练计划卡片
7. 免责声明
8. 底部按钮：`Customize Training Plan` / `Skip for Now`

---

### 免责声明 / Disclaimer

**中文**：本评估及训练建议仅供个人健康管理参考，不构成医疗评估或医疗建议。个性化推荐基于您自行填写的问卷和使用数据，不代表临床改善证明。如症状持续、加重或出现异常，请及时咨询专业医疗人员。

**English**: This assessment and training recommendations are for personal wellness reference only. They do not constitute medical diagnosis or medical advice. Personalized suggestions are based on your self-reported data and do not represent clinical outcomes. If symptoms persist, worsen, or become unusual, please consult a qualified healthcare professional.
