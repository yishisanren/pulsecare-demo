---
title: "更新日志"
path: "Changelog"
---

## 更新日志

> 本页汇总每次 PRD 版本更新对 demo 页面文档的影响。每个改动点已在对应页面用颜色高亮标注，可点开侧边栏对应页面直接查看。

<div class="v14-legend">
  <span class="lg-add">绿色 = 新增内容</span>
  <span class="lg-change">黄色 = 修改/替换</span>
  <span class="lg-remove">红色 = 已废弃</span>
  <span class="lg-info">蓝色 = 补充说明</span>
</div>

---

## v1.4 · 2026-04-28（双模式日程架构）

### 一句话总结

PRD 此前定义"评估输出双模式（Mixed 分型）"和"日程绑定单模式"互相矛盾，<span class="v14-change">v1.4 引入「双模式日程」架构</span>：<span class="v14-add">**1 条日程绑定 2 个模式（上下排列、无主副之分），每天生成 2 个独立任务卡片，可分别完成或请假；2 模式共用同一周期、频次、颜色槽和提醒时间。**</span>

### 触发场景

| 评估模块 | 触发分型 | 双模式组合 | 任务顺序 |
|---|---|---|---|
| 尿失禁 | <span class="v14-change">Mixed（无条件）</span> | <span class="v14-add">08 SUI + 09 UUI</span> | 08 SUI（20 min）→ 09 UUI（20 min） |
| 疼痛 | <span class="v14-change">Mixed Acute + Chronic</span> | <span class="v14-add">06 Chronic + 07 Acute</span> | 06 Chronic（20 min）→ 07 Acute（30 min） |

> <span class="v14-info">**关键改动**：v1.4 之前 Mixed 用"主+并入"或"日常+发作时"等措辞，存在用户决策模糊。v1.4 改为**自动启用双模式、整体锁定**，移除"主副"概念，移除条件触发。</span>

---

### 改动清单（25 个页面 · 137 处改动点）

#### 评估结果（5 个页面）

| 页面 | 改动类型 | 主要内容 |
|---|---|---|
| **assess-result-first**（尿失禁首次） | <span class="v14-change">改写</span> + <span class="v14-add">新增</span> | Mixed 模式映射 / 新增"Urge 含 Stress 次特征"行 / 引用块 |
| **assess-result-ui-nonFirst**（尿失禁非首次） | <span class="v14-change">改写</span> + <span class="v14-add">新增</span> | 同上 |
| **assess-result-pain-first**（疼痛首次） | <span class="v14-change">改写</span> + <span class="v14-add">新增</span> | 3 个 Mixed 严重度档位文案 / 双模式引用块 |
| **assess-result-pain-nonFirst**（疼痛非首次） | <span class="v14-change">改写</span> + <span class="v14-add">新增</span> | Mixed 模式映射 / 引用块 |
| **assess-result-multi**（多模块） | <span class="v14-change">改写</span> + <span class="v14-add">新增</span> | 尿失禁 + 疼痛两套 Mixed / 跨模块引用块 |

#### 计划生成与预览（4 个页面）

| 页面 | 改动类型 | 主要内容 |
|---|---|---|
| **plan-config**（多模块计划配置） | <span class="v14-add">新增</span> | Step 3 双模式分型规则 / 触发场景表 / Step 4 提醒共享 / 共享配置表 |
| **plan-config-single**（单模块计划配置） | <span class="v14-add">新增</span> | 双模式触发场景章节 |
| **plan-preview**（多模块预览） | <span class="v14-add">新增</span> | 双模式共用颜色槽规则 |
| **plan-preview-single**（单模块预览） | <span class="v14-add">新增</span> | 双模式上下排列说明 |

#### 日程管理（10 个页面）

| 页面 | 改动类型 | 主要内容 |
|---|---|---|
| **sched-home**（当日日程） | <span class="v14-add">新增</span> | 双模式当天显示 2 个任务卡片 |
| **sched-summary**（日程汇总） | <span class="v14-add">新增</span> | 双模式日程合并展示 |
| **sched-edit**（日程编辑） | <span class="v14-add">新增</span> | 双模式整体锁定 |
| **sched-delete**（日程删除） | <span class="v14-add">新增</span> | 不可只删其中一个 |
| **sched-skip**（请假） | <span class="v14-add">新增</span> | 双模式 2 任务可分别请假 |
| **sched-skip-multi**（多任务请假） | <span class="v14-change">改写</span> + <span class="v14-add">新增</span> | 双模式 2 任务也走多任务弹窗 |
| **sched-skip-streak**（连续请假） | <span class="v14-change">改写</span> | 连续请假统计粒度 |
| **sched-undo-skip**（撤销请假） | <span class="v14-add">新增</span> | 撤销 1 个不影响另 1 个 |
| **sched-complete**（完成态） | <span class="v14-add">新增</span> | 2 模式都跑完才弹完成页 |
| **sched-home-skipped / all-skipped** | <span class="v14-add">新增</span> | 1 Skip + 1 待完成 / 全 Skip 混合态 |

#### 训练执行（3 个页面）

| 页面 | 改动类型 | 主要内容 |
|---|---|---|
| **train-complete**（训练完成） | <span class="v14-add">新增</span> | 第 1 任务完成后回主页继续第 2 任务 |
| **train-complete-partial**（部分完成） | <span class="v14-add">新增</span> | 双模式提前结束的衔接 |
| **modal-modes**（模式选择面板） | <span class="v14-add">新增</span> | 双模式不通过此面板修改 |

#### 主页与记录（3 个页面）

| 页面 | 改动类型 | 主要内容 |
|---|---|---|
| **home-connected**（设备主页已连接） | <span class="v14-add">新增</span> | 双模式 2 个任务条目展示 |
| **rec-training**（训练记录） | <span class="v14-add">新增</span> | 双模式当天产生 2 条独立训练记录 |

---

### 不受影响的页面（无需更新）

以下页面与双模式无关，本次未改动：

- 所有 **臀腿（hip-）** 评估页面 —— 模块 3 没有 Mixed 分型
- **assess-result-\*-zero / -risk** —— 0 分态 / 风险态走转诊路径
- **train-mood、home-rest、home-no-schedule、home-completed、rec-assessment** —— 状态页与双模式无关

---

## 历史版本

### v1.3 · 2026-04-20（导览版）
- 评估题目与结果计算的三模块真值表确立
- 9 模式按钮状态机 + 异常兜底

### v1.2 · 2026-04-20（精简版）
- 草稿箱机制
- 安全门控

### v1.1 · 2026-04-13
- 首次评估流程
- 知情同意书框架
