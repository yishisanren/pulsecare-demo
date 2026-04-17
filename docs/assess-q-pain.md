---
title: "3.3 疼痛评估问卷 (4 题)"
path: "功能三 > 问卷评估 > 疼痛问卷"
---


## 3.3 疼痛评估问卷

> 与 PRD 3.3 模块 2 保持一致。共 4 题。

| 题号 | 问题 / Question | 类型 | 选项 / Options | 规则 / Rule |
|------|-----|------|----------|-----|
| **Q1** | Do you have any of the following along with the pain? | 多选 | 发热 / 伤口处红肿加剧 / 恶臭分泌物 / 单侧腿部突然严重肿胀 / 麻木或大小便失禁 / 无（继续评估）| **安全门控**：选了前 5 项任一 → 退出问卷，显示就医警告"⚠️ 请先咨询专业医生后再使用本设备。"不推荐任何模式 |
| **Q2** | Which best describes your pain? | 单选 | Cramping/Tightening/Spasm / Aching/Dull/Heavy / Sharp/Stabbing/Shooting / Burning/Tingling/Electric / Pain with Light Touch / Pain Comes and Goes | **确定疼痛类型**（映射到 5 个 Q2 判定类型）|
| **Q3** | How long have you had this pain? | 单选 | Less than 1 week / 1-6 weeks / More than 6 weeks | **辅助类型判定**（用于 Q2 × Q3 分型文案输出）|
| **Q4** | Rate your current pain (0-10) | 滑块 | No pain (0) — Worst pain (10) | **NRS 评分**，用于确定训练频次和周数 |

### Q2 描述词聚合 → 设备模式 / Q2 Descriptor Aggregation

| Q2 描述词判定类型 / Type | 中文 | 映射设备模式 |
|---|---|---|
| Acute / Muscle-related (Cramping/Tightening/Spasm) | 急性 / 肌肉相关 | 07 Acute Mode |
| Acute nociceptive (Sharp/Stabbing/Shooting) | 急性 伤害感受性 | 07 Acute Mode |
| Chronic nociceptive (Aching/Dull/Heavy) | 慢性 伤害感受性 | 06 Chronic Mode |
| Chronic neuropathic-like / Chronic neuropathic (Burning/Tingling/Electric + Pain with Light Touch) | 慢性（类）神经病理性 | 06 Chronic Mode |
| Mixed Acute + Chronic (Pain Comes and Goes) | 混合型（急性+慢性）| 06 Chronic Mode（日常）+ 07 Acute Mode（发作时）|

### NRS 训练频次映射 / NRS → Frequency

| NRS | 严重程度 | 训练频次 | 周数 |
|---|---|---|---|
| 0 | 无不适，不影响正常活动 | 无需 TENS | — |
| 1–3 | 能察觉到，但未显著干扰日常活动 | 3 次/周 | 2 周 |
| 4–6 | 干扰部分活动，可能需要止痛药或非药物措施 | 5 次/周 | 3 周 |
| 7–10 | 显著限制活动，可能需要紧急疼痛管理 | 每日 1 次 | 4 周 |

详见 PRD 3.4 模块 2 结果计算（`assess-result-pain-first.md`）。
