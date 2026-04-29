---
title: "4.5 训练完成激励 - 提前结束"
path: "功能四 > 训练执行 > 提前结束激励"
---


## 训练提前结束激励页

### 触发条件
用户在训练过程中点击 Stop 并确认结束

### 激励档位（根据完成进度）

| 完成度 | 图标 | 标题 | 文案 |
|--------|------|------|------|
| 70-89% | 💪 | Almost there! | You were so close! Every minute counts. |
| 50-69% | 👍 | Good effort! | You completed over half the session. That is real progress. |
| < 50% | 🌱 | Every step counts | Even a short session helps. Keep building the habit! |

### 页面内容
- 激励图标 + 标题 + 文案
- 训练数据卡片：模式名称、实际训练时长、完成进度百分比
- 心情反馈入口（5 级表情）
- 底部按钮："Back to Home"

### <span class="v14-add">双模式日程当天的衔接</span>
<span class="v14-add">当天属于双模式日程时，提前结束按"单次训练"独立触发激励页：</span>
- <span class="v14-add">第 1 个任务提前结束（≥50% 保存记录 / <50% 不保存）后回到日程主页</span>
- <span class="v14-add">第 2 个任务**仍为 Pending 状态**，不受第 1 个任务结束影响，可立即开始或稍后训练</span>
- <span class="v14-add">双模式当天进度按"两个任务的完成情况"独立计算</span>
