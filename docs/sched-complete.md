---
title: "5.7 日程完成与评估引导"
path: "功能五 > 训练日程管理 > 完成引导"
---


## 5.7 日程完成与评估引导

当用户完成一个完整的训练计划周期后的引导流程。

### 完成庆祝页面
**庆祝元素**
- 庆祝图标：🎉 或类似庆祝表情
- 标题："Congratulations! Plan Complete!"
- 训练统计：总训练天数、总时长、完成率

**单模块完成**
- 显示该模块的完成统计
- 直接引导重新评估该症状

**多模块同时完成**
- 显示所有完成模块的汇总统计
- 依次引导评估各个症状模块

<span class="v14-add">**双模式日程完成**</span>
- <span class="v14-add">触发条件：**两个模式都跑完**为周期结束（不是其中一个跑完就触发）</span>
- <span class="v14-add">统一弹一次完成页，文案：`Congratulations! You have completed your [模块名] training plan (covering [模式1] and [模式2]).`</span>
- <span class="v14-add">分别展示两个模式的训练次数 / 累计时长 / 完成率（顺序与计划生成 Step 3 一致：08 SUI → 09 UUI 或 06 Chronic → 07 Acute）</span>
- <span class="v14-add">引导重新评估该模块（一次评估，不分别引导）</span>

### 重新评估引导
**引导文案**
"It's time to reassess your [症状名称] to see how much you've improved!"

**操作按钮**
- **"Reassess Now"**：立即进入问卷评估
- **"Later"**：稍后评估，用户可从设备主页的评估入口主动发起

### Later 处理逻辑
用户选择"Later"后：
- 不在主页显示红点提醒（删除此逻辑）
- 用户可随时从"Take Assessment"入口重新评估
- 重新评估时触发日程替换逻辑

### 日程替换确认
如果用户已有生效日程但重新评估后生成新方案：
- 弹窗确认："您有正在进行的训练计划，确认替换为新方案吗？"
- "Replace"：删除旧日程，启用新方案
- "Cancel"：保持现有日程不变
