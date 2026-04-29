---
title: "4.5 训练完成激励"
path: "功能四 > 训练执行 > 完成激励"
---


## 4.5 训练完成激励

每次训练结束后的激励反馈页面，根据完成度提供不同的鼓励内容。

### 激励等级规则

**100% 完成**
- 图标：🎉 庆祝表情
- 标题："Fantastic! Training Complete!"
- 描述："You completed the full session. Great commitment to your health!"

**90-99% 完成**
- 图标：⭐ 星星表情
- 标题："Great Job! Almost There!"
- 描述："You're doing excellent! Every session brings you closer to your goals."

**70-89% 完成**
- 图标：💪 肌肉表情
- 标题："Good Effort! Keep Going!"
- 描述："You're making progress! Consistency is key to seeing results."

**<70% 完成**
- 图标：🌱 成长表情
- 标题："Every Step Counts!"
- 描述："Starting is the hardest part. You're building healthy habits!"

### 训练数据展示
**训练详情卡片**
- 训练时长：实际训练时长（如"18 mins"）
- 训练模式：完成的模式名称（如"01 Activation"）
- 完成进度：百分比显示（如"75%"）
- 日程进展：当前进度/总训练次数（如"8/24"）

### 心情反馈入口
在激励内容下方提供心情选择：
- 5个表情选项：Great/Good/Okay/Bad/Terrible
- 用户可选择当次训练的心情感受
- 心情数据记录在训练记录中

### <span class="v14-add">双模式日程当天的衔接</span>
<span class="v14-add">当天属于双模式日程（08+09 或 06+07）时，训练完成激励按"单次训练"独立触发：</span>
- <span class="v14-add">完成第 1 个任务（如 06 Chronic）后正常显示激励页 + 心情反馈，关闭后回到日程主页</span>
- <span class="v14-add">主页可见第 2 个任务卡片（07 Acute）仍为 Pending，可立即开始或稍后训练</span>
- <span class="v14-add">2 个任务都完成后，整条双模式日程当天才记 +1（共用进度条）</span>
- <span class="v14-add">日程**周期完成**的庆祝页要等两个模式都跑完才触发（详见日程完成页）</span>
