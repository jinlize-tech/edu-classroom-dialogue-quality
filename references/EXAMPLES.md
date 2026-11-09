# 课堂对话与提问质量分析示例

## 典型场景

一节40分钟小学数学课需要判断教师是否过度使用封闭式提问。

## 具体示例

输入脱敏转录后，系统引用具体片段说明连续6次一问一答、平均等待时间偏短，并建议设计一次等候3秒的开放问题实验。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "transcript_redacted": "脱敏课堂转录已核对（脱敏示例）",
  "grade_and_subject": "年级与学科已核对（脱敏示例）",
  "learning_objectives": [
    {}
  ],
  "class_type": "班型已核对（脱敏示例）",
  "observation_focus": [
    {}
  ],
  "consent_status": "已取得明确授权并完成脱敏"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出课堂对话分析表、问题/追问片段、改进建议等核心成果。
5. 由业务负责人确认输入事实、关键假设和最终成果适用范围后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
