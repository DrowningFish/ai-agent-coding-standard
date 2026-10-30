# Agent 开发约束模板

复制到业务项目的协作与编码约束，帮助AI在工程扩大、长上下文和多人交接后保持方向与质量。本仓库只维护约束文本，不生成自身需求、计划、changelog、检查点或输出资料。

## 使用

1. 复制[AGENTS.md](AGENTS.md)与整个[agent-spec](agent-spec/README.md)目录；已有规则先比较合并，不覆盖项目定制。
2. 用户可填写[project-rules.md](agent-spec/project-rules.md)，也可由Agent按当前任务逐步核实补全。无需先填完整，不默认全库扫描或新建资料。
3. 一项影响较大且需要设计的大需求固定一份文档，范围、设计、状态、审查、验证和交付摘要在同一文件持续更新；普通小改动只简记项目changelog。已有总需求只回补受影响的整体规则，不逐次建补充方案、测试或交付文档，例外见[document-format.md](agent-spec/document-format.md)。
4. 常用角色为方案分析、开发实现、独立审查，专项测试按需启用。需求与必要设计合并沟通，开发负责日常自测，审查按风险检查范围、依据和验证；简单可逆修改可自查。角色不要求各建会话或文档，详见[workflow.md](agent-spec/workflow.md)。
5. 测试从本次差异及受影响路径选择，先针对性检查，再按影响扩大；全量回归须有明确验收/CI要求或全局影响依据，不因新会话、同一大需求持续开发或生成新包重复全测。

## 结构

- AGENTS.md：日常硬约束和按需索引。
- agent-spec/workflow.md：分流、接入、实施、验证与交接。
- agent-spec/security.md：数据、Git、外部工具和协作边界。
- agent-spec/project-rules.md：可填写的项目特别要求。
- agent-spec/document-format.md、delivery.md：需要文档或产物时读取。
- agent-spec/standards/：按实际技术栈使用的后端、前端及接口规范。

不自动创建Agent任务或Git流程，不为套用模板迁移技术栈；模板默认值可由明确项目选择调整。静态检查不能证明模型长期稳定遵循。
