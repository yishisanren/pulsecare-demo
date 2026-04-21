---
title: "3.3 疼痛评估问卷 (Red-Flag + Pain Descriptor + NRS)"
path: "功能三 > 问卷评估 > 疼痛问卷"
---


## 3.3 疼痛评估问卷

包含安全筛查（红旗） + 疼痛描述词 + 持续时间 + 分部位 NRS + 疼痛性状 / 频率 / 单次时长。

### Q1：Red-Flag 安全筛查

**题干**：Do you have any of the following along with the pain?
**题型**：多选
**选项**：

- ☐ Fever
- ☐ Increasing redness/swelling at wound site
- ☐ Foul-smelling discharge
- ☐ Sudden severe swelling in one leg
- ☐ Numbness or loss of control of bladder/bowel
- ☐ None

**路由 / 安全门控**：勾选除 None 以外的任一项 → 直接退出问卷，显示就医警告"⚠️ 请先咨询专业医生后再使用本设备。"不推荐任何模式；勾选 None → 继续 Q2。

### Q2：疼痛描述（Pain Descriptor）

**题干**：Which best describes your pain?
**题型**：单选
**选项**：

- Cramping / Tightening / Spasm
- Aching / Dull / Heavy
- Sharp / Stabbing / Shooting
- Burning / Tingling / Electric
- Pain with Light Touch / Allodynia
- Pain Comes and Goes / Activity-related

### Q3：疼痛持续时间

**题干**：How long have you had this pain?
**题型**：单选
**选项**：

- Less than 1 week
- 1–6 weeks
- More than 6 weeks

### Q4：当前疼痛强度（总体 NRS）

**题干**：Please rate your current pain on a scale from 0 (no pain) to 10 (worst pain).
**题型**：11 分量表
**选项**：no pain【 0 —— 1 —— 2 —— 3 —— 4 —— 5 —— 6 —— 7 —— 8 —— 9 —— 10 】worst pain

### Q4–Q6：分部位 NRS

| 题号 | 问题题干 | 选项 |
|------|------|------|
| Q4 | Pelvic Pain / Uterine Cramping | (0–10) |
| Q5 | Lower Back Pain | (0–10) |
| Q6 | Leg Pain / Cramps | (0–10) |

### 疼痛性状（Pain Quality）

**题干**：Pain Quality (check all that apply):
**题型**：多选
**选项**：

- ☐ Dull：Continuous, deep ache
- ☐ Sharp：Sudden, intense, stabbing pain
- ☐ Burning：Hot, tingling, or stinging sensation
- ☐ Cramping：Tight, squeezing, or intermittent pain
- ☐ Throbbing：Pulsating, rhythmic pain
- ☐ Shooting：Pain traveling along a nerve path
- ☐ Aching：Generalized, mild to moderate discomfort
- ☐ Other: __________

### 疼痛频率 / 单次时长

| 项目 | 选项 |
|------|------|
| Pain Frequency | ☐ Constant ☐ Intermittent ☐ Frequency per day |
| Duration per episode | __________ minutes |

### 其他部位 NRS

| 项目 | 选项 | 备注 |
|------|------|------|
| Perineal or Surgical Wound Pain | (0–10) | 有手术时评估 |
| Breast Pain / Engorgement | (0–10) | — |
| Other (specify): __________ | (0–10) | — |

---

### Q2 描述词 × Q3 持续时间 → 设备模式 / Pain Type Mapping

| Q2 描述词类型 | 中文 | 持续时间分流 | 映射设备模式 |
|---|---|---|---|
| Acute / Muscle-related（Cramping/Tightening/Spasm） | 急性 / 肌肉相关 | 任意持续时间 | `07 Acute Mode` |
| Acute nociceptive（Sharp/Stabbing/Shooting） | 急性 伤害感受性 | < 6 weeks | `07 Acute Mode` |
| Chronic nociceptive（Aching/Dull/Heavy） | 慢性 伤害感受性 | ≥ 6 weeks | `06 Chronic Mode` |
| Chronic neuropathic-like（Burning/Tingling/Electric + Pain with Light Touch） | 慢性（类）神经病理性 | ≥ 6 weeks | `06 Chronic Mode` |
| Mixed Acute + Chronic（Pain Comes and Goes） | 混合型（急性+慢性） | 任意持续时间 | `06 Chronic Mode`（日常）+ `07 Acute Mode`（发作时） |

### NRS → 训练频次 / NRS Frequency Mapping

| NRS | 严重程度 | 训练频次 | 周数 |
|---|---|---|---|
| 0 | 无不适，不影响正常活动 | 无需 TENS | — |
| 1–3 | 能察觉到，但未显著干扰日常活动 | 3 次/周 | 2 周 |
| 4–6 | 干扰部分活动，可能需要止痛药或非药物措施 | 5 次/周 | 3 周 |
| 7–10 | 显著限制活动，可能需要紧急疼痛管理 | 每日 1 次 | 4 周 |

---

> 题干与选项文案严格依据《问卷评估需求 20260129》Excel「模块 2：疼痛」原文。详细类型判定与推荐模式输出见"评估结果 · 疼痛首次"页面。
