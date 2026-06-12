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

<div class="min-h-[80vh] px-8 py-6 md:px-16">
  <div class="mx-auto flex min-h-[80vh] max-w-[1180px] items-start pt-4 md:pt-6">
    <div v-motion :initial="{ opacity: 0, y: 100 }" :enter="{ opacity: 1, y: 0 }" class="w-full rounded-[40px] border border-primary/50 
        bg-[radial-gradient(circle_at_top_right,oklch(61.71%_.1375_39.0427_/_0.12),transparent_36%),radial-gradient(circle_at_bottom_left,rgba(233,230,220,0.8),transparent_30%),rgba(255,255,255,0.5)] px-8 py-8 shadow-sm md:px-12 md:py-10">
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-xs font-semibold uppercase tracking-[0.22em] text-primary shadow-sm">
        Datacooper · Tableau User Group Sharing
      </div>
      <h1 class="mt-4 max-w-5xl text-5xl font-black tracking-[-0.05em] leading-[0.94] text-primary md:text-6xl">
        From Manual Dragging to Engineering BI
      </h1>
      <p class="mt-4 max-w-4xl text-base leading-7 text-muted-foreground md:text-xl md:leading-relaxed">
        <strong class="text-foreground">cwprep</strong> automates Tableau Prep flows, 
        <strong class="text-foreground">cwtwb</strong> handles engineering generation of Tableau Workbooks, 
        <strong class="text-foreground">datacooper.com</strong> builds these into user-friendly online tools.
      </p>
      <div class="mt-6 flex flex-wrap gap-2">
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">cwtwb/cwprep = BI Development Accelerator</span>
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

# Positioning of cwtwb/cwprep

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

# The Pain of Manual Labor

<div class="mx-auto max-w-5xl">
  <div class="rounded-[28px] border border-primary/50 bg-white/50 px-8 py-7 text-lg leading-8 text-muted-foreground shadow-sm">
    The most time-consuming part in Tableau isn't "drawing a chart," but doing these mechanical tasks repeatedly.
  </div>

  <div class="mt-6 grid gap-4 md:grid-cols-3">
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly dragging fields</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly adjusting layouts</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly copying KPI modules</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly migrating workbooks</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly checking if files open correctly</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">Repeatedly fixing small issues</div>
  </div>

  <div class="mt-6 rounded-[24px] border border-primary/50 bg-white/50 px-6 py-5 text-base leading-7 text-foreground shadow-sm text-center">
    None of these are difficult alone, but they add no new business value while consuming development time.
  </div>
</div>

---
layout: center
---

# Paradigm Shift & Quick Generation Demo

<div class="grid grid-cols-2 gap-4 mt-4 text-left">
  <!-- Left: Paradigm Comparison -->
  <div class="space-y-4">
    <div class="p-4 border border-primary/50 rounded-[24px] bg-white/50 shadow-sm">
      <h3 class="text-xl font-bold mb-3 text-foreground">Manual (Traditional)</h3>
      <ul class="space-y-2 text-muted-foreground text-sm">
        <li>❌ 300+ repetitive mouse clicks</li>
        <li>❌ Non-reusable binary .twb files</li>
        <li>❌ Full re-dragging for changes</li>
        <li>❌ Logic hidden in GUI, non-auditable</li>
      </ul>
    </div>
    <div class="p-4 border border-primary/50 rounded-[24px] bg-white/50 shadow-md">
      <h3 class="text-xl font-bold mb-3 text-primary">Engineering (Modern)</h3>
      <ul class="space-y-2 text-foreground font-medium text-sm">
        <li>✅ Single command/prompt generation</li>
        <li>✅ Plain-text config, Git-friendly</li>
        <li>✅ Modular components, rapid swapping</li>
        <li>✅ Code is documentation, fully traceable</li>
      </ul>
    </div>
  </div>

  <!-- Right: Video Demos -->
  <div class="space-y-4">
    <div class="rounded-xl border border-primary/30 bg-white/50 p-3 shadow-sm">
      <div class="aspect-video rounded-lg overflow-hidden bg-black mb-2">
        <Youtube id="b7WrC0ngqwk" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs">Zero Barrier Text-to-Flow</h4>
    </div>
    <div class="rounded-xl border border-primary/30 bg-white/50 p-3 shadow-sm">
      <div class="aspect-video rounded-lg overflow-hidden bg-black mb-2">
        <Youtube id="4RMevXQObkE" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs">Agent Complex Logic Parsing</h4>
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

# Who Is This For?

<div class="mx-auto mt-8 grid max-w-5xl gap-4 md:grid-cols-3">
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="mt-2 text-lg font-bold text-foreground">Tableau Analysts</h3>
    <p class="mt-2 text-sm leading-6 text-muted-foreground">Less repetitive dragging and copying — more time for insights and business judgment.</p>
  </div>
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="mt-2 text-lg font-bold text-foreground">Data Engineering / IT</h3>
    <p class="mt-2 text-sm leading-6 text-muted-foreground">Automation, version control, and batch deployment — bringing BI into engineering workflows.</p>
  </div>
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="mt-2 text-lg font-bold text-foreground">Team Leads / Managers</h3>
    <p class="mt-2 text-sm leading-6 text-muted-foreground">Auditable, repeatable deliverables — reducing key-person dependency and knowledge loss.</p>
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
layout: center
class: text-center
---

# cwprep vs Tableau Agent

<div class="mx-auto mt-4 grid max-w-5xl gap-4 md:grid-cols-[1fr_auto_1fr]">
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-lg font-bold text-foreground">Tableau Agent</h3>
    <ul class="mt-3 space-y-2 text-sm leading-6 text-muted-foreground">
      <li>Closed-source, official product</li>
      <li>Natural language driven Prep flows</li>
      <li>Tableau Cloud only</li>
      <li>No Join / Union support</li>
      <li>No SQL export</li>
    </ul>
  </div>
  <div class="flex items-center justify-center">
    <div class="text-2xl font-black text-primary">VS</div>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-md">
    <h3 class="text-lg font-bold text-primary">cwprep</h3>
    <ul class="mt-3 space-y-2 text-sm leading-6 text-foreground font-medium">
      <li>Open-source, self-hosted</li>
      <li>Natural language + code dual mode</li>
      <li>Any environment</li>
      <li class="text-primary font-bold">✅ Join / Union / Pivot</li>
      <li class="text-primary font-bold">✅ Flow → SQL Translation</li>
    </ul>
  </div>
</div>

---
layout: center
---

# cwprep Typical Cases & Quick Demo

<div class="grid grid-cols-2 gap-6 mt-4 text-left">
  <div class="space-y-4">
    <div class="p-6 border border-primary/50 rounded-[28px] bg-white/50 shadow-sm">
      <h3 class="text-xl font-bold mb-3 text-primary">Case 1: Zero Barrier Generation</h3>
      <p class="text-sm leading-relaxed text-muted-foreground">
        No local environment needed. Users send cleaning logic in natural language to the Agent, and the system generates a standard .tfl file in seconds.
      </p>
      <ul class="mt-3 space-y-1 text-xs text-foreground font-medium">
        <li>✅ Text-to-Flow in seconds</li>
        <li>✅ Web-based, lightweight, no install</li>
      </ul>
    </div>
    <div class="p-6 border border-primary/50 rounded-[28px] bg-white/50 shadow-sm">
      <h3 class="text-xl font-bold mb-3 text-primary">Case 2: Complex Logic Parsing</h3>
      <p class="text-sm leading-relaxed text-muted-foreground">
        Agent deeply understands multi-step, cross-table business descriptions (Orders, Returns, Customers) and translates them into data pipelines.
      </p>
      <ul class="mt-3 space-y-1 text-xs text-foreground font-medium">
        <li>✅ Auto-detect ER relations & Joins</li>
        <li>✅ Handle complex aggregations & filters</li>
      </ul>
    </div>
  </div>

  <div class="grid grid-cols-1 gap-4">
    <div class="rounded-2xl border border-primary/30 bg-white/50 p-3 shadow-md">
      <div class="aspect-video rounded-xl overflow-hidden bg-black mb-2">
        <Youtube id="b7WrC0ngqwk" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs text-center">Demo: Seconds Response (Text-to-Flow)</h4>
    </div>
    <div class="rounded-2xl border border-primary/30 bg-white/50 p-3 shadow-md">
      <div class="aspect-video rounded-xl overflow-hidden bg-black mb-2">
        <Youtube id="4RMevXQObkE" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs text-center">Demo: Deep Parsing (Multi-table Logic)</h4>
    </div>
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
  A["Natural Language / TWB / Layout JSON"] --> B["Workbook Composer"]
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
layout: center
class: text-center
---

# cwtwb vs Tableau Agent (Web)

<div class="mx-auto mt-4 grid max-w-5xl gap-4 md:grid-cols-[1fr_auto_1fr]">
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="text-lg font-bold text-foreground">Tableau Agent (Web)</h3>
    <ul class="mt-3 space-y-2 text-sm leading-6 text-muted-foreground">
      <li>Limited to Worksheets only</li>
      <li>Cannot build Dashboards</li>
      <li>No advanced formatting support</li>
      <li>No support for Params/Sets</li>
    </ul>
  </div>
  <div class="flex items-center justify-center">
    <div class="text-2xl font-black text-primary">VS</div>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-md">
    <h3 class="text-lg font-bold text-primary">cwtwb</h3>
    <ul class="mt-3 space-y-2 text-sm leading-6 text-foreground font-medium">
      <li class="text-primary font-bold">✅ Full Dashboard Orchestration</li>
      <li class="text-primary font-bold">✅ Declarative Layout & Formatting</li>
      <li class="text-primary font-bold">✅ XSD Validation & Versioning</li>
    </ul>
  </div>
</div>

---
layout: default
---

# cwtwb: One Sentence Intro

<div class="grid grid-cols-1 gap-4" style="grid-template-columns: 1.05fr 0.95fr">
  <div class="flex flex-col justify-between">
    <h2 class="mt-3 text-3xl font-black tracking-[-0.04em] text-foreground md:text-4xl">
      Turning Tableau workbooks into repeatable, verifiable, and migratable assets.
    </h2>
    <div class="mt-4 grid gap-2 md:grid-cols-2">
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">Deterministic Output</div>
        <div class="mt-1 leading-6 text-muted-foreground">Stable results, no manual error.</div>
      </div>
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">Verifiable Delivery</div>
        <div class="mt-1 leading-6 text-muted-foreground">XSD validation ensures files open.</div>
      </div>
    </div>
  </div>
  <div class="rounded-[28px] border border-primary/50 bg-white/50 p-5 shadow-sm text-sm text-muted-foreground flex flex-col justify-center">
    <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-primary mb-4">
      Core Value
    </div>
    cwprep manages data flows, cwtwb manages dashboard generation. 
    Integrating BI into scripts, version control, and batch production.
  </div>
</div>

---
layout: center
---

# cwtwb Cases & Closed-loop Demo

<div class="grid grid-cols-2 gap-6 mt-4 text-left">
  <div class="space-y-4">
    <div class="p-6 border border-primary/50 rounded-[28px] bg-white/50 shadow-sm">
      <h3 class="text-xl font-bold mb-3 text-primary">Case 3: Declarative Code & Auto Fix</h3>
      <p class="text-sm leading-relaxed text-muted-foreground">
        Python framework demo: Schema awareness, code generation, script execution, and automatic bug fixing.
      </p>
      <ul class="mt-3 space-y-1 text-xs text-foreground font-medium">
        <li>✅ AI perceives DB Schema / ER diagrams</li>
        <li>✅ <strong>Highlight:</strong> Agent auto-fixes case-sensitive filter bugs</li>
      </ul>
    </div>
    <div class="p-6 border border-primary/50 rounded-[28px] bg-white/50 shadow-sm">
      <h3 class="text-xl font-bold mb-3 text-primary">Case 4: End-to-End Live Rendering</h3>
      <p class="text-sm leading-relaxed text-muted-foreground">
        From raw docs to functional Tableau dashboards. Watch the rendering process live in the Tableau client.
      </p>
      <ul class="mt-3 space-y-1 text-xs text-foreground font-medium">
        <li>✅ Full end-to-end automation loop</li>
        <li>✅ "Hot-reload" experience for BI dashboards</li>
      </ul>
    </div>
  </div>

  <div class="grid grid-cols-1 gap-4">
    <div class="rounded-2xl border border-primary/30 bg-white/50 p-3 shadow-md">
      <div class="aspect-video rounded-xl overflow-hidden bg-black mb-2">
        <Youtube id="dNzMbLOEA7A" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs text-center">Demo: Python Practice & Auto Bug Fix</h4>
    </div>
    <div class="rounded-2xl border border-primary/30 bg-white/50 p-3 shadow-md">
      <div class="aspect-video rounded-xl overflow-hidden bg-black mb-2">
        <Youtube id="NMy4__CCCDI" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs text-center">Demo: Dashboard Live Rendering</h4>
    </div>
  </div>
</div>

---
layout: section
---

# datacooper.com

---
layout: default
---

# datacooper Online Tool Prototypes

<div class="grid grid-cols-1 gap-4" style="grid-template-columns: 1.05fr 0.95fr">
  <div class="flex flex-col justify-between">
    <div>
      <h2 class="mt-3 text-3xl font-black tracking-[-0.04em] text-foreground md:text-4xl">
        Building a platform, not just scripts.
      </h2>
    </div>
    <div class="mt-4 grid grid-cols-2 gap-2">
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm shadow-sm">Online Access</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm shadow-sm">Code-to-Tool</div>
    </div>
  </div>
  <div class="rounded-[28px] border border-primary/50 bg-white/50 p-6 shadow-sm">
    <div class="space-y-3">
      <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm">
        <div class="text-sm font-semibold text-primary">Layout Parsing</div>
        <div class="mt-1 text-xs text-muted-foreground">Extract dashboard structures, export to JSON.</div>
      </div>
      <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm">
        <div class="text-sm font-semibold text-primary">KPI Cloning</div>
        <div class="mt-1 text-xs text-muted-foreground">Clone KPI sheets, swap metrics only, preserve styles.</div>
      </div>
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

# Try It Out

<div class="mx-auto mt-6 max-w-3xl text-left">
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 shadow-sm">
    <div class="font-mono text-base leading-8 text-foreground">
      <div><span class="text-muted-foreground">$</span> pip install cwprep cwtwb</div>
      <div class="mt-2"><span class="text-muted-foreground">$</span> cwprep-mcp <span class="text-xs text-muted-foreground"># start cwprep MCP server</span></div>
      <div><span class="text-muted-foreground">$</span> cwtwb-mcp <span class="text-xs text-muted-foreground"># start cwtwb MCP server</span></div>
    </div>
  </div>
  <div class="mt-4 grid gap-3 md:grid-cols-2">
    <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 text-left shadow-sm">
      <div class="text-sm font-semibold text-primary">GitHub</div>
      <div class="mt-1 text-xs leading-5 text-muted-foreground">github.com/imgwho/cwprep / cwtwb</div>
    </div>
    <div class="rounded-[20px] border border-primary/50 bg-white/50 p-4 text-left shadow-sm">
      <div class="text-sm font-semibold text-primary">datacooper.com</div>
      <div class="mt-1 text-xs leading-5 text-muted-foreground">Online Tools · Docs · Community</div>
    </div>
  </div>
</div>

---
layout: section
---

# Q&A / Discussion

---
layout: quote
---

# Don't leave Tableau. Let AI give time back to humans.
