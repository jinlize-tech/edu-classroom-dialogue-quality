# 课堂对话与提问质量分析

基于课堂转录或观察记录分析教师提问、学生回应、追问、等待时间和反馈质量，输出可操作的改进建议。

## 适用用户

教师、教研组长、教学主管、课堂观察员

## 主要输出

- 课堂对话分析表
- 问题/追问片段
- 参与结构
- 证据摘要
- 改进建议
- 下一次观察指标

## 安装

将包含`SKILL.md`的根目录导入支持的Skill环境。

本地验证：

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 使用

1. 阅读`USAGE.md`。
2. 按`contract/input.schema.json`准备输入。
3. 调用产品或Agent完成专业处理。
4. 使用`scripts/validate_output.js`检查成果。
5. 高风险结论交由业务负责人确认。

## 边界

- 不使用外部收费API。
- 不依赖其他产品完成核心任务。
- 不自动执行正式审批、退款、人员处罚或系统变更。
- 客户可见内容不包含公司品牌推广或内部研发资料。

## 状态

- 版本：`1.0.0`
- 本地契约与自动化测试：见`test-results/`
- 生成式模型运行：`MODEL_RUNTIME_NOT_VERIFIED`
- WorkBuddy安装、调用、审核、上架：`NOT_EXECUTED`
- 安装包：`dist/edu-classroom-dialogue-quality-v1.0.0.zip`

## 许可证

Apache-2.0。详见`LICENSE`。
