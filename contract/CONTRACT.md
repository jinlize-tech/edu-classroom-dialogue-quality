# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `transcript_redacted` | 脱敏课堂转录 | string | 是 |
| `grade_and_subject` | 年级与学科 | string | 是 |
| `learning_objectives` | 课堂目标 | array | 是 |
| `class_type` | 班型 | string | 是 |
| `observation_focus` | 观察重点 | array | 否 |
| `consent_status` | 录制与使用授权状态 | string | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `课堂对话分析表`：结构化条目数组，不允许空壳或占位文本。
- `问题/追问片段`：结构化条目数组，不允许空壳或占位文本。
- `参与结构`：结构化条目数组，不允许空壳或占位文本。
- `证据摘要`：结构化条目数组，不允许空壳或占位文本。
- `改进建议`：结构化条目数组，不允许空壳或占位文本。
- `下一次观察指标`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
