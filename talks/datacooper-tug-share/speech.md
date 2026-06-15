# Datacooper TUG 分享讲稿

> 时长：30 分钟演讲 + 10 分钟 Q&A
> 含 4 段视频 Demo，播放时做简短旁白即可

---

## 【P1】标题页

各位好，今天分享的主题是"从手工拖拽到工程化 BI"。

我会围绕三个东西展开：cwprep、cwtwb，以及 datacooper.com。

先看一下今天的内容安排。

## 【P2】目录

今天分四个部分：

第一部分是背景与定位——这些工具为什么存在，适合谁用。

第二部分是 cwprep——Tableau Prep 的数据流引擎。

第三部分是 cwtwb——Tableau Workbook 的工程化生成。

第四部分是 datacooper.com 的未来方向，以及怎么快速上手。

先说一个定位，免得大家产生误解。

## 【P3】工具定位

这些 Python 工具不是用来替代 BI 开发人员的，也不是要把分析师变成程序员。

定位很简单：**辅助加速 BI 开发过程**。把重复的、机械的、可规则化的工作交给工具，让开发者把时间花在业务理解和结果判断上。

## 【P4】Tableau 在数据分析全流程中的位置

在展开之前，先快速对齐一下 Tableau 在整个数据分析流程里的位置。

整个流程大致分五步：数据接入、数据准备、Tableau 建模和可视化、分发协作、反馈优化。

我们的工具主要落在两个环节：cwprep 落在"数据准备"，cwtwb 落在"Tableau 生成与编排"。中间由 Tableau 本身承接分析表达。

## 【P5】为什么要做这些工具

那问题来了，为什么要做这些工具？

## 【P6】机械劳动的痛点

如果回头看 Tableau 的日常开发，最耗时的往往不是"画一个图"，而是这些机械动作：

反复拖拽字段、反复调布局、反复复制 KPI 模块、反复迁移 workbook、反复检查文件能不能正常打开、反复修一些很细碎但很耗时间的问题。

这些事单个看都不难，但它们有一个共同的问题：**不创造新的业务价值，却持续消耗开发时间**。

## 【P7】这些工具适合谁

所以这些工具适合谁？三类人：

第一，**Tableau 分析师**——减少重复拖拽和复制粘贴，把时间还给业务分析和洞察判断。

第二，**数据工程和 IT**——自动化、版本控制、批量部署，让 BI 进入工程化流程。

第三，**团队管理者**——可审计、可复现、可交付，降低人员依赖和知识流失风险。

## 【P8】cwprep

好，接下来进入第一个工具：cwprep。

## 【P9】cwprep 一句话介绍

cwprep 的定位用一句话说清楚：**输入一句话，输出一个可用的 Tableau Prep .tfl / .tflx 文件。**

四个核心能力：Text-to-PrepFlow——用自然语言描述数据处理逻辑；MCP 集成——可接 Claude、Gemini、Cursor 这些客户端；避免 GUI 依赖——不用打开 Tableau Prep 也能构建流程；可审查——支持把 flow 翻译成 SQL，便于 DBA 和合规团队查看。

底层支持 22 种数据流操作、4 种数据库、SQL 翻译、TFLX 打包。

核心价值也很清楚：cwprep 管"数据怎么流动"，cwtwb 管"仪表板怎么生成"。效率加速、质量稳定、工程协作。

## 【P10】cwprep 架构图

大家看这个架构图。cwprep 是分层设计的。

最上面是接口层，左边是 MCP Server，支持 Claude、Cursor、VSCode、Gemini 这些客户端；右边是 Python Library，可以直接 import 来写脚本。

中间是核心引擎 TFLBuilder，包含 TFLBuilder、TFLPackager、SQLTranslator、ExpressionTranslator 四个核心组件。

再下面是操作层，分三块：数据源——支持 MySQL、PostgreSQL、SQL Server、Excel、CSV；转换操作——Join、Union、Filter、Rename、Calculation、Pivot 等等；分析与输出——聚合、逆透视、SQL 翻译、TFLX 打包。

最后是校验和打包，输出 .tfl 或 .tflx 文件。

这里有一个很关键的分支：**SQL Translator**。很多 BI 场景里，真正卡住的不是能不能做，而是能不能解释、能不能审、能不能给 DBA 看。SQL 翻译就是解决这个问题的。

## 【P11】cwprep vs Tableau Agent

我知道很多人会问：Tableau 自己不是有 Agent 吗，为什么还要做 cwprep？

做一个直接对比。Tableau Agent 是官方闭源产品，自然语言驱动 Prep 流，但仅限 Tableau Cloud，而且**不支持 Join 和 Union**，也不支持 SQL 导出。

cwprep 是开源的，可以本地部署，支持任意环境，Join、Union、Pivot 都支持，还能把整个 flow 翻译成 SQL。

简单来说：官方 Agent 能做的，cwprep 基本都能做；官方 Agent 做不了的，cwprep 也能做。功能覆盖率达到 88%。

## 【P12】cwprep 典型案例与快速演示

这里有两个典型案例，直接看 Demo。

**案例 1：零门槛秒级生成。** 完全不需要本地安装 Tableau Prep。用户通过自然语言把清洗逻辑发给 Agent，系统在几秒内直接生成标准的 .tfl 文件。

**案例 2：多表复杂逻辑解析。** Agent 深度理解多步骤、跨多张表的业务描述——订单、退货、客户之间的关联，自动识别 ER 关系和 Join 逻辑，精准转化成数据管道。

先看第一段视频。

> 【播放视频 1：极速生成】

简单场景下的秒级响应。再看第二个。

> 【播放视频 2：复杂逻辑】

即使是多表关联的复杂场景，Agent 也能准确解析并生成完整的 Prep 流。

## 【P13】cwtwb

接下来是第二个工具：cwtwb。

如果说 cwprep 管的是"数据怎么流动"，那 cwtwb 管的是"仪表板怎么生成"。

## 【P14】cwtwb 架构图

大家看这个架构图，也是分层设计。

接口层：左边是 MCP Server，支持 Claude、Cursor、VSCode、Claude Code；右边是 Python Library，import TWBEditor 就能用。

核心是 TWBEditor，由四个 Mixin 组成：ParametersMixin 管参数，ConnectionsMixin 管数据连接，ChartsMixin 管图表，DashboardsMixin 管仪表板。

下面三个子系统：Chart Builders——支持 Basic、DualAxis、Pie、Text、Map、Recipes 等图表构建；Dashboard System——负责布局、交互动作和依赖管理；Analysis & Migration——迁移工具、分析器和能力注册表。

最底层是 XML Engine，基于 lxml，把模板经过 patch、validate、save 流程，输出 .twb 或 .twbx。

## 【P15】cwtwb vs Tableau Agent (Web)

同样做一个对比。这次对标 Tableau Agent 的 Web 端。

Tableau Agent Web 端目前只能生成 Worksheets 工作表，无法构建完整 Dashboard，不支持格式化美化，不支持参数和集，也不支持数据建模。

cwtwb 可以做到完整的 Dashboard 编排、声明式布局与格式化、跨源数据迁移、XSD 结构校验与版本化。

cwtwb 填补的是官方 Agent 在复杂布局和自动化生产上的空白。

## 【P16】cwtwb 一句话介绍

一句话概括：**手工拖半天的仪表板，AI 一句话从零生成——cwtwb 让每个 Tableau 用户都提速 10 倍。**

四个核心能力：生成——从代码或 agent 调用生成 TWB；校验——结构校验加 XSD 校验；迁移——快速迁移到新数据源；编排——支持 Chart 和 Layout 编排。

支持 15+ 图表类型、50+ MCP 工具。核心价值三个词：确定性输出、交付可验证、适合迁移项目。

## 【P17】cwtwb 实战案例与闭环演示

看两个实战案例。

**案例 3：MCP 驱动的 AI 看板生成。** 只需配置 MCP 服务、提供数据源和模板，输入你的需求，AI 就能自动规划布局并生成 Tableau 文件。零代码，自然语言描述就能出看板。

**案例 4：端到端实时仪表板渲染。** 从原始文档到功能完备的 Tableau 仪表板。大家可以直接看到 Dashboard 从无到有的渲染过程，就像"热更新"仪表板一样。

> 【播放视频 3：MCP 驱动的 AI 看板生成】

> 【播放视频 4：Dashboard 实时渲染】

## 【P18】datacooper.com

最后一个部分：datacooper.com。

如果说 cwprep 和 cwtwb 是底层能力，那 datacooper.com 就是把这些能力面向用户、面向社区的产品化入口。

## 【P19】datacooper 在线工具原型

方向很简单：不只是本地脚本，而是做成在线工具平台。底层共用 Python SDK。

目前已经有两个工具原型：

第一个是**布局解析**——上传 workbook，自动提取 dashboard 布局结构，导出 JSON。

第二个是**KPI 复制**——复制 KPI 工作表，只替换指标，保留原结构和样式。这个在现实 BI 场景里特别实用，因为经常不是从零做一个 KPI，而是复制一个已验证的模板，只换一个指标。

更远的方向是协作与版本管理——创想方向，非当前承诺。

## 【P20】试试看

两个工具都已发布到 PyPI，一行命令就能安装：

```
pip install cwprep cwtwb
```

MCP 服务器也有独立入口：cwprep-mcp 和 cwtwb-mcp。

GitHub 上有源码，datacooper.com 上有在线工具和文档。开源项目，AGPL-3.0 协议，欢迎大家 Star、试用、反馈。

## 【P21】致谢

在结束之前，我想感谢一些在这个过程中给了我很大帮助的人。

感谢 Patrick Therriault，引导我深入 Tableau 社区。感谢 Andy Cotgreave，他的洞察推动了项目前进。感谢 Adam Mico，一直以来的耐心和扎实建议。感谢 Jeffrey Shaffer，你推荐的技巧成了很好的过程约束。感谢 Matthew Miller、Elif Tutuk、Paul Morgan、Olga L.，来自官方的极有价值的提示。感谢 Li-Lun Tu 在品牌建设方面的建议。感谢 Alex Mou 的鼓励以及交流中给我的建议。

也感谢每一位留言和参与讨论、帮助我走在正确方向上的朋友。

## 【P22】结语

最后留一句话：

**不离开 Tableau，用 AI 把时间还给人类。**

## 【P23】Q&A / 交流

好，正式内容讲完了。大家有什么问题，或者想聊的方向，我们现在可以交流。

> 【Q&A 时间，约 10 分钟】

谢谢大家。
