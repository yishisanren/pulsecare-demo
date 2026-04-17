---
title: "3.4 疼痛评估结果·首次"
path: "功能三 > 问卷评估 > 疼痛评估结果（首次）"
---

### 评估结果 · 臀腿疼痛（首次） / Assessment Result · Hip-Leg Pain (First)

> 本页规则以《电疗坐垫问卷输出逻辑》为唯一真值源，与 PRD 3.4 保持一致。

---

### 第一步：定疼痛模式（Q2 描述词聚合 → Acute / Chronic） / Step 1 · Pain Mode

| Q2 描述词判定类型 / Type | 中文 | 映射设备模式 / Device Mode |
|---|---|---|
| Acute / Muscle-related | 急性 / 肌肉相关 | 07 Acute Mode · 07 急性疼痛模式 |
| Acute nociceptive | 急性 伤害感受性 | 07 Acute Mode · 07 急性疼痛模式 |
| Chronic nociceptive | 慢性 伤害感受性 | 06 Chronic Mode · 06 慢性疼痛模式 |
| Chronic neuropathic-like / Chronic neuropathic | 慢性类神经病理性 / 慢性神经病理性 | 06 Chronic Mode · 06 慢性疼痛模式 |
| Mixed Acute + Chronic | 混合型（急性+慢性） | 06 Chronic Mode（日常）+ 07 Acute Mode（发作时）|

---

### 第二步：定类型文案（Q2 × Q3 持续时间） / Step 2 · Classification (15 rows)

基于 Q2 判定类型（5 类）× Q3 持续时间（<1 周 / 1–6 周 / >6 周），输出 **15 条分型文案 + 15 条模式方案文案**。

Based on Q2 type (5) × Q3 duration (3), **15 classification + 15 mode-plan outputs**.

| Q2 判定类型 | Q3 | 疼痛类型文案（中文） | Type Output (EN) | 模式方案文案（中文） | Mode Plan Output (EN) |
|---|---|---|---|---|---|
| Acute / Muscle-related | <1 week | 短期肌肉痉挛或收缩性疼痛。常见于产后早期恢复阶段。 | Short-term muscle spasm or contractile pain. Common in the early postpartum recovery phase. | 使用 07 Acute Mode 缓解短期痉挛痛，可配合轻柔活动。 | Use "07 Acute Mode" to relieve short-term spasm pain, paired with gentle activity. |
| Acute / Muscle-related | 1–6 weeks | 持续肌肉痉挛或收缩性疼痛。产后恢复中，短期疼痛可能反复出现。 | Persistent muscle spasm or contractile pain. Short-term pain may recur during postpartum recovery. | 继续 07 Acute Mode 缓解疼痛，注意休息和轻度拉伸。 | Continue "07 Acute Mode" to relieve pain; rest and do light stretching. |
| Acute / Muscle-related | >6 weeks | 持续急性肌肉痛。超过 6 周仍存在，可能提示慢性或复发风险。 | Persistent acute muscle pain. Symptoms lasting more than 6 weeks may indicate chronic risk or recurrence. | 使用 07 Acute Mode 缓解，同时建议咨询医生。 | Use "07 Acute Mode" for relief; also consult a clinician. |
| Acute nociceptive | <1 week | 锐痛、刺痛，多与活动或组织拉伤相关。产后早期出现。 | Sharp, stabbing pain, often associated with activity or tissue strain. Appears in the early postpartum period. | 使用 07 Acute Mode 缓解，减少疼痛诱因动作。 | Use "07 Acute Mode" for relief; reduce pain-triggering movements. |
| Acute nociceptive | 1–6 weeks | 活动相关的锐痛或刺痛。产后 1–6 周仍可能出现。 | Activity-related sharp or stabbing pain. May persist 1–6 weeks postpartum. | 继续 07 Acute Mode 缓解，配合日常恢复训练。 | Continue "07 Acute Mode" for relief, combined with daily recovery exercises. |
| Acute nociceptive | >6 weeks | 锐痛持续存在。超过 6 周仍有急性疼痛，可能伴慢性机制。 | Sharp pain persists. Acute pain lasting over 6 weeks may involve a chronic component. | 使用 07 Acute Mode 缓解，同时建议专业评估。 | Use "07 Acute Mode" for relief; seek professional evaluation. |
| Chronic nociceptive | <1 week | 初期出现持续钝痛或酸痛。产后早期即可出现慢性痛征兆。 | Early persistent dull or aching pain. Signs of chronic pain can appear even in the early postpartum period. | 尝试 06 Chronic Mode 日常缓解，注意活动规律。 | Try "06 Chronic Mode" for daily relief; keep activity regular. |
| Chronic nociceptive | 1–6 weeks | 持续酸痛或钝痛，伴日常活动干扰。产后恢复中期常见。 | Persistent aching or dull pain that interferes with daily activities. Common in mid-postpartum recovery. | 使用 06 Chronic Mode 缓解日常不适，结合轻度锻炼。 | Use "06 Chronic Mode" for daily relief combined with light exercise. |
| Chronic nociceptive | >6 weeks | 长期钝痛或酸痛。产后超过 6 周仍存在慢性疼痛。 | Long-term dull or aching pain. Chronic pain persists beyond 6 weeks postpartum. | 建议 06 Chronic Mode 日常缓解，并可咨询康复专业人员。 | Recommend "06 Chronic Mode" for daily relief; consider consulting a rehab specialist. |
| Chronic neuropathic-like / Chronic neuropathic | <1 week | 早期神经性疼痛（灼热、刺痛、麻木）。产后刚出现时需关注疼痛发展。 | Early neuropathic pain (burning, tingling, numbness). Monitor closely when it first appears postpartum. | 使用 06 Chronic Mode 缓解，同时观察症状变化。 | Use "06 Chronic Mode" for relief; monitor symptom changes. |
| Chronic neuropathic-like / Chronic neuropathic | 1–6 weeks | 持续神经性疼痛（烧灼感、针刺感、麻木）。产后中期慢性疼痛常见。 | Persistent neuropathic pain (burning, pins-and-needles, numbness). Common in mid-postpartum chronic pain. | 使用 06 Chronic Mode 日常缓解疼痛，注意避免加重因素。 | Use "06 Chronic Mode" for daily pain relief; avoid aggravating factors. |
| Chronic neuropathic-like / Chronic neuropathic | >6 weeks | 长期神经性疼痛（灼热、刺痛、麻木、轻触痛）。超过 6 周持续存在，提示慢性机制主导。 | Long-term neuropathic pain (burning, tingling, numbness, allodynia). Persistence beyond 6 weeks suggests a chronic mechanism dominates. | 建议 06 Chronic Mode 日常使用，并咨询专业康复或医生评估。 | Recommend daily "06 Chronic Mode"; consult a rehab specialist or clinician for evaluation. |
| Mixed Acute + Chronic | <1 week | 同时存在急性痉挛/刺痛和持续背景痛。产后早期即可出现混合疼痛。 | Both acute spasm/stabbing and persistent background pain are present. Mixed pain can appear in the early postpartum period. | 日常使用 06 Chronic Mode，急性发作可使用 07 Acute Mode 缓解。 | Use "06 Chronic Mode" daily; for acute flare-ups, use "07 Acute Mode" for relief. |
| Mixed Acute + Chronic | 1–6 weeks | 混合疼痛，既有急性刺痛/痉挛，又有持续酸痛或神经性痛。产后恢复中期常见。 | Mixed pain with both acute stabbing/spasm and persistent aching or neuropathic pain. Common in mid-postpartum recovery. | 日常 06 Chronic Mode 缓解基础疼痛，急性 flare 时使用 07 Acute Mode。 | Use "06 Chronic Mode" daily to relieve background pain; switch to "07 Acute Mode" during acute flares. |
| Mixed Acute + Chronic | >6 weeks | 持续混合疼痛，背景慢性痛加急性触发痛。超过 6 周仍存在，提示慢性机制明显。 | Persistent mixed pain combining chronic background pain and acute triggers. Persistence over 6 weeks suggests a clearly chronic mechanism. | 建议 06 Chronic Mode 日常使用，急性 flare 使用 07 Acute Mode 并考虑专业评估。 | Recommend daily "06 Chronic Mode"; use "07 Acute Mode" for acute flares and consider professional evaluation. |

---

### 第三步：定严重程度 + 训练频次（NRS Score） / Step 3 · Severity + Frequency

| NRS | 严重程度文案（中文） | Severity Output (EN) | 训练频次 | 周数 |
|---|---|---|---|---|
| 0 | 无不适，不影响正常活动。 | No discomfort, normal activity not affected. | 无需 TENS | — |
| 1–3 | 能察觉到，但未显著干扰日常活动。 | Noticeable but does not significantly interfere with daily activities. | 3 次/周 | 2 周 |
| 4–6 | 干扰部分活动，可能需要止痛药或非药物措施。 | Interferes with some activities, may need analgesics or non-pharmacological measures. | 5 次/周 | 3 周 |
| 7–10 | 显著限制活动，可能需要紧急疼痛管理。 | Significantly limits activity, may require urgent pain management. | 每日 1 次 | 4 周 |

---

### Q1 安全门控 / Safety Gate

Q1 选了以下任一风险项（前 5 项）→ 评估中止，不推荐任何模式，展示就医警告。

If any of the 5 risk items is selected in Q1 → assessment aborts, no mode recommended, clinical referral warning shown.

| 选项 / Option | 中文 | English | 触发安全门控 |
|---|---|---|---|
| 1 | 发热 | Fever | ✓ |
| 2 | 伤口处红肿加剧 | Increasing redness or swelling at wound site | ✓ |
| 3 | 恶臭分泌物 | Foul-smelling discharge | ✓ |
| 4 | 单侧腿部突然严重肿胀 | Sudden severe swelling in one leg | ✓ |
| 5 | 麻木或大小便失禁 | Numbness or loss of control of bladder or bowel | ✓ |
| 6 | 无（继续评估） | None | — |

**警告文案 / Warning copy**：

| 中文 | English |
|------|---------|
| ⚠️ 请先咨询专业医生后再使用本设备。 | ⚠️ Please contact a healthcare professional before using the device. |

---

### 页面结构 / Page Structure

1. 评估得分（大字百分比 + NRS X/10 · 持续时间）
2. 分型结果卡片（第二步输出的疼痛类型文案 + 模式方案文案）
3. 严重程度卡片（第三步 NRS 文案原文）
4. 推荐训练计划卡片（Mode 编号+中英名 · TENS · 单次时长 · 频次/周 · 周数 · 总次数）
5. 免责声明
6. 底部按钮：`Customize Training Plan` / `Skip for Now`

---

### 免责声明 / Disclaimer

**中文**：本评估及训练建议仅供个人健康管理参考，不构成医疗评估或医疗建议。个性化推荐基于您自行填写的问卷和使用数据，不代表临床改善证明。如症状持续、加重或出现异常，请及时咨询专业医疗人员。

**English**: This assessment and training recommendations are for personal wellness reference only. They do not constitute medical diagnosis or medical advice. Personalized suggestions are based on your self-reported data and do not represent clinical outcomes. If symptoms persist, worsen, or become unusual, please consult a qualified healthcare professional.
