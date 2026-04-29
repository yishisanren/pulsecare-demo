---
title: "3.4 疼痛评估结果·非首次"
path: "功能三 > 问卷评估 > 疼痛评估结果（非首次）"
---

### 评估结果 · 臀腿疼痛（非首次） / Assessment Result · Hip-Leg Pain (Follow-up)

> 本页规则以《电疗坐垫问卷输出逻辑》为唯一真值源，与 PRD 3.4 保持一致。
> 分型 / 严重程度 / 训练频次 / 模式映射逻辑与首次评估完全相同，详见"评估结果 · 疼痛首次"页面。

---

### 趋势图 / Trend Chart

- 始终展示，最多显示最近 7 次评估 / Always visible, shows up to 7 most recent assessments
- 纵轴为百分比（0–100%）/ Y-axis: percentage (0–100%)
- 横轴为评估次序 / X-axis: assessment index
- 1 次数据显示 1 个点 / A single data point if only one assessment exists

---

### 分型文案（15 条）与严重程度 + 训练频次（NRS 4 档）

详见"评估结果 · 疼痛首次"页面。非首次评估沿用相同规则。

See first-assessment page for full 15-row Q2 × Q3 classification + NRS severity table. Follow-up assessment uses the same rules.

---

### 模式映射 / Mode Mapping

| Q2 判定类型 | 推荐模式 |
|---|---|
| Acute / Muscle-related、Acute nociceptive | 07 Acute Mode · 07 急性疼痛模式 |
| Chronic nociceptive、Chronic neuropathic(-like) | 06 Chronic Mode · 06 慢性疼痛模式 |
| **Mixed Acute + Chronic** | **双模式自动启用：06 Chronic Mode + 07 Acute Mode**（每个训练日同时完成两个模式） |

> **Mixed → 双模式日程（v1.4）**：一日程绑 2 模式（无主副、上下排列），不可修改/拆分/移除。当天 2 个独立任务卡片，顺序固定 `06 Chronic (20 min)` → `07 Acute (30 min)`，共用周期/频次/颜色槽/提醒。

---

### Q1 安全门控 / Safety Gate

与首次评估规则一致。Q1 选风险项（前 5 项任一）→ 评估中止，不推荐任何模式，展示就医警告"⚠️ 请先咨询专业医生后再使用本设备。"

Same as first-assessment logic.

---

### 页面结构 / Page Structure

1. 趋势图（单模块单条曲线）
2. 评估得分（大字百分比 + NRS X/10 · 持续时间）
3. 分型结果卡片
4. 严重程度卡片
5. 推荐训练计划卡片
6. 免责声明
7. 底部按钮：`Customize Training Plan` / `Skip for Now`

---

### 免责声明 / Disclaimer

**中文**：本评估及训练建议仅供个人健康管理参考，不构成医疗评估或医疗建议。个性化推荐基于您自行填写的问卷和使用数据，不代表临床改善证明。如症状持续、加重或出现异常，请及时咨询专业医疗人员。

**English**: This assessment and training recommendations are for personal wellness reference only. They do not constitute medical diagnosis or medical advice. Personalized suggestions are based on your self-reported data and do not represent clinical outcomes. If symptoms persist, worsen, or become unusual, please consult a qualified healthcare professional.
