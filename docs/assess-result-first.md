---
title: "3.4 尿失禁评估结果·首次"
path: "功能三 > 问卷评估 > 尿失禁评估结果（首次）"
---

### 评估结果 · 尿失禁（首次） / Assessment Result · Urinary Incontinence (First)

> 本页规则以《电疗坐垫问卷输出逻辑》为唯一真值源，与 PRD 3.4 保持一致。
> This page aligns with the source-of-truth logic document and PRD 3.4.

---

### 第一步：定类型（3IQ × UDI-6 Q9/Q10） / Step 1 · Classification

主类型由 3IQ Q3 决定（Stress / Urge / Mixed / Other），次级特征由 UDI-6 Q9（Urgency，阈值 ≥2）与 Q10（Stress，阈值 ≥2）判定。四种主类型 × 四种次级组合 = **16 条分型文案**。

Primary type by 3IQ Q3; secondary features by UDI-6 Q9 (Urgency, threshold ≥2) and Q10 (Stress, threshold ≥2). 4 × 4 = **16 classification outputs**.

| 3IQ 主类型 | Q9 <2 / Q10 <2 | Q9 <2 / Q10 ≥2 | Q9 ≥2 / Q10 <2 | Q9 ≥2 / Q10 ≥2 |
|---|---|---|---|---|
| **Stress** | 主要为 Stress 漏尿<br/>Primarily stress incontinence. | 主要为 Stress 漏尿<br/>Primarily stress incontinence. | 主要为 Stress 漏尿，同时存在 Urgency 症状<br/>Primarily stress incontinence, with urgency symptoms. | 主要为 Stress 漏尿，同时存在 Urgency 与 Stress 症状<br/>Primarily stress incontinence, with both urgency and stress symptoms. |
| **Urge** | 主要为 Urge 漏尿<br/>Primarily urge incontinence. | 主要为 Urge 漏尿，同时存在 Stress 症状<br/>Primarily urge incontinence, with stress symptoms. | 主要为 Urge 漏尿<br/>Primarily urge incontinence. | 主要为 Urge 漏尿，同时存在 Urgency 与 Stress 症状<br/>Primarily urge incontinence, with both urgency and stress symptoms. |
| **Mixed** | 为 Mixed 漏尿，同时存在 Urgency 与 Stress 症状<br/>Mixed incontinence, with both urgency and stress symptoms. | 为 Mixed 漏尿，存在 Stress 症状<br/>Mixed incontinence, with stress symptoms. | 为 Mixed 漏尿，存在 Urgency 症状<br/>Mixed incontinence, with urgency symptoms. | 为 Mixed 漏尿，同时存在 Urgency 与 Stress 症状<br/>Mixed incontinence, with both urgency and stress symptoms. |
| **Other** | 非典型机制，需进一步评估<br/>Atypical pattern — further evaluation needed. | 非典型机制，需进一步评估<br/>Atypical pattern — further evaluation needed. | 非典型机制，需进一步评估<br/>Atypical pattern — further evaluation needed. | 非典型机制，需进一步评估<br/>Atypical pattern — further evaluation needed. |

---

### 第二步：定严重程度 + 训练频次 / Step 2 · Severity + Training Frequency

基于 **ICIQ-UI SF 总分 × UDI-6 标准化（≥33）× IIQ-7 总分（≥9.5）** 三维组合。

> UDI-6 阈值 33 指**标准化百分制**（= UDI-6 原始总分 × 100 / 18，范围 0–100）。
> IIQ-7 阈值 9.5 指原始总分（总分 0–21）。
> ICIQ-UI SF 总分为 Q4 + Q5 + Q6 三题之和（0–21）。

| ICIQ | UDI-6 | IIQ-7 | 严重程度 / Severity | 频次 × 周数 |
|---|---|---|---|---|
| 0–5 | <33 | <9.5 | 症状 slight，生活质量未受显著影响<br/>Slight symptoms; quality of life not significantly affected. | 2次/周 × 4周 |
| 6–12 | <33 | <9.5 | 症状 moderate，生活质量未受显著影响<br/>Moderate symptoms; quality of life not significantly affected. | 3次/周 × 6周 |
| 13–18 | <33 | <9.5 | 症状 severe，生活质量未受显著影响<br/>Severe symptoms; quality of life not significantly affected. | 4次/周 × 8周 |
| 19–21 | <33 | <9.5 | 症状 very severe，生活质量未受显著影响<br/>Very severe symptoms; quality of life not significantly affected. | 5次/周 × 10周 |
| 0–5 | ≥33 | <9.5 | 症状 moderate，生活质量未受显著影响<br/>Moderate symptoms; quality of life not significantly affected. | 3次/周 × 6周 |
| 6–12 | ≥33 | <9.5 | 症状 severe，生活质量未受显著影响<br/>Severe symptoms; quality of life not significantly affected. | 4次/周 × 8周 |
| 13–18 | ≥33 | <9.5 | 症状 very severe，生活质量未受显著影响<br/>Very severe symptoms; quality of life not significantly affected. | 5次/周 × 10周 |
| 19–21 | ≥33 | <9.5 | 症状 very severe，生活质量未受显著影响<br/>Very severe symptoms; quality of life not significantly affected. | 5次/周 × 10周 |
| 0–5 | <33 | ≥9.5 | 症状 slight，生活质量受影响<br/>Slight symptoms; quality of life affected. | 3次/周 × 5周 |
| 6–12 | <33 | ≥9.5 | 症状 moderate，生活质量受影响<br/>Moderate symptoms; quality of life affected. | 4次/周 × 7周 |
| 13–18 | <33 | ≥9.5 | 症状 severe，生活质量受影响<br/>Severe symptoms; quality of life affected. | 5次/周 × 9周 |
| 19–21 | <33 | ≥9.5 | 症状 very severe，生活质量受影响<br/>Very severe symptoms; quality of life affected. | 5次/周 × 12周 |
| 0–5 | ≥33 | ≥9.5 | 症状 moderate，生活质量受影响<br/>Moderate symptoms; quality of life affected. | 4次/周 × 7周 |
| 6–12 | ≥33 | ≥9.5 | 症状 severe，生活质量受影响<br/>Severe symptoms; quality of life affected. | 5次/周 × 9周 |
| 13–18 | ≥33 | ≥9.5 | 症状 very severe，生活质量受影响<br/>Very severe symptoms; quality of life affected. | 5次/周 × 12周 |
| 19–21 | ≥33 | ≥9.5 | 症状 very severe，生活质量受影响<br/>Very severe symptoms; quality of life affected. | 5次/周 × 12周 |

---

### 第三步：模式映射 / Step 3 · Mode Mapping

| 3IQ 主类型 | 推荐模式 / Recommended Mode |
|---|---|
| Stress（含 Stress+Urgency 次特征） | 08 SUI Mode · 08 压力性尿失禁模式 |
| Urge（含 Urgency 特征） | 09 UUI Mode · 09 急迫性尿失禁模式 |
| Mixed | 08 SUI Mode（主），同时存在 Urgency 时训练计划可并入 09 UUI Mode / 08 SUI Mode primary; 09 UUI Mode may be added when urgency coexists |
| Other | 不推荐模式，建议转诊 / Not recommended; refer to specialist |

---

### 页面结构 / Page Structure

1. 评估得分（大字百分比 + 原始分 ICIQ X/21 · UDI-6 标准化 · IIQ-7 X/21）
2. 分型结果卡片（第一步表格输出）
3. 严重程度卡片（第二步表格输出）
4. 推荐训练计划卡片（Mode 编号+中英名 · 频次/周 · 周数 · 总次数 = 频次 × 周数）
5. 免责声明
6. 底部按钮：`Customize Training Plan（定制训练计划）` / `Skip for Now（暂不制定）`

---

### 免责声明 / Disclaimer

**中文**：本评估及训练建议仅供个人健康管理参考，不构成医疗评估或医疗建议。个性化推荐基于您自行填写的问卷和使用数据，不代表临床改善证明。如症状持续、加重或出现异常，请及时咨询专业医疗人员。

**English**: This assessment and training recommendations are for personal wellness reference only. They do not constitute medical diagnosis or medical advice. Personalized suggestions are based on your self-reported data and do not represent clinical outcomes. If symptoms persist, worsen, or become unusual, please consult a qualified healthcare professional.
