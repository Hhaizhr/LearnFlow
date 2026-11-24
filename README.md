# LearnFlow Agent

面向开发者的**本地优先、主动式**学习与知识成长 Agent。

不是帮你保存更多笔记，而是把散落在 AI 对话、Markdown、代码实践里的学习记录，变成**可追溯的长期记忆 → 跨来源知识关联 → 少而有用的下一步建议 → 真实产出（实验 / 技术博客）**。

> 核心闭环：知识采集 → 知识理解 → 长期记忆与关联 → 主动发现 → 用户确认 → 学习/实践/写作 → 反馈入库

## 当前状态

**设计阶段收尾，M0（工程底座）进行中。** 仓库暂无可运行产品，只有设计文档与工程骨架。

- 唯一事实源：[LearnFlow Core MVP 实施设计 V0.3](docs/LearnFlow%20Core%20MVP%20实施设计%20V0.3.md)
- 历史文档：
  - [V0.1 项目设计文档](docs/LearnFlow%20Agent%20项目设计文档.md)
  - [V0.2 产品与核心技术设计](docs/LearnFlow_Agent_产品与核心技术设计_V0.2.md)
  - [V0.2 工程落地细化版](docs/learnflow_agent_v0_2.md)

## 计划中的技术栈

| 层 | 选型 |
| --- | --- |
| 后端 | Java 21 + Spring Boot 4.x + Spring AI 2.x（版本以 M0 实测锁定） |
| 数据 | PostgreSQL 16 + pgvector，中文全文检索（zhparser 或应用侧分词） |
| 前端 | React 19 + TypeScript + Vite + Tailwind + CodeMirror 6 |
| 工作流 | 自研确定性状态机 + PostgreSQL 任务队列 |
| 部署 | Docker Compose，本地优先，支持本地 Ollama / 云端模型按隐私策略路由 |

## MVP 只验证一件事

> 给定多日、跨来源的真实学习记录，LearnFlow 能否产出**有原文证据、可执行、低打扰**的学习与博客选题建议？

## 开发

M0 完成后，本节会替换为实际的一键启动说明。计划中的命令：

```bash
docker compose up -d
```

## 许可

待定（计划 MIT）。
