# Datacooper TUG Sharing — Speech Script (EN)

> Duration: 30 min talk + 10 min Q&A
> Includes 4 video demos — keep narration short during playback

---

## 【P1】Title Page

Hi everyone. Today I want to talk about one idea: moving from manual dragging to engineering BI.

I will cover three things: cwprep, cwtwb, and datacooper.com.

Let me start with a quick note on what these tools are — and what they are not.

## 【P2】Positioning

These Python tools are **not** here to replace BI developers. They are not trying to turn analysts into programmers.

The goal is simple: **help you work faster**. Hand over the repetitive, rule-based tasks to tools, so you can spend your time on what matters — understanding the business and making good decisions.

## 【P3】Tableau's Position in the Data Analytics Lifecycle

Before we go deeper, let me quickly show where Tableau fits in the data workflow.

There are five steps: data ingestion, data prep, Tableau modeling and visualization, distribution, and optimization.

Our tools focus on two steps. cwprep works on **data prep**. cwtwb works on **Tableau generation and orchestration**. Tableau itself stays in the middle, handling the analysis and expression.

## 【P4】Why Build These Tools?

So why did we build these tools?

## 【P5】The Pain of Manual Labor

If you look at day-to-day Tableau work, the biggest time sink is not "drawing a chart." It is doing the same mechanical tasks over and over.

Dragging fields again. Adjusting layouts again. Copying KPI modules again. Migrating workbooks again. Checking if files open correctly — again. Fixing small but time-consuming issues — again and again.

None of these are hard on their own. But they share one problem: **they don't create new business value, yet they keep eating up your time.**

## 【P6】Paradigm Shift & Quick Demo

This slide shows the difference between the old way and the new way.

On the left, the **manual approach**: 300+ mouse clicks, binary .twb files you can't reuse, full re-dragging for every change, and logic hidden deep in the GUI.

On the right, the **engineering approach**: one command to generate, plain-text config you can put in Git, modular components you can swap in seconds, and code that serves as documentation.

Now let me show you two quick demos.

> 【Play Video 1: Zero Barrier Text-to-Flow】

This first one shows how fast it is — just describe what you want, and the system generates a Prep flow file in seconds.

> 【Play Video 2: Complex Logic Parsing】

The second one is more complex. The Agent reads a multi-table business description and turns it into a complete data pipeline.

## 【P7】Who Is This For?

So who can benefit from these tools? Three groups.

First, **Tableau analysts** — less dragging and copying, more time for real analysis.

Second, **data engineers and IT** — automation, version control, batch deployment. BI becomes part of the engineering workflow.

Third, **team leads and managers** — auditable, repeatable deliverables. Less risk when someone leaves the team.

## 【P8】cwprep

Now let's talk about the first tool: cwprep.

## 【P9】cwprep Architecture

cwprep is basically a text-to-PrepFlow engine.

You give it a sentence, it gives you a working Tableau Prep flow file.

Look at the architecture. On the left, the input can be natural language or an MCP call. MCP is an open protocol for AI tools — think of it as a USB port for AI. It works with Claude, Gemini, Cursor, and other clients.

The input goes through a Planner, then a Flow Builder, then a Validator. The output is a .tfl or .tflx file.

There is also a **SQL Translator**. This is very important. It can turn your Prep flow into SQL, so your DBA or compliance team can read and review it.

## 【P10】cwprep vs Tableau Agent

I know many of you are thinking: doesn't Tableau already have an Agent?

Yes, but here is the difference.

Tableau Agent is a closed-source product. It only works on Tableau Cloud. And it **does not support Join or Union**. It also cannot export SQL.

cwprep is open-source. You can run it anywhere — local, cloud, any environment. It supports Join, Union, and Pivot. And it can translate your entire flow into SQL.

In short: what the official Agent can do, cwprep can also do. What the official Agent cannot do — Join, Union, SQL translation — cwprep can do those too.

## 【P11】cwprep Typical Cases & Quick Demo

Let me show you two real cases.

**Case 1: Zero barrier generation.** You don't even need Tableau Prep installed locally. Just describe your cleaning logic in plain English, send it to the Agent, and you get a .tfl file in seconds. That's Text-to-Flow.

**Case 2: Complex multi-table logic.** The Agent reads a description that spans multiple tables — orders, returns, customers — understands the relationships, and generates the correct Join logic, aggregations, and filters.

Let's watch the demos.

> 【Play Video 3: Seconds Response — Text-to-Flow】

> 【Play Video 4: Deep Parsing — Multi-table Logic】

As you can see, even with complex scenarios, the Agent produces accurate, complete Prep flows.

## 【P12】cwtwb

Now the second tool: cwtwb.

If cwprep handles "how data flows," then cwtwb handles "how dashboards are built."

## 【P13】cwtwb Architecture

Look at the architecture. The input can be natural language, an existing TWB file, or layout JSON.

There are three core engines: Workbook Composer for overall structure, Chart Recipe Engine for charts, and Layout Engine for dashboard layout.

All outputs go through **worksheet refactoring and migration**, then through **validation** — both structural and Tableau XSD validation. The final output is a .twb or .twbx file.

The key words at the end: **repeatable, verifiable, migratable**.

## 【P14】cwtwb vs Tableau Agent (Web)

Again, let me compare with the official tool — this time, Tableau Agent on the Web.

The Web Agent can only create individual worksheets. It cannot build full dashboards. It does not support advanced formatting or parameters and sets.

cwtwb can do **full dashboard orchestration**, **declarative layout and formatting**, and **XSD validation with versioning**.

Basically, cwtwb fills the gaps that the official Agent leaves open — complex layouts and automated production.

## 【P15】cwtwb: One Sentence Intro

If I had to describe cwtwb in one sentence, it would be:

**Turn Tableau workbooks into repeatable, verifiable, and migratable engineering assets.**

Two key features: deterministic output — you get the same result every time, no manual errors. And verifiable delivery — structural and XSD validation ensures the file actually works.

The core idea: cwprep manages data flows, cwtwb manages dashboard generation. Together, they bring BI into scripts, version control, and batch production.

## 【P16】cwtwb Cases & Closed-loop Demo

Two more real cases.

**Case 3: Declarative code with auto-fix.** This shows the 4-step Python workflow: the AI reads your database schema, generates code, runs the script, and — here's the interesting part — **automatically fixes bugs**. In the demo, it catches and corrects a case-sensitive filter error on its own.

**Case 4: End-to-end live dashboard rendering.** From a raw document to a working Tableau dashboard. You can watch the dashboard appear in real time, from nothing to a complete view. It's like hot-reloading a dashboard.

Let's watch.

> 【Play Video 5: Python Practice & Auto Bug Fix】

> 【Play Video 6: Dashboard Live Rendering】

## 【P17】datacooper.com

Last part: datacooper.com.

If cwprep and cwtwb are the core capabilities, then datacooper.com is where we turn them into tools that anyone can use — online.

## 【P18】datacooper Online Tool Prototypes

The direction is simple: not just local scripts, but an online platform.

We already have two working prototypes.

The first is **layout parsing**. Upload a workbook, and it extracts the dashboard structure and exports it as JSON.

The second is **KPI cloning**. Copy a KPI worksheet, swap only the metric, and keep everything else — the layout, the formatting, the structure. This is very useful in real BI work, because you rarely build a KPI from scratch. You usually copy a proven template and just change one number. This avoids the problems you get with Replace References.

The long-term plan: turn common Tableau tasks into an online BI toolbox.

## 【P19】Try It Out

Both tools are on PyPI. One line to install:

```
pip install cwprep cwtwb
```

MCP servers also have their own commands: cwprep-mcp and cwtwb-mcp.

Source code is on GitHub. Documentation and online tools are at datacooper.com. Everything is open source under AGPL-3.0. Feel free to star, try it out, and give us feedback.

## 【P20】Q&A / Discussion

That's the end of the formal part. Let's open it up — any questions or topics you'd like to discuss?

> 【Q&A, about 10 minutes】

## 【P21】Closing

I'll leave you with one sentence:

**Don't leave Tableau. Let AI give time back to humans.**

Thank you.
