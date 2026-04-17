---
title: "3.0 知情同意页"
path: "功能三 > 问卷评估 > 知情同意"
---


## 3.0 知情同意页 (Informed Consent)

评估流程的入口页面，用户必须阅读并同意后才能开始评估。

### 页面结构（4个信息区块 + 复选框）

**1. About This Assessment**
- 说明评估内容：盆底肌症状（尿失禁、疼痛、功能限制）
- 预估时长：5-10分钟
- 用途：生成个性化训练方案

**2. Non-Diagnostic Disclaimer**
- 明确声明：本评估不是医学评估
- 结果仅供参考，不替代专业医疗建议
- 症状严重请咨询医生

**3. Privacy & Data Handling**
- 数据本地存储，仅用于生成训练推荐
- 不与第三方共享
- 可在设置中随时删除数据

**4. Consent Checkbox**
- 文案："I have read and understood the above information, and I consent to proceed with this assessment."
- 必须勾选才能启用"Start Assessment"按钮

### 交互逻辑
- 底部按钮 `Start Assessment` 初始禁用（disabled）
- 勾选复选框后按钮启用
- 取消勾选按钮重新禁用
- 点击按钮跳转 → `assess-select`

### 导航
- 顶部 Cancel → 返回主页
