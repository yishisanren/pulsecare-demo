---
title: "3.4 疼痛评估结果·风险项"
path: "功能三 > 问卷评估 > 疼痛评估结果（风险项）"
---

### 评估结果 · 臀腿疼痛（风险项） / Assessment Result · Hip-Leg Pain (Safety Gate)

---

### 触发条件 / Trigger

Q1 选了任一风险项（前 5 项）/ Q1 selected any risk item (first 5)

### Q1 选项清单 / Q1 Options

**题干 / Question**：
- 中文：过去一周，您是否出现以下情况？（多选）
- English: In the past week, have you experienced any of the following? (Multiple choice)

| 选项 | 中文 | English | 触发安全门控 |
|---|---|---|---|
| 1 | 发热 | Fever | ✓ |
| 2 | 伤口处红肿加剧 | Increasing redness or swelling at wound site | ✓ |
| 3 | 恶臭分泌物 | Foul-smelling discharge | ✓ |
| 4 | 单侧腿部突然严重肿胀 | Sudden severe swelling in one leg | ✓ |
| 5 | 麻木或大小便失禁 | Numbness or loss of control of bladder or bowel | ✓ |
| 6 | 无（继续评估） | None | — |

### 输出文案 / Output Copy

| 中文 | English |
|------|---------|
| ⚠️ 请先咨询专业医生后再使用本设备。 | ⚠️ Please contact a healthcare professional before using the device. |

### 规则 / Rule

- 不进入后续评估题（安全门控直接跳出）/ Skip remaining assessment questions
- 不显示 NRS 得分、分型、严重程度 / NRS score, classification, severity hidden
- 不推荐任何训练模式 / No training mode recommended

---

### 免责声明 / Disclaimer

**中文**：本评估及训练建议仅供个人健康管理参考，不构成医疗评估或医疗建议。个性化推荐基于您自行填写的问卷和使用数据，不代表临床改善证明。如症状持续、加重或出现异常，请及时咨询专业医疗人员。

**English**: This assessment and training recommendations are for personal wellness reference only. They do not constitute medical evaluation or medical advice. Personalized suggestions are based on your self-reported data and do not represent clinical outcomes. If symptoms persist, worsen, or become unusual, please consult a qualified healthcare professional.
