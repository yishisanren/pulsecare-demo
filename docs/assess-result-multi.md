---
title: "3.4 评估结果·非首次多模块"
path: "功能三 > 问卷评估 > 评估结果（非首次多模块）"
---

### 评估结果 · 多模块合并 / Assessment Result · Multi-Module

> 本页规则以《电疗坐垫问卷输出逻辑》为唯一真值源，与 PRD 3.4 保持一致。

---

### 触发条件 / Trigger

用户在筛选路由页勾选了 2 个或 3 个模块并完成评估。
User selected 2 or 3 modules in screening & routing and completed the assessment.

---

### 页面结构 / Page Structure

1. **趋势图 / Trend Chart**：
   - 首次：不展示 / First assessment: hidden
   - 非首次：多条曲线在同一图上（各模块不同颜色 + 图例），最多显示最近 7 次评估，纵轴百分比。
2. **各模块结果卡片（纵向堆叠）**，按 尿失禁 → 疼痛 → 臀腿功能 顺序。
3. 免责声明
4. 底部按钮：
   - 至少 1 个模块有推荐计划 → `Customize Training Plan` + `Skip for Now`
   - 全部模块 0 分态或风险态（无推荐）→ 仅 `返回主页 / Back to Home`

---

## 模块 1 · 尿失禁 / Module 1 · Urinary Incontinence

### 分型文案（16 条 · 完整版）与严重程度 + 训练频次（16 条 · 完整版）

详见"评估结果 · 尿失禁首次"页面。多模块合并页沿用相同规则。

See "评估结果 · 尿失禁首次" page for the full 16-row classification and severity × frequency tables.

### 模式映射 / Mode Mapping

| 3IQ 主类型 | 推荐模式 |
|---|---|
| Stress | 08 SUI Mode · 08 压力性尿失禁模式 |
| Urge | 09 UUI Mode · 09 急迫性尿失禁模式 |
| Mixed | 08 SUI Mode（主），同时存在 Urgency 时训练计划可并入 09 UUI Mode |
| Other | 不推荐模式，建议转诊 |

### 0 分态 / No Symptoms

| 触发 | 中文 | English |
|------|------|---------|
| 3IQ Q1 = No | 未检测到尿失禁症状，暂无需训练。 | No urinary incontinence symptoms detected. Training not required. |

---

## 模块 2 · 臀腿疼痛 / Module 2 · Hip-Leg Pain

### 分型文案（15 条）+ NRS 严重程度（4 档）

详见"评估结果 · 疼痛首次"页面。多模块合并页沿用相同规则。

See "评估结果 · 疼痛首次" page for the full 15-row Q2 × Q3 classification + NRS severity table.

### 模式映射 / Mode Mapping

| Q2 判定类型 | 推荐模式 |
|---|---|
| Acute / Muscle-related、Acute nociceptive | 07 Acute Mode · 07 急性疼痛模式 |
| Chronic nociceptive、Chronic neuropathic(-like) | 06 Chronic Mode · 06 慢性疼痛模式 |
| Mixed Acute + Chronic | 06 Chronic Mode（日常）+ 07 Acute Mode（发作时） |

### 特殊场景 / Special Scenarios

| 场景 | 中文 | English |
|------|------|---------|
| Q1 选风险项（前 5 项）| ⚠️ 请先咨询专业医生后再使用本设备。 | ⚠️ Please contact a healthcare professional before using the device. |
| NRS = 0 | 无症状，不训练。未检测到疼痛症状，日常活动不受影响。 | No symptoms; no training needed. No pain detected; normal activity is not affected. |

---

## 模块 3 · 臀腿功能 / Module 3 · Hip-Leg Function

### 题目数说明

根据合规意见，删除原 Q19，**共 24 题**。PGQ 有效满分 = 24 × 3 = **72**。

### 维度得分公式 / Dimension Scores

| 维度 | 求和题号 | 标准化公式 | 受限阈值 |
|---|---|---|---|
| Control | Q1 + Q16 + Q17 + Q18 + Q20 + Q23（6 题）| / **18** | ≥ 0.3 |
| Endurance | Q2 + Q3 + Q5 + Q6 + Q7 + Q8 + Q9 + Q10 + Q12 + Q14 + Q16 + Q24（12 题）| / **36** | ≥ 0.3 |
| Strength | Q4 + Q9 + Q10 + Q11 + Q12 + Q13 + Q14 + Q15 + Q16 + Q20（10 题）| / **30** | ≥ 0.3 |

### 分型文案（8 条）+ PGQ% 影响程度（4 档）

详见"评估结果 · 臀腿首次"页面。多模块合并页沿用相同规则。

See "评估结果 · 臀腿首次" page for the full 8-row classification + PGQ% impact table.

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
| 三维全 < 0.3 | 不推荐（功能良好）|

### 0 分态 / Good Function

| 触发 | 中文 | English |
|------|------|---------|
| C/E/S 三维度均 < 0.3 | 功能良好，不推荐训练。 | Good function; no training recommended. |

---

## 多模块卡片展示规则 / Multi-Card Display Rules

每张卡片顶部：模块色标点 + 模块名 + 该模块得分百分比（大字）
卡片内容随状态切换：
- **正常结果态**：分型文案 + 严重程度/影响程度 + 推荐训练计划（Mode + 频次 × 周数 + 总次数）
- **0 分态**：展示 "未检测到症状 / 无症状，不训练 / 功能良好，不推荐训练" 对应文案，不显示推荐
- **风险态（仅疼痛模块）**：红色警告 + 风险项列表，不显示推荐

---

### 免责声明 / Disclaimer

**中文**：本评估及训练建议仅供个人健康管理参考，不构成医疗评估或医疗建议。个性化推荐基于您自行填写的问卷和使用数据，不代表临床改善证明。如症状持续、加重或出现异常，请及时咨询专业医疗人员。

**English**: This assessment and training recommendations are for personal wellness reference only. They do not constitute medical diagnosis or medical advice. Personalized suggestions are based on your self-reported data and do not represent clinical outcomes. If symptoms persist, worsen, or become unusual, please consult a qualified healthcare professional.
