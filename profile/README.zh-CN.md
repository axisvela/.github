# AxisVela

[English](README.md) | **简体中文**

**独立开发者项目**，面向受治理的自治系统 —— 智能体、工作流、机器人与数字孪生 —— 全部公开构建。

AxisVela 是个人维护的项目集合，不是一家公司。公开仓库是开放的界面：可运行的框架、协议、契约、SDK 与参考实现。核心版与企业版在私有仓库中开发并单独提供。

## 完整项目地图

有关完整地图 —— 每个项目的目标、关系、概念以及从哪里开始 —— 请参阅 [AxisVela Open](https://github.com/axisvela/axisvela-open) 或[文档站点](https://axisvela.github.io/axisvela-open/)。

## 从这里开始

### [praxo-core](https://github.com/axisvela/praxo-core) —— MIT 智能体框架

进入整个生态系统的入口。一个真实、可运行的 Go 框架，而不是空壳契约：

- 受治理的智能体循环，以及模型 / 工具 / 记忆 / 事件原语
- 插件、沙箱与策略执行
- MCP、Anthropic 与 OpenAI 适配器
- OpenTelemetry 埋点与基准测试
- 双语文档与 MkDocs 站点

先克隆它。运行它不需要本组织中的任何其他仓库。

```bash
git clone https://github.com/axisvela/praxo-core
cd praxo-core
go test ./...
```

## 生态地图

公开仓库分为三层。

### 可运行的框架与协议

| 仓库 | 简介 |
| --- | --- |
| [praxo-core](https://github.com/axisvela/praxo-core) | MIT 智能体框架：循环、适配器、沙箱、策略、OTel |
| [harmovela](https://github.com/axisvela/harmovela) | 面向自治系统的开放协调协议 |
| [TAXOVELA](https://github.com/axisvela/TAXOVELA) | AI 原生企业架构设计与校验技能 + CLI |
| [enterprise-autonomy](https://github.com/axisvela/enterprise-autonomy) | 更广泛生态系统的介绍与端到端示例 |

### 开放产品界面

每个 `*-open` 仓库发布某款产品的 Apache-2.0 集成界面：版本化契约、SDK、CLI、示例，部分还提供签名二进制文件。其背后的运行时位于独立的私有核心仓库中。

| 领域 | 公开界面 |
| --- | --- |
| 开发协作 | [coordivela-open](https://github.com/axisvela/coordivela-open) |
| 持久化工作流 | [rheovela-open](https://github.com/axisvela/rheovela-open) |
| 智能体记忆 | [mnemovela-open](https://github.com/axisvela/mnemovela-open) |
| 身份与授权 | [aegivela-open](https://github.com/axisvela/aegivela-open), [eidovela-open](https://github.com/axisvela/eidovela-open), [NOMIVELA-open](https://github.com/axisvela/NOMIVELA-open) |
| 集成网关 | [limenora-open](https://github.com/axisvela/limenora-open) |
| 语义与知识织物 | [gnosivela-open](https://github.com/axisvela/gnosivela-open), [ontovela-open](https://github.com/axisvela/ontovela-open) |
| 验证与仿真 | [tekmovela-open](https://github.com/axisvela/tekmovela-open), [peiravela-open](https://github.com/axisvela/peiravela-open), [SYNDOVELA-open](https://github.com/axisvela/SYNDOVELA-open) |
| 能力与规划 | [moduregis-open](https://github.com/axisvela/moduregis-open), [orchadyn-open](https://github.com/axisvela/orchadyn-open) |
| 运维与协作 | [symbivela-open](https://github.com/axisvela/symbivela-open), [noetivela-open](https://github.com/axisvela/noetivela-open), [kinetovela-open](https://github.com/axisvela/kinetovela-open) |

### 相邻项目

| 仓库 | 简介 |
| --- | --- |
| [AXISRobo-PAMP](https://github.com/axisvela/AXISRobo-PAMP) | 面向企业架构管理的实用平台 |

## 如何参与

- **试用生态系统：** 从 [praxo-core](https://github.com/axisvela/praxo-core) 开始。如果它无法运行，那就是一个值得反馈的缺陷。
- **使用某个开放界面：** 在对应的 `*-open` 仓库提交 issue。
- **商业或企业使用：** 在相关仓库提交 issue，并询问企业联系途径。
- **安全报告：** 请遵循受影响仓库中的 `SECURITY.md`，而不要提交公开 issue。

## 状态

这些项目处于早期阶段。公开契约已版本化，但在某个仓库宣布 1.0 之前，API 可能会在次要版本之间发生变化。每个仓库的 `CHANGELOG.md`、`ROADMAP.md` 与发布标签是权威来源。
