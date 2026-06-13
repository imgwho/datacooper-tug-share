---
theme: seriph
title: Datacooper TUG Share
info: |
  Tableau User Group 分享
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
        Datacooper · Tableau User Group 分享
      </div>
      <h1 class="mt-4 max-w-5xl text-5xl font-black tracking-[-0.05em] leading-[0.94] text-primary md:text-6xl">
        从手工拖拽到工程化 BI
      </h1>
      <p class="mt-4 max-w-4xl text-base leading-7 text-muted-foreground md:text-xl md:leading-relaxed">
        <strong class="text-foreground">cwprep</strong> 负责 Tableau Prep 的数据流自动化，
        <strong class="text-foreground">cwtwb</strong> 负责 Tableau Workbook 的工程化生成，
        <strong class="text-foreground">datacooper.com</strong> 则把这些能力做成更容易使用的在线工具平台。
      </p>
      <div class="mt-6 flex flex-wrap gap-2">
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">cwtwb/cwprep = BI 开发加速器</span>
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">MCP</span>
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">可复现</span>
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">可审查</span>
        <span v-click class="rounded-full border border-primary/50 bg-white/50 px-4 py-2 text-sm font-medium text-foreground shadow-sm">可迁移</span>
      </div>
    </div>
  </div>
</div>

---
layout: center
---

# 目录

<div class="mx-auto mt-6 grid max-w-5xl gap-4 md:grid-cols-2">
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <div class="text-3xl font-black text-primary opacity-40">01</div>
    <h3 class="mt-1 text-lg font-bold text-foreground">背景与定位</h3>
    <ul class="mt-2 space-y-1 text-sm leading-6 text-muted-foreground">
      <li>工具定位 · Tableau 在数据流程中的位置</li>
      <li>机械劳动的痛点 · 适合谁</li>
    </ul>
  </div>
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <div class="text-3xl font-black text-primary opacity-40">02</div>
    <h3 class="mt-1 text-lg font-bold text-foreground">cwprep · 数据流引擎</h3>
    <ul class="mt-2 space-y-1 text-sm leading-6 text-muted-foreground">
      <li>一句话介绍 · 分层架构图</li>
      <li>vs Tableau Agent · 案例与演示</li>
    </ul>
  </div>
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <div class="text-3xl font-black text-primary opacity-40">03</div>
    <h3 class="mt-1 text-lg font-bold text-foreground">cwtwb · 工作簿工程</h3>
    <ul class="mt-2 space-y-1 text-sm leading-6 text-muted-foreground">
      <li>分层架构图 · vs Tableau Agent (Web)</li>
      <li>一句话介绍 · 实战案例与演示</li>
    </ul>
  </div>
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <div class="text-3xl font-black text-primary opacity-40">04</div>
    <h3 class="mt-1 text-lg font-bold text-foreground">datacooper.com & 收尾</h3>
    <ul class="mt-2 space-y-1 text-sm leading-6 text-muted-foreground">
      <li>在线工具平台方向</li>
      <li>快速上手 · Q&A</li>
    </ul>
  </div>
</div>

---
layout: fact
---

# cwtwb/cwprep 工具的定位

## 辅助加速 BI 开发过程

<div class="mt-6 max-w-4xl text-lg leading-8 text-muted-foreground">
  不是替代 BI 开发人员，而是把重复、机械、可规则化的工作交给工具。
</div>

---
layout: center
class: text-center
---

# Tableau 在数据分析全流程中的位置

<div class="mx-auto mt-8 grid max-w-6xl gap-4 md:grid-cols-5">
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">1. 数据接入</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">数据库、Excel、CSV、接口</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">2. 数据准备</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">清洗、转换、合并、聚合</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">3. Tableau</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">建模、计算、布局、可视化</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">4. 分发协作</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">发布、查看、评审、迭代</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">5. 反馈优化</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">修订数据、调整设计、重发版本</div>
  </div>
</div>

<div class="mx-auto mt-7 max-w-4xl rounded-[24px] border border-primary/50 bg-white/50 px-6 py-4 text-base leading-7 text-foreground shadow-sm">
  cwprep 主要落在“数据准备”，cwtwb 主要落在“Tableau 生成与编排”，中间由 Tableau 承接分析表达。
</div>

---
layout: section
---

# 为什么要做这些工具

---
layout: center
class: text-center
---

# 机械劳动的痛点

<div class="mx-auto max-w-5xl">
  <div class="rounded-[28px] border border-primary/50 bg-white/50 px-8 py-7 text-lg leading-8 text-muted-foreground shadow-sm">
    Tableau 里最耗时的，往往不是“画一个图”，而是机械性地反复做这些事。
  </div>

  <div class="mt-6 grid gap-4 md:grid-cols-3">
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复拖拽字段</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复调布局</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复复制 KPI 模块</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复迁移 workbook</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复检查文件能否正常打开</div>
    <div v-click class="rounded-[22px] border border-primary/50 bg-white/50 px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复修细碎但耗时的问题</div>
  </div>
</div>

---
layout: center
class: text-center
---

# 这些工具适合谁

<div class="mx-auto mt-8 grid max-w-5xl gap-4 md:grid-cols-3">
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="mt-2 text-lg font-bold text-foreground">Tableau 分析师</h3>
    <p class="mt-2 text-sm leading-6 text-muted-foreground">减少重复拖拽和复制粘贴，把时间还给业务分析和洞察判断。</p>
  </div>
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="mt-2 text-lg font-bold text-foreground">数据工程 / IT</h3>
    <p class="mt-2 text-sm leading-6 text-muted-foreground">自动化、版本控制、批量部署，让 BI 进入工程化流程。</p>
  </div>
  <div v-click class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-sm">
    <h3 class="mt-2 text-lg font-bold text-foreground">团队管理者</h3>
    <p class="mt-2 text-sm leading-6 text-muted-foreground">可审计、可复现、可交付，降低人员依赖和知识流失风险。</p>
  </div>
</div>

---
layout: section
---

# cwprep

---
layout: default
---

# cwprep 一句话介绍

<div class="grid grid-cols-1 gap-4" style="grid-template-columns: 1.05fr 0.95fr">
  <div class="flex flex-col justify-between">
    <div>
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
        一句话
      </div>
      <h2 class="mt-3 text-3xl font-black tracking-[-0.04em] text-foreground md:text-4xl">
        输入一句话，输出一个可用的 Tableau Prep .tfl / .tflx 文件。
      </h2>
    </div>
    <div class="mt-4 grid gap-2 md:grid-cols-2">
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">Text-to-PrepFlow</div>
        <div class="mt-1 leading-6 text-muted-foreground">直接用自然语言描述数据处理逻辑。</div>
      </div>
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">MCP 集成</div>
        <div class="mt-1 leading-6 text-muted-foreground">可接 Claude、Gemini、Cursor 等客户端。</div>
      </div>
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">避免 GUI 依赖</div>
        <div class="mt-1 leading-6 text-muted-foreground">不用每次打开 Tableau Prep 也能构建流程。</div>
      </div>
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">可审查</div>
        <div class="mt-1 leading-6 text-muted-foreground">支持把 flow 翻译成 SQL，便于 DBA / 合规查看。</div>
      </div>
    </div>
    <div v-click class="mt-3 flex flex-wrap gap-2">
      <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-xs font-medium text-foreground shadow-sm">22 种数据流操作</span>
      <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-xs font-medium text-foreground shadow-sm">4 种数据库</span>
      <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-xs font-medium text-foreground shadow-sm">SQL 翻译</span>
      <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-xs font-medium text-foreground shadow-sm">TFLX 打包</span>
    </div>
  </div>
  <div class="rounded-[28px] border border-primary/50 bg-white/50 p-5 shadow-sm">
    <div v-click class="inline-flex items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
      核心价值
    </div>
    <p v-click class="mt-3 text-sm leading-6 text-muted-foreground">
      cwprep 管"数据怎么流动"，cwtwb 管"仪表板怎么生成"。
    </p>
    <div class="mt-3 grid gap-2">
      <div v-click class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 shadow-sm">
        <div class="text-sm font-semibold text-primary">效率加速</div>
        <div class="mt-1 text-xs leading-5 text-muted-foreground">把重复性的 Prep 流搭建自动化。</div>
      </div>
      <div v-click class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 shadow-sm">
        <div class="text-sm font-semibold text-primary">质量稳定</div>
        <div class="mt-1 text-xs leading-5 text-muted-foreground">把常见规则固化下来，减少人工偏差。</div>
      </div>
      <div v-click class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 shadow-sm">
        <div class="text-sm font-semibold text-primary">工程协作</div>
        <div class="mt-1 text-xs leading-5 text-muted-foreground">让数据清洗进入脚本、版本控制和批量生产流程。</div>
      </div>
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

# cwprep 架构图

<div class="big-diagram mt-10 mb-10">

```mermaid
flowchart TD
  subgraph Interfaces["Interfaces"]
    direction LR
    MCP["MCP Server\n(tools · resources · prompts)\nClaude / Cursor / VSCode / Gemini"]
    PY["Python Library\nfrom cwprep import TFLBuilder, TFLPackager\nbuilder.add_...() / builder.build()"]
  end

  subgraph Core["TFLBuilder"]
    direction LR
    SDK["TFLBuilder · TFLPackager · SQLTranslator · ExpressionTranslator"]
  end

  subgraph Operations["Operations"]
    direction LR
    DS["Data Sources\nMySQL · PostgreSQL · SQL Server\nExcel · CSV · SQL"]
    TF["Transformations\nJoin · Union · Filter · Rename\nCalculation · Change Type · Pivot"]
    AN["Analytics & Output\nAggregate · Unpivot\nSQL Translation · TFLX Packaging"]
  end

  subgraph Validation["Validation & Packaging"]
    direction LR
    VL["validate_flow_definition → build → save_tfl / save_tflx"]
  end

  OUT[".tfl / .tflx"]

  MCP --> Core
  PY --> Core
  Core --> DS
  Core --> TF
  Core --> AN
  DS --> VL
  TF --> VL
  AN --> VL
  VL --> OUT
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
      <li>官方闭源产品</li>
      <li>自然语言驱动 Prep 流</li>
      <li>仅限 Tableau Cloud</li>
      <li>不支持 Join / Union</li>
      <li>不支持 SQL 导出</li>
    </ul>
    <div class="mt-4 text-[8px] break-all text-muted-foreground opacity-60">
      Source: <a href="https://help.tableau.com/current/prep/en-us/prep_einstein.htm" target="_blank" class="hover:text-primary transition-colors">https://help.tableau.com/current/prep/en-us/prep_einstein.htm</a>
    </div>
  </div>
  <div class="flex items-center justify-center">
    <div class="text-2xl font-black text-primary">VS</div>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-md">
    <h3 class="text-lg font-bold text-primary">cwprep</h3>
    <ul class="mt-3 space-y-2 text-sm leading-6 text-foreground font-medium">
      <li>开源，可本地部署</li>
      <li>自然语言 + 代码双驱动</li>
      <li>支持任意环境</li>
      <li class="text-primary font-bold">✅ Join / Union / Pivot</li>
      <li class="text-primary font-bold">✅ Flow → SQL 翻译</li>
    </ul>
  </div>
</div>

<div class="mx-auto mt-5 max-w-3xl rounded-[20px] border border-primary/50 bg-white/50 px-5 py-3 text-sm leading-6 text-foreground shadow-sm">
  功能覆盖率达 <strong class="text-primary">88%</strong>，并独享 Join、Union、SQL 翻译等能力。
</div>

---
layout: center
---

# cwprep 典型案例与快速演示

<div class="grid grid-cols-2 gap-6 mt-4 text-left">
  <div class="space-y-4">
    <div class="p-6 border border-primary/50 rounded-[28px] bg-white/50 shadow-sm">
      <h3 class="text-xl font-bold mb-3 text-primary">案例 1：零门槛秒级生成</h3>
      <p class="text-sm leading-relaxed text-muted-foreground">
        完全不需要本地环境。用户通过自然语言将清洗逻辑发送给 Agent，系统在几秒内直接生成标准的 .tfl 文件。
      </p>
      <ul class="mt-3 space-y-1 text-xs text-foreground font-medium">
        <li>✅ 文本直接转清洗流 (Text-to-Flow)</li>
        <li>✅ Web 端轻量化操作，无需安装</li>
      </ul>
    </div>
    <div class="p-6 border border-primary/50 rounded-[28px] bg-white/50 shadow-sm">
      <h3 class="text-xl font-bold mb-3 text-primary">案例 2：多表复杂逻辑解析</h3>
      <p class="text-sm leading-relaxed text-muted-foreground">
        Agent 深度理解包含多步骤、跨多张表（订单、退货、客户）关联的业务描述，并精准转化为数据管道。
      </p>
      <ul class="mt-3 space-y-1 text-xs text-foreground font-medium">
        <li>✅ 自动识别 ER 关系与 Join 逻辑</li>
        <li>✅ 处理复杂的聚合与过滤规则</li>
      </ul>
    </div>
  </div>

  <div class="grid grid-cols-1 gap-4">
    <div class="rounded-2xl border border-primary/30 bg-white/50 p-3 shadow-md">
      <div class="aspect-video rounded-xl overflow-hidden bg-black mb-2">
        <Youtube id="b7WrC0ngqwk" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs text-center">视频演示：极速生成 (Seconds Response)</h4>
    </div>
    <div class="rounded-2xl border border-primary/30 bg-white/50 p-3 shadow-md">
      <div class="aspect-video rounded-xl overflow-hidden bg-black mb-2">
        <Youtube id="4RMevXQObkE" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs text-center">视频演示：复杂逻辑 (Deep Parsing)</h4>
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

# cwtwb 架构图

<div class="big-diagram mt-10 mb-10">

```mermaid
flowchart TD
  subgraph Interfaces["Interfaces"]
    direction LR
    MCP["MCP Server\n(tools_workbook)\nClaude / Cursor / VSCode / Claude Code"]
    PY["Python Library\nfrom cwtwb.twb_editor import TWBEditor\neditor.add_...() / configure_...() / save(...)"]
  end

  subgraph Core["TWBEditor"]
    direction LR
    MX["ParametersMixin · ConnectionsMixin · ChartsMixin · DashboardsMixin"]
  end

  subgraph Subsystems["Subsystems"]
    direction LR
    CB["Chart Builders\nBasic · DualAxis · Pie\nText · Map · Recipes"]
    DS["Dashboard System\nlayouts · actions\ndependencies"]
    AM["Analysis & Migration\nmigration.py · twb_analyzer.py\ncapability_registry"]
  end

  subgraph Foundation["XML Engine (lxml)"]
    direction LR
    XE["template.twb / .twbx → patch → validate → save"]
  end

  OUT["output.twb / output.twbx"]

  MCP --> Core
  PY --> Core
  Core --> CB
  Core --> DS
  Core --> AM
  CB --> XE
  DS --> XE
  AM --> XE
  XE --> OUT
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
      <li>仅限 Worksheets (工作表)</li>
      <li>无法构建 Dashboard</li>
      <li>无法进行格式化美化</li>
      <li>不支持参数/集等交互控件</li>
      <li>不支持数据建模 (Join/Relation)</li>
    </ul>
    <div class="mt-4 text-[8px] break-all text-muted-foreground opacity-60">
      Source: <a href="https://help.tableau.com/current/online/en-us/web_author_einstein.htm" target="_blank" class="hover:text-primary transition-colors">https://help.tableau.com/current/online/en-us/web_author_einstein.htm</a>
    </div>
  </div>
  <div class="flex items-center justify-center">
    <div class="text-2xl font-black text-primary">VS</div>
  </div>
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-6 text-left shadow-md">
    <h3 class="text-lg font-bold text-primary">cwtwb</h3>
    <ul class="mt-3 space-y-2 text-sm leading-6 text-foreground font-medium">
      <li class="text-primary font-bold">✅ 完整的 Dashboard 编排</li>
      <li class="text-primary font-bold">✅ 声明式布局与格式化</li>
      <li class="text-primary font-bold">✅ 支持跨源数据迁移</li>
      <li class="text-primary font-bold">✅ XSD 结构校验与版本化</li>
      <li>支持离线/自动化批量生产</li>
    </ul>
  </div>
</div>

<div class="mx-auto mt-5 max-w-3xl rounded-[20px] border border-primary/50 bg-white/50 px-5 py-3 text-sm leading-6 text-foreground shadow-sm">
  cwtwb 是 **"工程化 BI 生成器"**，填补了官方 Agent 在复杂布局和自动化生产上的空白。
</div>

---
layout: default
---

# cwtwb 一句话介绍

<div class="grid grid-cols-1 gap-4" style="grid-template-columns: 1.05fr 0.95fr">
  <div class="flex flex-col justify-between">
    <div>
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
        一句话
      </div>
      <h2 class="mt-3 text-3xl font-black tracking-[-0.04em] text-foreground md:text-4xl">
        把 Tableau workbook 变成可复现、可验证、可迁移的工程产物。
      </h2>
    </div>
    <div class="mt-4 grid gap-2 md:grid-cols-2">
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">生成</div>
        <div class="mt-1 leading-6 text-muted-foreground">从代码或 agent 调用生成 TWB。</div>
      </div>
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">校验</div>
        <div class="mt-1 leading-6 text-muted-foreground">结构校验 + XSD 校验。</div>
      </div>
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">迁移</div>
        <div class="mt-1 leading-6 text-muted-foreground">快速迁移到新数据源。</div>
      </div>
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">编排</div>
        <div class="mt-1 leading-6 text-muted-foreground">支持 Chart、Layout 等编排。</div>
      </div>
    </div>
    <div v-click class="mt-3 flex flex-wrap gap-2">
      <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-xs font-medium text-foreground shadow-sm">15+ 图表类型</span>
      <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-xs font-medium text-foreground shadow-sm">50+ MCP 工具</span>
      <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-xs font-medium text-foreground shadow-sm">XSD 校验</span>
      <span class="rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-xs font-medium text-foreground shadow-sm">声明式布局</span>
    </div>
  </div>
  <div class="rounded-[28px] border border-primary/50 bg-white/50 p-5 shadow-sm">
    <div v-click class="inline-flex items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
      核心价值
    </div>
    <p v-click class="mt-3 text-sm leading-6 text-muted-foreground">
      cwprep 管"数据怎么流动"，cwtwb 管"仪表板怎么生成"。
    </p>
    <div class="mt-3 grid gap-2">
      <div v-click class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 shadow-sm">
        <div class="text-sm font-semibold text-primary">确定性输出</div>
        <div class="mt-1 text-xs leading-5 text-muted-foreground">结果稳定复现。</div>
      </div>
      <div v-click class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 shadow-sm">
        <div class="text-sm font-semibold text-primary">交付可验证</div>
        <div class="mt-1 text-xs leading-5 text-muted-foreground">能检查，能打开。</div>
      </div>
      <div v-click class="rounded-[18px] border border-primary/50 bg-white/50 px-4 py-3 shadow-sm">
        <div class="text-sm font-semibold text-primary">适合迁移项目</div>
        <div class="mt-1 text-xs leading-5 text-muted-foreground">无需从零重建。</div>
      </div>
    </div>
  </div>
</div>

---
layout: center
---

# cwtwb 实战案例与闭环演示

<div class="grid grid-cols-2 gap-6 mt-4 text-left">
  <div class="space-y-4">
    <div class="p-6 border border-primary/50 rounded-[28px] bg-white/50 shadow-sm">
      <h3 class="text-xl font-bold mb-3 text-primary">案例 3：声明式代码与自动纠错</h3>
      <p class="text-sm leading-relaxed text-muted-foreground">
        演示 Python 开发框架的 4 步流程：感知架构、生成代码、运行脚本、自动纠错（Bug Fix）。
      </p>
      <ul class="mt-3 space-y-1 text-xs text-foreground font-medium">
        <li>✅ AI 感知数据库 Schema / ER 图</li>
        <li>✅ <strong>亮点：</strong> Agent 自动修正大小写敏感错误</li>
      </ul>
    </div>
    <div class="p-6 border border-primary/50 rounded-[28px] bg-white/50 shadow-sm">
      <h3 class="text-xl font-bold mb-3 text-primary">案例 4：端到端实时仪表板渲染</h3>
      <p class="text-sm leading-relaxed text-muted-foreground">
        从原始文档到功能完备的 Tableau 仪表板。观众可以实时观察到 Dashboard 在客户端从无到有的渲染过程。
      </p>
      <ul class="mt-3 space-y-1 text-xs text-foreground font-medium">
        <li>✅ 全流程自动化闭环</li>
        <li>✅ 像写代码一样“热更新”仪表板</li>
      </ul>
    </div>
  </div>

  <div class="grid grid-cols-1 gap-4">
    <div class="rounded-2xl border border-primary/30 bg-white/50 p-3 shadow-md">
      <div class="aspect-video rounded-xl overflow-hidden bg-black mb-2">
        <Youtube id="dNzMbLOEA7A" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs text-center">视频演示：Python 实战与自动纠错</h4>
    </div>
    <div class="rounded-2xl border border-primary/30 bg-white/50 p-3 shadow-md">
      <div class="aspect-video rounded-xl overflow-hidden bg-black mb-2">
        <Youtube id="NMy4__CCCDI" width="100%" height="100%" />
      </div>
      <h4 class="font-bold text-xs text-center">视频演示：Dashboard 实时渲染</h4>
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

# datacooper 在线工具原型

<div class="grid grid-cols-1 gap-4" style="grid-template-columns: 1.05fr 0.95fr">
  <div class="flex flex-col justify-between">
    <div>
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
        未来方向
      </div>
      <h2 class="mt-3 text-3xl font-black tracking-[-0.04em] text-foreground md:text-4xl">
        把这些能力做成在线工具平台，而不只是本地脚本。
      </h2>
      <p v-click class="mt-4 max-w-xl text-base leading-7 text-muted-foreground">
        不是把命令搬到网页，而是把常见 BI 动作变成上传即用、顺手操作的在线工作台。底层共用 Python SDK。
      </p>
    </div>
    <div v-click class="mt-4 grid grid-cols-2 gap-2">
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm leading-6 shadow-sm">在线使用</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm leading-6 shadow-sm">直接处理文件</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm leading-6 shadow-sm">更低门槛</div>
      <div class="rounded-[18px] border border-primary/50 bg-white/50 p-3 text-sm leading-6 shadow-sm">代码变工具</div>
    </div>
  </div>
  <div class="rounded-[28px] border border-primary/50 bg-white/50 p-6 shadow-sm">
    <div v-click class="inline-flex items-center gap-2 rounded-full border border-primary/50 bg-white/50 px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
      已有的两个工具原型
    </div>
    <div class="mt-4 space-y-3">
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm">
        <div class="text-sm font-semibold text-primary">布局解析</div>
        <div class="mt-1 text-xs leading-5 text-muted-foreground">提取 dashboard 布局结构，导出 JSON。</div>
      </div>
      <div v-click class="rounded-[20px] border border-primary/50 bg-white/50 p-4 shadow-sm">
        <div class="text-sm font-semibold text-primary">KPI 复制</div>
        <div class="mt-1 text-xs leading-5 text-muted-foreground">复制 KPI 工作表，只替换指标，保留原结构和样式。</div>
      </div>
    </div>
    <div v-click class="mt-4 rounded-[20px] border border-dashed border-primary/50 bg-white/50 px-4 py-3">
      <div class="text-xs font-semibold text-primary">更长远</div>
      <div class="mt-1 text-xs leading-5 text-muted-foreground">
        协作与版本管理 — 创想方向，非当前承诺。
      </div>
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

# 试试看

<div class="mx-auto mt-3 max-w-3xl text-left">
  <div class="rounded-[24px] border border-primary/50 bg-white/50 p-4 shadow-sm font-mono text-[13px] leading-6 text-foreground">
    <div class="mb-2 text-muted-foreground"># 1. 安装 SDK</div>
    <div><span class="text-muted-foreground">$</span> pip install cwprep</div>
    <div><span class="text-muted-foreground">$</span> pip install cwtwb</div>
    <div class="mt-3 mb-2 text-muted-foreground"># 2. 配置 MCP (Claude Desktop / Cursor)</div>
    <pre class="bg-black/5 p-2.5 rounded-lg text-[11px] leading-relaxed whitespace-pre overflow-auto">
{{ `{
  "mcpServers": {
    "cwprep": { "command": "uvx", "args": ["cwprep"] },
    "cwtwb": { "command": "uvx", "args": ["cwtwb"] }
  }
}` }}
    </pre>
  </div>
  <div class="mt-3 grid gap-3 md:grid-cols-2">
    <a href="https://github.com/imgwho/cwprep" target="_blank" class="rounded-[20px] border border-primary/50 bg-white/50 px-4 py-3 text-left shadow-sm hover:bg-primary/5 transition-colors no-underline">
      <div class="text-sm font-semibold text-primary">GitHub: cwprep</div>
      <div class="mt-0.5 text-xs text-muted-foreground">github.com/imgwho/cwprep</div>
    </a>
    <a href="https://github.com/imgwho/cwtwb" target="_blank" class="rounded-[20px] border border-primary/50 bg-white/50 px-4 py-3 text-left shadow-sm hover:bg-primary/5 transition-colors no-underline">
      <div class="text-sm font-semibold text-primary">GitHub: cwtwb</div>
      <div class="mt-0.5 text-xs text-muted-foreground">github.com/imgwho/cwtwb</div>
    </a>
    <a href="https://datacooper.com" target="_blank" class="col-span-full rounded-[20px] border border-primary/50 bg-white/50 px-4 py-3 text-left shadow-sm hover:bg-primary/5 transition-colors no-underline">
      <div class="text-sm font-semibold text-primary">datacooper.com</div>
      <div class="mt-0.5 text-xs leading-5 text-muted-foreground">在线工具 · 文档 · 社区</div>
    </a>
  </div>
</div>

---
layout: center
---

# 致谢

<div class="mx-auto mt-4 max-w-4xl space-y-3 text-left">
  <div class="grid gap-3 md:grid-cols-2">
    <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
      <div class="text-sm font-bold text-foreground">Patrick Therriault</div>
      <div class="mt-1 text-xs leading-5 text-muted-foreground">引导我深入 Tableau 社区</div>
    </div>
    <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
      <div class="text-sm font-bold text-foreground">Andy Cotgreave</div>
      <div class="mt-1 text-xs leading-5 text-muted-foreground">推动项目前进的洞察</div>
    </div>
    <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
      <div class="text-sm font-bold text-foreground">Adam Mico</div>
      <div class="mt-1 text-xs leading-5 text-muted-foreground">耐心与扎实的建议</div>
    </div>
    <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
      <div class="text-sm font-bold text-foreground">Jeffrey Shaffer</div>
      <div class="mt-1 text-xs leading-5 text-muted-foreground">推荐的技巧成为很好的过程约束</div>
    </div>
    <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
      <div class="text-sm font-bold text-foreground">Matthew Miller · Elif Tutuk · Paul Morgan · Olga L.</div>
      <div class="mt-1 text-xs leading-5 text-muted-foreground">来自官方的极有价值的提示</div>
    </div>
    <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
      <div class="text-sm font-bold text-foreground">Li-Lun Tu</div>
      <div class="mt-1 text-xs leading-5 text-muted-foreground">品牌建设方面的建议</div>
    </div>
  </div>
  <div class="rounded-[20px] border border-primary/50 bg-white/50 px-5 py-4 shadow-sm">
    <div class="text-sm font-bold text-foreground">Alex Mou</div>
    <div class="mt-1 text-xs leading-5 text-muted-foreground">鼓励以及交流中给我的建议</div>
  </div>
  <div class="rounded-[20px] border border-dashed border-primary/50 bg-white/50 px-5 py-4 text-center shadow-sm">
    <div class="text-sm leading-6 text-muted-foreground">感谢每一位留言和参与讨论、帮助我走在正确方向上的朋友！</div>
  </div>
</div>

---
layout: quote
---

# 不离开 Tableau，用 AI 把时间还给人类。

---
layout: section
---

# Q&A / 交流
