# 项目说明

**复制此模板到新项目后，先填写本页**。AI Agent 每次开始任务都会读取这些信息。

## 基本信息

| 项 | 值 |
|---|---|
| 项目名称 | 待填写 |
| 项目目标 | 待填写 |
| 主要用户 | 待填写 |
| 当前阶段 | 需求澄清 |

## 技术选择

| 类别 | 选择 |
|---|---|
| 后端 | JDK 17 + Spring Boot 3.x |
| 构建工具 | Maven / Gradle（待选择） |
| 前端框架 | Vue 3 / React（**必须二选一**） |
| 前端 UI 库 | Element Plus / Ant Design（跟随框架） |
| 数据库 | 待选择（MySQL / TDSQL / TiDB / Oracle） |
| 缓存 | Redis（可选） |
| 配置管理 | Nacos（可选） |
| 注册中心 | Eureka / Nacos（可选） |

## 工程位置

| 项 | 路径 |
|---|---|
| 后端源码根目录 | 待填写，如 `backend/src/main/java` |
| 前端源码根目录 | 待填写，如 `frontend/src` |
| 配置文件目录 | 待填写，如 `backend/src/main/resources` |
| 部署相关目录 | 待填写，如 `deployment/docker` |

## 常用命令

### 后端构建和运行

```bash
# 待填写，例如
mvn clean install
mvn spring-boot:run
# 或
gradle build
gradle bootRun
```

### 后端测试

```bash
# 待填写，例如
mvn test
# 或
gradle test
```

### 前端开发

```bash
# 待填写，例如
npm install
npm run dev
npm run lint
npm run test
npm run build
```

### 本地启动完整应用

```bash
# 待填写：如何一起启动后端和前端
```

### 验证命令

项目验证的关键命令（Agent 在测试阶段会执行这些）：

```bash
# 后端
待填写，通常为：mvn clean verify

# 前端
待填写，通常为：npm run lint && npm run test && npm run build
```

## 文档导航

| 文档 | 用途 |
|---|---|
| `requirements.md` | 需求分析、功能清单、验收标准 |
| `architecture.md` | 系统设计、模块划分、技术方案、关键决策 |
| `development-plan.md` | 里程碑、任务分解、当前进度 |
| `test-plan.md` | 测试范围、测试用例、验证结果 |
| `PROGRESS.md` | 实时进度更新、待办事项、阻塞项 |
| `standards/backend-java.md` | Java/Spring Boot 开发规范 |
| `standards/frontend.md` | Vue3/React 开发规范 |
| `standards/database.md` | 数据库设计规范 |
| `standards/api.md` | API 设计与接口约定 |

## 文档维护原则

- 只记录对后续对话和开发**仍有价值**的内容
- 临时讨论、显而易见的实现细节和可以从代码直接看出的信息**不重复维护**
- 每个文档都可以快速阅读（3-5 分钟）
- 定期（每个里程碑完成后）检查和清理过时内容

## Agent 开始任务流程

1. Agent 会先读取本文件了解项目背景
2. 根据任务类型阅读相关文档
3. 检查现有代码和 `PROGRESS.md` 了解进度
4. 信息足够时直接工作；不足时只提 3-5 个关键问题
5. 完成任务后更新相关文档和 `PROGRESS.md`

---

**模板使用说明**：
- 本文件为新项目的模板，复制到项目后删除"待填写"的项，只保留实际的项目信息
- 不同项目可以根据实际情况调整文档复杂度（不必全部使用）
- 核心原则：**让 Agent 用最少时间理解项目，然后高效地执行任务**
