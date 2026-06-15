# Datacooper TUG Sharing — Speech Script (EN)

> Duration: 30 min talk + 10 min Q&A
> Includes 4 video demos — keep narration short during playback

---

## 【P1】Title Page

Hi everyone. Today I want to talk about one idea: moving from manual dragging to engineering BI.

I will cover three things: cwprep, cwtwb, and datacooper.com.

Let me show you what we will go through today.

## 【P2】Agenda

Four parts today.

Part one: background and positioning — why these tools exist and who they are for.

Part two: cwprep — the Prep flow engine.

Part three: cwtwb — the workbook engineering tool.

Part four: datacooper.com and how to get started.

Let me start with a quick note on what these tools are — and what they are not.

## 【P3】Positioning

These Python tools are **not** here to replace BI developers. They are not trying to turn analysts into programmers.

The goal is simple: **help you work faster**. Give the repetitive, rule-based tasks to tools, so you can spend your time on what matters — understanding the business and making good decisions.

## 【P4】Tableau's Position in the Data Analytics Lifecycle

Before we go deeper, let me quickly show where Tableau fits in the data workflow.

Five steps: data ingestion, data prep, Tableau modeling and visualization, distribution, and feedback.

Our tools focus on two steps. cwprep works on **data prep**. cwtwb works on **Tableau generation**. Tableau itself stays in the middle, handling the analysis.

## 【P5】Why Build These Tools?

So why did we build these tools?

## 【P6】The Pain of Manual Labor

If you look at daily Tableau work, the biggest time sink is not "drawing a chart." It is doing the same tasks over and over.

Dragging fields again. Adjusting layouts again. Copying KPI modules again. Migrating workbooks again. Checking if files open — again. Fixing small but slow problems — again and again.

None of these are hard. But they share one problem: **they don't create new value, but they keep eating your time.**

## 【P7】Paradigm Shift & Quick Demo

This slide shows the old way vs. the new way.

On the left, the **manual way**: 300+ mouse clicks, binary .twb files you can't reuse, full re-dragging for every change, logic hidden in the GUI.

On the right, the **engineering way**: one command to generate, plain-text config for Git, modular parts you can swap fast, code that is also documentation.

Let me show you two quick demos.

> 【Play Video 1: Zero Barrier Text-to-Flow】

This first one shows how fast it is — just say what you want, and the system makes a Prep flow file in seconds.

> 【Play Video 2: Complex Logic Parsing】

The second one is harder. The Agent reads a multi-table description and turns it into a full data pipeline.

## 【P8】Who Is This For?

So who can use these tools? Three groups.

First, **Tableau analysts** — less dragging and copying, more time for real analysis.

Second, **data engineers and IT** — automation, version control, batch deployment. BI becomes part of the engineering workflow.

Third, **team leads and managers** — auditable, repeatable results. Less risk when someone leaves the team.

## 【P9】cwprep

Now let's talk about the first tool: cwprep.

## 【P10】cwprep: One Sentence Intro

One sentence: **give it one sentence, get a working Tableau Prep .tfl / .tflx file.**

Four key features. Text-to-PrepFlow — describe your data logic in plain English. MCP Integration — works with Claude, Gemini, Cursor. No GUI needed — build flows without opening Tableau Prep. Auditable — translate flows to SQL for your DBA to review.

Under the hood: 22 flow operations, 4 databases, SQL translation, TFLX packaging.

Core value: cwprep handles "how data flows", cwtwb handles "how dashboards are built". Speed, consistency, and teamwork.

## 【P11】cwprep Architecture

Let's look at the architecture. It is built in layers.

On top, the interface layer. Left side: MCP Server — works with Claude, Cursor, VSCode, Gemini. Right side: Python Library — import and write scripts directly.

In the middle, the core engine: TFLBuilder, TFLPackager, SQLTranslator, and ExpressionTranslator.

Below that, the operations layer. Three groups: Data Sources — MySQL, PostgreSQL, SQL Server, Excel, CSV. Transformations — Join, Union, Filter, Rename, Calculation, Pivot, and more. Analytics and Output — Aggregate, Unpivot, SQL Translation, TFLX Packaging.

At the bottom, validation and packaging. The output is .tfl or .tflx.

One key part: the **SQL Translator**. In many BI projects, the real problem is not "can you do it" — it is "can you explain it, audit it, show it to your DBA." SQL translation solves that.

## 【P12】cwprep vs Tableau Agent

I know many of you are thinking: doesn't Tableau already have an Agent?

Yes, but here is the difference.

Tableau Agent is closed-source. It only works on Tableau Cloud. And it **does not support Join or Union**. No SQL export either.

cwprep is open-source. Run it anywhere — local, cloud, any setup. It supports Join, Union, and Pivot. And it can translate your whole flow into SQL.

Bottom line: what the official Agent can do, cwprep can do too. What the official Agent cannot do — Join, Union, SQL — cwprep can do. Feature coverage is 88%.

## 【P13】cwprep Typical Cases & Quick Demo

Two real cases. Let's watch the demos.

**Case 1: Zero barrier.** You don't need Tableau Prep installed. Just describe your cleaning logic, send it to the Agent, and get a .tfl file in seconds.

**Case 2: Complex logic.** The Agent reads a description across multiple tables — orders, returns, customers — finds the relationships, and builds the right Join logic.

> 【Play Video 3: Seconds Response — Text-to-Flow】

Fast response in a simple case. Now the second one.

> 【Play Video 4: Deep Parsing — Multi-table Logic】

Even with complex multi-table logic, the Agent produces accurate Prep flows.

## 【P14】cwtwb

Now the second tool: cwtwb.

If cwprep handles "how data flows," then cwtwb handles "how dashboards are built."

## 【P15】cwtwb Architecture

Let's look at the architecture. Same layered design.

Interface layer: MCP Server on the left — works with Claude, Cursor, VSCode, Claude Code. Python Library on the right — import TWBEditor and start coding.

Core engine: TWBEditor, made of four Mixins. ParametersMixin for parameters, ConnectionsMixin for data connections, ChartsMixin for charts, DashboardsMixin for dashboards.

Three subsystems below. Chart Builders — Basic, DualAxis, Pie, Text, Map, Recipes. Dashboard System — layouts, actions, dependencies. Analysis and Migration — migration tools, analyzer, capability registry.

At the bottom, XML Engine based on lxml. Template goes through patch, validate, save — output is .twb or .twbx.

## 【P16】cwtwb vs Tableau Agent (Web)

Let me compare again — this time with Tableau Agent on the Web.

The Web Agent can only make worksheets. No full dashboards. No formatting. No parameters or sets. No data modeling.

cwtwb can do **full dashboard orchestration**, **declarative layout and formatting**, **cross-source migration**, and **XSD validation with versioning**.

cwtwb fills the gaps the official Agent leaves open — complex layouts and automated production.

## 【P17】cwtwb: One Sentence Intro

One sentence: **dashboards that take hours to drag-and-drop — AI builds from scratch in one prompt. cwtwb makes every Tableau user 10× faster.**

Four features: Generate — build TWB from code or agent calls. Validate — structural and XSD validation. Migrate — quickly move to new data sources. Orchestrate — chart and layout orchestration.

15+ chart types, 50+ MCP tools. Three core values: deterministic output, verifiable delivery, ready for migration.

## 【P18】cwtwb Cases & Closed-loop Demo

Two more real cases.

**Case 3: AI dashboard generation via MCP.** Just configure the MCP server with your data source and template, describe what you need, and AI auto-plans the layout and generates a Tableau file. Zero code — plain language in, .twb out.

**Case 4: End-to-end live rendering.** From a raw document to a working Tableau dashboard. You can watch the dashboard appear in real time — like hot-reloading a dashboard.

> 【Play Video 5: AI Dashboard Generation via MCP】

> 【Play Video 6: Dashboard Live Rendering】

## 【P19】datacooper.com

Last part: datacooper.com.

If cwprep and cwtwb are the core capabilities, then datacooper.com is where we turn them into tools anyone can use — online.

## 【P20】datacooper Online Tool Prototypes

The direction is simple: not just local scripts, but an online platform. All powered by the same Python SDK.

Two working prototypes so far.

First: **layout parsing**. Upload a workbook, it pulls out the dashboard structure, exports as JSON.

Second: **KPI cloning**. Copy a KPI worksheet, swap only the metric, keep everything else. This is very useful in real work, because you rarely build a KPI from scratch. You copy a proven template and just change one number.

Further out: collaboration and version management — a direction we are thinking about, not a current promise.

## 【P21】Try It Out

Both tools are on PyPI. One line to install:

```
pip install cwprep cwtwb
```

MCP servers have their own commands: cwprep-mcp and cwtwb-mcp.

Source code is on GitHub. Docs and online tools are at datacooper.com. Open source under AGPL-3.0. Please star, try it, and give us feedback.

## 【P22】Acknowledgments

Before I finish, I want to thank some people who helped me a lot on this journey.

Patrick Therriault — for guiding me deeper into the Tableau community. Andy Cotgreave — for the insights that pushed this project forward. Adam Mico — for your patience and solid advice. Jeffrey Shaffer — the skills you suggested became very useful process constraints. Matthew Miller, Elif Tutuk, Paul Morgan, Olga L. — for the useful hints from an official perspective. Li-Lun Tu — for suggestions on building a brand. Alex Mou — for your encouragement and the advice in our conversations.

And everyone who left a comment or joined the discussion to keep me on the right track — thank you all.

## 【P23】Closing

I will leave you with one sentence:

**Don't leave Tableau. Let AI give time back to humans.**

## 【P24】Q&A / Discussion

That's the end of the formal part. Any questions or topics you want to talk about? Let's discuss.

> 【Q&A, about 10 minutes】

Thank you.
