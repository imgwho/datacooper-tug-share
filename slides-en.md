---
theme: seriph
title: Datacooper TUG Share (EN)
info: |
  Tableau User Group Sharing
  cwprep · cwtwb · datacooper.com
class: text-left
transition: fade
drawings:
  persist: false
mdc: true
background: "#e9e6dc"
---

<div class="min-h-[86vh] px-8 py-10 md:px-16">
  <div class="mx-auto flex min-h-[86vh] max-w-[1180px] items-start pt-6 md:pt-10">
    <div v-motion :initial="{ opacity: 0, y: 100 }" :enter="{ opacity: 1, y: 0 }" class="w-full rounded-[40px] border border-primary/50 
        bg-[radial-gradient(circle_at_top_right,oklch(61.71%_.1375_39.0427_/_0.12),transparent_36%),radial-gradient(circle_at_bottom_left,rgba(233,230,220,0.8),transparent_30%),rgba(255,255,255,0.5)] px-8 py-10 shadow-sm md:px-12 md:py-14">
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-xs font-semibold uppercase tracking-[0.22em] text-primary shadow-sm">
        Datacooper · Tableau User Group Sharing
      </div>
      <h1 class="mt-6 max-w-5xl text-5xl font-black tracking-[-0.05em] leading-[0.94] text-primary md:text-7xl">
        From Manual Dragging to Engineering BI
      </h1>
      <p class="mt-6 max-w-4xl text-lg leading-8 text-muted-foreground md:text-2xl md:leading-relaxed">
        <strong class="text-foreground">cwprep</strong> automates Tableau Prep flows, 
        <strong class="text-foreground">cwtwb</strong> handles engineering generation of Tableau Workbooks, 
        <strong class="text-foreground">datacooper.com</strong> builds these into user-friendly online tools.
      </p>
      <div class="mt-8 flex flex-wrap gap-3">
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">Python Tools = BI Development Accelerator</span>
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">MCP</span>
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">Repeatable</span>
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">Auditable</span>
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">Migratable</span>
      </div>
    </div>
  </div>
</div>

---
layout: fact
---

# Positioning of Python Tools

## Accelerating the BI Development Process

<div class="mt-6 max-w-4xl text-lg leading-8 text-muted-foreground">
  Not replacing BI developers, but handing over repetitive, mechanical, and rule-based tasks to tools.
</div>

---
layout: center
class: text-center
---

# Tableau's Position in the Data Analytics Lifecycle

<div class="mx-auto mt-8 grid max-w-6xl gap-4 md:grid-cols-5">
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">1. Data Ingestion</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">DB, Excel, CSV, API</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">2. Data Prep</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">Clean, Transform, Join, Agg</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">3. Tableau</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">Modeling, Calc, Layout, Viz</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">4. Distribution</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">Publish, Review, Iterate</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">5. Optimization</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">Revise Data, Adjust Design</div>
  </div>
</div>

<div class="mx-auto mt-7 max-w-4xl rounded-[24px] border border-primary/50 bg-white/50 px-6 py-4 text-base leading-7 text-foreground shadow-sm">
  cwprep focuses on "Data Prep", cwtwb focuses on "Tableau Generation & Orchestration", with Tableau serving as the analytic expression.
</div>

---
layout: section
---

# Why Build These Tools?

---
layout: center
class: text-center
---

<div class="mx-auto max-w-5xl">
  <div class="rounded-[28px] border border-primary/50 bg-white/50 px-8 py-7 text-lg leading-8 text-muted-foreground shadow-sm">
    The most time-consuming part in Tableau isn't "drawing a chart," but doing these mechanical tasks repeatedly.
  </div>

  <div class="mt-6 grid gap-4 md:grid-cols-2">
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly dragging fields</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly adjusting layouts</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly copying KPI modules</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly migrating workbooks</div>
  </div>

  <div class="mt-6 rounded-[24px] border border-primary/50 bg-white/50 px-6 py-5 text-base leading-7 text-foreground shadow-sm">
    None of these are difficult alone, but they add no new business value while consuming development time.
  </div>
</div>

---
layout: center
---

# Paradigm Shift in Development

<div class="grid grid-cols-2 gap-10 mt-10 text-left">
  <div v-click class="p-8 border border-primary/50 rounded-[32px] bg-white/50 shadow-sm">
    <h3 class="text-2xl font-bold mb-6 text-foreground">Manual Approach</h3>
    <ul class="space-y-4 text-muted-foreground text-lg">
      <li class="flex items-start gap-3"><span>❌</span> <span>300+ repetitive mouse clicks</span></li>
      <li class="flex items-start gap-3"><span>❌</span> <span>Non-reusable binary .twb files</span></li>
      <li class="flex items-start gap-3"><span>❌</span> <span>Full re-dragging for changes</span></li>
      <li class="flex items-start gap-3"><span>❌</span> <span>Logic hidden deep in GUI, non-auditable</span></li>
    </ul>
  </div>
  
  <div v-click class="p-8 border border-primary/50 rounded-[32px] bg-white/50 shadow-md">
    <h3 class="text-2xl font-bold mb-6 text-primary">Engineering Approach</h3>
    <ul class="space-y-4 text-foreground font-medium text-lg">
      <li class="flex items-start gap-3"><span>✅</span> <span>Single command/prompt generation</span></li>
      <li class="flex items-start gap-3"><span>✅</span> <span>Plain-text config, Git-friendly</span></li>
      <li class="flex items-start gap-3"><span>✅</span> <span>Modular components, rapid swapping</span></li>
      <li class="flex items-start gap-3"><span>✅</span> <span>Code is documentation, fully traceable</span></li>
    </ul>
  </div>
</div>

---
layout: section
---

# cwprep

---
layout: center
class: text-center
---

# cwprep Architecture

<div class="big-diagram mt-10 mb-10">

```mermaid
flowchart LR
  A["Natural Language / MCP"] --> B["Planner"]
  C["DB / Excel / CSV"] --> B
  B --> D["Flow Builder"]
  D --> E["Validator"]
  D --> F["SQL Translator"]
  E --> G[".tfl / .tflx"]
  F --> G
  G --> H["Auditable / Reusable / Shareable"]
```

</div>

---
layout: default
---

## cwprep

### One Prompt

Input one sentence, output a usable Tableau Prep `.tfl` / `.tflx` file.

### What it can do

- Text-to-PrepFlow: Describe data logic in natural language
- MCP Integration: Works with Claude, Gemini, Cursor
- Avoid GUI Dependency: Build flows without opening Tableau Prep
- Auditable: Translates flows to SQL for DBA/Compliance review

---
layout: center
class: text-center
---

# cwprep Typical Use Cases

<div class="mx-auto mt-8 grid max-w-6xl gap-4 md:grid-cols-2">
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">Data Joining & Merging</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Automating multi-source Join logic.</p>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">Automated Data Cleaning</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Type conversion and filtering based on business rules.</p>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">Metric Aggregation</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Preprocessing complex business metrics at the Prep layer.</p>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">End-to-End Automation</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">From raw data to TFLX file generation.</p>
  </div>
</div>

---
layout: fact
---

# The Value of cwprep

## Turning Prep flow creation into an engineering action

---
layout: center
class: text-center
---

<div class="mx-auto grid max-w-6xl gap-4 md:grid-cols-3">
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">Efficiency</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Automates repetitive Prep flow building.</p>
  </div>
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">Stability</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Solidifies common rules, reducing human error.</p>
  </div>
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">Collaboration</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Brings data cleaning into scripts and version control.</p>
  </div>
</div>

---
layout: section
---

# cwtwb

---
layout: center
class: text-center
---

# cwtwb Architecture

<div class="big-diagram mt-10 mb-10">

```mermaid
flowchart LR
  A["Prompt / Existing TWB / Layout JSON"] --> B["Workbook Composer"]
  A --> C["Chart Recipe Engine"]
  A --> D["Layout Engine"]
  B --> E["Worksheet Refactor / Migration"]
  C --> E
  D --> E
  E --> F["Validation"]
  F --> G[".twb / .twbx"]
  G --> H["Repeatable / Verifiable / Migratable"]
```

</div>

---
layout: default
---

<div class="grid min-h-[78vh] grid-cols-1 gap-8" style="grid-template-columns: 1.05fr 0.95fr">
  <div class="flex flex-col justify-between">
    <div>
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
        One Goal
      </div>
      <h2 class="mt-4 text-4xl font-black tracking-[-0.04em] text-foreground md:text-5xl">
        Turning Tableau workbooks into repeatable, verifiable, and migratable assets.
      </h2>
    </div>
    <div class="mt-8 grid gap-3 md:grid-cols-2">
      <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">Generation</div>
        <div class="mt-1 leading-6 text-muted-foreground">Generate TWB from code or agent calls.</div>
      </div>
      <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">Validation</div>
        <div class="mt-1 leading-6 text-muted-foreground">Structural + XSD validation.</div>
      </div>
      <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">Migration</div>
        <div class="mt-1 leading-6 text-muted-foreground">Rapidly migrate to new data sources.</div>
      </div>
      <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">Orchestration</div>
        <div class="mt-1 leading-6 text-muted-foreground">Manage Charts and Layouts.</div>
      </div>
    </div>
  </div>
  <div class="rounded-[28px] border border-primary/50 bg-white/50 p-7 shadow-sm">
    <div class="inline-flex items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
      Key Difference
    </div>
    <p class="mt-5 text-lg leading-8 text-muted-foreground">
      cwprep manages "How data flows",<br>
      cwtwb manages "How dashboards are built".
    </p>
    <div class="mt-6 grid gap-3 md:grid-cols-2">
      <div class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 text-sm text-foreground shadow-sm">Repeatable</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 text-sm text-foreground shadow-sm">Verifiable</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 text-sm text-foreground shadow-sm">Migratable</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 text-sm text-foreground shadow-sm">Orchestrable</div>
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

<div class="mx-auto grid max-w-6xl gap-6 md:grid-cols-[1.1fr_0.9fr]">
  <div class="flex items-start justify-center text-left">
    <div>
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
        Core Positioning
      </div>
      <h2 class="mt-4 max-w-xl text-4xl font-black tracking-[-0.04em] leading-[1.1] text-foreground md:text-5xl">
        Workbook engineering layer.
      </h2>
      <p class="mt-5 max-w-lg text-lg leading-8 text-muted-foreground">
        Turning workbook generation, validation, migration, and refactoring into repeatable engineering tasks.
      </p>
    </div>
  </div>

  <div class="rounded-[28px] border border-primary/50 bg-white/50 p-7 text-left shadow-sm">
    <div class="inline-flex items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
      Core Value
    </div>
    <div class="mt-6 grid gap-4">
      <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
        <div class="text-base font-semibold text-primary">Deterministic Output</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">Stable and repeatable results.</div>
      </div>
      <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
        <div class="text-base font-semibold text-primary">Verifiable Delivery</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">Inspectable and openable files.</div>
      </div>
      <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
        <div class="text-base font-semibold text-primary">Migration Friendly</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">No need to rebuild from scratch.</div>
      </div>
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

# Typical cwtwb Use Cases

<div class="mx-auto mt-8 grid max-w-6xl gap-4 md:grid-cols-2">
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">End-to-End Automation</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Generate complete TWBX files with one click.</p>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">Local Sheet Refactoring</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Replace specific KPI metrics while keeping layout intact.</p>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">Cross-Env Source Migration</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Rapidly adapt to Dev/Prod data source changes.</p>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">Declarative Layout Management</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">Define layouts in JSON to batch produce dashboards.</p>
  </div>
</div>

---
layout: section
---

# datacooper.com

---
layout: default
---

<div class="grid min-h-[78vh] grid-cols-1 gap-8" style="grid-template-columns: 1.05fr 0.95fr">
  <div class="flex flex-col justify-between">
    <div>
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
        Future Direction
      </div>
      <h2 class="mt-4 text-4xl font-black tracking-[-0.04em] text-foreground md:text-5xl">
        Building an online platform, not just local scripts.
      </h2>
      <p class="mt-5 max-w-xl text-base leading-7 text-muted-foreground md:text-lg">
        Not just wrapping commands in a UI, but turning BI tasks into a natural online workflow.
        Powered by our Python SDK under the hood.
      </p>
    </div>
    <div class="mt-8 grid grid-cols-2 gap-3">
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm leading-6 shadow-sm">Online Access</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm leading-6 shadow-sm">Direct File Processing</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm leading-6 shadow-sm">Low Entry Barrier</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm leading-6 shadow-sm">Code-to-Tool Transformation</div>
    </div>
    <div class="mt-6 rounded-[24px] border border-dashed border-primary/50 bg-white/50 p-5 shadow-sm">
      <div class="text-sm font-semibold text-primary">The Intuitive Workflow</div>
      <div class="mt-3 flex flex-wrap gap-2 text-sm text-foreground">
        <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1">Upload</span>
        <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1">Parse</span>
        <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1">Preview</span>
        <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1">Adjust</span>
        <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1">Export</span>
      </div>
    </div>
    <div class="mt-4 text-sm leading-6 text-muted-foreground">
      Focusing on natural BI workflows rather than just exposing SDK functions.
    </div>
  </div>
  <div class="rounded-[28px] border border-primary/50 bg-white/50 p-7 shadow-sm">
    <div class="inline-flex items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
      Available Prototypes
    </div>
    <div class="mt-4 text-sm leading-6 text-muted-foreground">
      Current tools already cover two practical directions for platform evolution.
    </div>
    <div class="mt-6 space-y-4">
      <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm">
        <div class="text-sm font-semibold text-primary">Layout Parsing</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">Extracting dashboard structures and exporting to JSON.</div>
      </div>
      <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm">
        <div class="text-sm font-semibold text-primary">KPI Cloning</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">Cloning KPI sheets with metric swapping while preserving styles.</div>
      </div>
    </div>
    <div class="mt-6 rounded-[20px] border border-dashed border-primary/50 bg-white/50 px-5 py-4">
      <div class="text-sm font-semibold text-primary">Long-term Vision</div>
      <div class="mt-2 text-sm leading-6 text-muted-foreground">
        Collaboration and version management are conceptual directions for future growth.
      </div>
    </div>
  </div>
</div>

---
layout: quote
---

# Transforming Tableau development from craftsmanship into an engineering workflow.
