# 使用说明

## 适用任务

一节40分钟小学数学课需要判断教师是否过度使用封闭式提问。

## 准备输入

课堂转录或结构化观察记录、年级学科、教学目标、班型、观察重点、已脱敏学生标识。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 核对转录质量
2. 切分教学片段
3. 编码提问与反馈
4. 统计参与和等待时间
5. 提炼模式
6. 给出保留点与改进实验

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

业务负责人复核输入事实、关键假设和最终成果适用范围后，成果才可进入正式业务使用。
