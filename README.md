# From Manual Dragging to Engineering BI

This repository contains the slides for the Tableau User Group sharing session about `cwprep`, `cwtwb`, and `datacooper.com`.

---

## Presentation Outline (English)

### 1. Introduction: Positioning & Goals
- Introduction to `cwprep` (Data Prep automation), `cwtwb` (Workbook engineering), and `datacooper.com` (Online platform).
- Goal: Not to replace developers, but to eliminate repetitive, mechanical tasks.

### 2. The Pain Point: Why Build These Tools?
- The hidden cost of "Manual Dragging": fields, layouts, KPI modules, and datasource migrations.
- Paradigm Shift: Transitioning from manual mouse clicks (non-reusable, non-auditable) to an Engineering Approach (modular, version-controlled, auditable).

### 3. Target Audience
- **Tableau Analysts**: Focus on insights rather than dragging.
- **Data Engineers / IT**: Automation and batch deployment.
- **Managers**: Repeatable and verifiable deliverables.

### 4. cwprep: Tableau Prep Automation
- **Architecture**: Text-to-PrepFlow engine with MCP integration.
- **Features**: 22 operations, SQL translation, TFLX packaging.
- **Comparison**: `cwprep` vs. Tableau Agent (Prep). Highlights exclusive support for Join, Union, and SQL translation.

### 5. cwtwb: Tableau Workbook Engineering
- **Architecture**: Workbook Composer, Layout Engine, and Recipe Engine.
- **Features**: Full dashboard orchestration, declarative layouts, XSD validation.
- **Comparison**: `cwtwb` vs. Tableau Agent (Web). Highlights full dashboard support and offline automation.

### 6. Future: datacooper.com
- Transitioning from local scripts to an online BI workspace.
- Current Prototypes: Layout parsing and KPI cloning.

### 7. Getting Started
- Installation and MCP server setup.
- Open source links and community.

---

## 内容大纲 (中文)

### 1. 背景介绍：定位与目标
- 介绍 `cwprep` (数据准备自动化)、`cwtwb` (工作簿工程化) 和 `datacooper.com` (在线平台)。
- 核心定位：不是替代开发人员，而是将重复、机械的工作交给工具。

### 2. 行业痛点：为什么要造轮子？
- “手工拖拽”的隐形成本：反复调整字段、布局、KPI 模块及数据源迁移。
- 范式改变：从纯手工点击（无法复用、无法审计）转向工程化方式（模块化、可版本化、可追溯）。

### 3. 目标受众
- **Tableau 分析师**：将时间还给业务洞察。
- **数据工程 / IT**：实现自动化与批量部署。
- **团队管理者**：确保交付物可复现、可审计。

### 4. cwprep：Tableau Prep 自动化
- **架构设计**：基于 MCP 协议的文本转流程引擎。
- **核心能力**：22 种操作支持、SQL 翻译、TFLX 自动打包。
- **方案对比**：`cwprep` vs. Tableau Agent (Prep)。突出 cwprep 对 Join、Union 和 SQL 翻译的独家支持。

### 5. cwtwb：Tableau 工作簿工程化
- **架构设计**：工作簿编排器、布局引擎与图表配方引擎。
- **核心能力**：完整的仪表板编排、声明式布局、XSD 结构校验。
- **方案对比**：`cwtwb` vs. Tableau Agent (Web)。突出 cwtwb 在复杂仪表板构建和离线自动化方面的优势。

### 6. 未来愿景：datacooper.com
- 从本地脚本向在线 BI 工作台的演进。
- 现有原型：布局解析工具与 KPI 快速克隆。

### 7. 快速上手
- 安装方式与 MCP 服务器启动指令。
- 开源社区与反馈渠道。

---

## How to Preview

```bash
# Preview Chinese Version
npm run dev

# Preview English Version
npm run dev:en
```
