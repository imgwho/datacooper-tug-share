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

<div class="min-h-[86vh] px-8 py-10 md:px-16">
  <div class="mx-auto flex min-h-[86vh] max-w-[1180px] items-start pt-6 md:pt-10">
    <div v-motion :initial="{ opacity: 0, y: 100 }" :enter="{ opacity: 1, y: 0 }" class="w-full rounded-[40px] border border-primary/10 bg-[radial-gradient(circle_at_top_right,oklch(61.71%_.1375_39.0427_/_0.12),transparent_36%),radial-gradient(circle_at_bottom_left,rgba(233,230,220,0.8),transparent_30%),var(--card)] px-8 py-10 shadow-sm md:px-12 md:py-14">
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/20 bg-background px-4 py-2 text-xs font-semibold uppercase tracking-[0.22em] text-primary shadow-sm">
        Datacooper · Tableau User Group 分享
      </div>
      <h1 class="mt-6 max-w-5xl text-5xl font-black tracking-[-0.05em] leading-[0.94] text-primary md:text-7xl">
        从手工拖拽到工程化 BI
      </h1>
      <p class="mt-6 max-w-4xl text-lg leading-8 text-muted-foreground md:text-2xl md:leading-relaxed">
        <strong class="text-foreground">cwprep</strong> 负责 Tableau Prep 的数据流自动化，
        <strong class="text-foreground">cwtwb</strong> 负责 Tableau Workbook 的工程化生成，
        <strong class="text-foreground">datacooper.com</strong> 则把这些能力做成更容易使用的在线工具平台。
      </p>
      <div class="mt-8 flex flex-wrap gap-3">
        <span v-click class="rounded-full border border-primary/20 bg-background px-4 py-2 text-sm font-medium text-foreground shadow-sm">Python 工具 = BI 开发加速器</span>
        <span v-click class="rounded-full border border-primary/20 bg-background px-4 py-2 text-sm font-medium text-foreground shadow-sm">MCP</span>
        <span v-click class="rounded-full border border-primary/20 bg-background px-4 py-2 text-sm font-medium text-foreground shadow-sm">可复现</span>
        <span v-click class="rounded-full border border-primary/20 bg-background px-4 py-2 text-sm font-medium text-foreground shadow-sm">可审查</span>
        <span v-click class="rounded-full border border-primary/20 bg-background px-4 py-2 text-sm font-medium text-foreground shadow-sm">可迁移</span>
      </div>
    </div>
  </div>
</div>

---
layout: fact
---

# Python 工具的定位

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
  <div v-click class="rounded-[22px] border border-primary/10 bg-card p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">1. 数据接入</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">数据库、Excel、CSV、接口</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/10 bg-card p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">2. 数据准备</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">清洗、转换、合并、聚合</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/10 bg-card p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">3. Tableau</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">建模、计算、布局、可视化</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/10 bg-card p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">4. 分发协作</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">发布、查看、评审、迭代</div>
  </div>
  <div v-click class="rounded-[22px] border border-primary/10 bg-card p-4 shadow-sm">
    <div class="text-sm font-semibold text-primary">5. 反馈优化</div>
    <div class="mt-2 text-sm leading-6 text-muted-foreground">修订数据、调整设计、重发版本</div>
  </div>
</div>

<div class="mx-auto mt-7 max-w-4xl rounded-[24px] border border-primary/20 bg-primary/10 px-6 py-4 text-base leading-7 text-foreground shadow-sm">
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

<div class="mx-auto max-w-5xl">
  <div class="rounded-[28px] border border-primary/10 bg-card px-8 py-7 text-lg leading-8 text-muted-foreground shadow-sm">
    Tableau 里最耗时的，往往不是“画一个图”，而是机械性地反复做这些事。
  </div>

  <div class="mt-6 grid gap-4 md:grid-cols-2">
    <div v-click class="rounded-[22px] border border-primary/10 bg-card px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复拖拽字段</div>
    <div v-click class="rounded-[22px] border border-primary/10 bg-card px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复调布局</div>
    <div v-click class="rounded-[22px] border border-primary/10 bg-card px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复复制 KPI 模块</div>
    <div v-click class="rounded-[22px] border border-primary/10 bg-card px-6 py-5 text-lg font-medium text-foreground shadow-sm">反复迁移 workbook</div>
  </div>

  <div class="mt-6 rounded-[24px] border border-primary/20 bg-primary/10 px-6 py-5 text-base leading-7 text-foreground shadow-sm">
    这些事单个看都不难，但它们不创造新的业务价值，却持续消耗开发时间。
  </div>
</div>

---
layout: center
---

# 研发范式的改变

<div class="grid grid-cols-2 gap-10 mt-10 text-left">
  <div v-click class="p-8 border border-primary/10 rounded-[32px] bg-white/50 shadow-sm">
    <h3 class="text-2xl font-bold mb-6 text-foreground">传统方式 (Manual)</h3>
    <ul class="space-y-4 text-muted-foreground text-lg">
      <li class="flex items-start gap-3"><span>❌</span> <span>300+ 次重复的鼠标点击</span></li>
      <li class="flex items-start gap-3"><span>❌</span> <span>无法复用的二进制 .twb 文件</span></li>
      <li class="flex items-start gap-3"><span>❌</span> <span>变更时需全量重新拖拽</span></li>
      <li class="flex items-start gap-3"><span>❌</span> <span>逻辑隐藏在 GUI 深处，无法审计</span></li>
    </ul>
  </div>
  
  <div v-click class="p-8 border border-primary/30 rounded-[32px] bg-primary/5 shadow-md">
    <h3 class="text-2xl font-bold mb-6 text-primary">工程化方式 (Engineering)</h3>
    <ul class="space-y-4 text-foreground font-medium text-lg">
      <li class="flex items-start gap-3"><span>✅</span> <span>一行命令/一句话生成</span></li>
      <li class="flex items-start gap-3"><span>✅</span> <span>纯文本配置，可 Git 管理</span></li>
      <li class="flex items-start gap-3"><span>✅</span> <span>模块化组件，秒级替换指标</span></li>
      <li class="flex items-start gap-3"><span>✅</span> <span>代码即文档，随时可追溯审计</span></li>
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

# cwprep 架构图

<div class="big-diagram mt-10 mb-10">

```mermaid
flowchart LR
  A["自然语言 / MCP"] --> B["Planner"]
  C["数据库 / Excel / CSV"] --> B
  B --> D["Flow Builder"]
  D --> E["Validator"]
  D --> F["SQL Translator"]
  E --> G[".tfl / .tflx"]
  F --> G
  G --> H["可审查 / 可复用 / 可分享"]
```

</div>

---
layout: default
---

## cwprep

### 一句话

输入一句话，输出一个可用的 Tableau Prep `.tfl` / `.tflx` 文件。

### 它能做什么

- Text-to-PrepFlow: 直接用自然语言描述数据处理逻辑
- MCP 集成: 可接 Claude、Gemini、Cursor 等客户端
- 避免 GUI 依赖: 不用每次打开 Tableau Prep 也能构建流程
- 可审查: 支持把 flow 翻译成 SQL，便于 DBA / 合规查看

---
layout: center
class: text-center
---

# cwprep 典型案例

<div class="mx-auto mt-8 grid max-w-6xl gap-4 md:grid-cols-2">
  <div class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">数据合并与连接</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">自动化处理多数据源 Join 逻辑。</p>
  </div>
  <div class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">自动化数据清洗</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">根据业务规则自动完成类型转换与过滤。</p>
  </div>
  <div class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">指标聚合计算</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">在 Prep 层预处理复杂的业务指标。</p>
  </div>
  <div class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">全流程自动化</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">从原始数据到 TFLX 文件的端到端生成。</p>
  </div>
</div>

---
layout: fact
---

# cwprep 的价值

## 让 Prep 流生成、修改、审查都变成工程动作

---
layout: center
class: text-center
---

<div class="mx-auto grid max-w-6xl gap-4 md:grid-cols-3">
  <div v-click class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">效率加速</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">把重复性的 Prep 流搭建自动化。</p>
  </div>
  <div v-click class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">质量稳定</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">把常见规则固化下来，减少人工偏差。</p>
  </div>
  <div v-click class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">工程协作</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">让数据清洗进入脚本、版本控制和批量生产流程。</p>
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
flowchart LR
  A["Prompt / Existing TWB / Layout JSON"] --> B["Workbook Composer"]
  A --> C["Chart Recipe Engine"]
  A --> D["Layout Engine"]
  B --> E["Worksheet Refactor / Migration"]
  C --> E
  D --> E
  E --> F["Validation"]
  F --> G[".twb / .twbx"]
  G --> H["可复现 / 可验证 / 可迁移"]
```

</div>

---
layout: default
---

<div class="grid min-h-[78vh] grid-cols-1 gap-8" style="grid-template-columns: 1.05fr 0.95fr">
  <div class="flex flex-col justify-between">
    <div>
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/20 bg-secondary px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
        一句话
      </div>
      <h2 class="mt-4 text-4xl font-black tracking-[-0.04em] text-foreground md:text-5xl">
        把 Tableau workbook 变成可复现、可验证、可迁移的工程产物。
      </h2>
    </div>
    <div class="mt-8 grid gap-3 md:grid-cols-2">
      <div class="rounded-[20px] border border-primary/10 bg-card p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">生成</div>
        <div class="mt-1 leading-6 text-muted-foreground">从代码或 agent 调用生成 TWB。</div>
      </div>
      <div class="rounded-[20px] border border-primary/10 bg-card p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">校验</div>
        <div class="mt-1 leading-6 text-muted-foreground">结构校验 + XSD 校验。</div>
      </div>
      <div class="rounded-[20px] border border-primary/10 bg-card p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">迁移</div>
        <div class="mt-1 leading-6 text-muted-foreground">快速迁移到新数据源。</div>
      </div>
      <div class="rounded-[20px] border border-primary/10 bg-card p-4 shadow-sm text-sm">
        <div class="font-semibold text-primary">编排</div>
        <div class="mt-1 leading-6 text-muted-foreground">支持 Chart、Layout 等编排。</div>
      </div>
    </div>
  </div>
  <div class="rounded-[28px] border border-primary/20 bg-card p-7 shadow-sm">
    <div class="inline-flex items-center gap-2 rounded-full border border-primary/20 bg-background px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
      你可以理解成
    </div>
    <p class="mt-5 text-lg leading-8 text-muted-foreground">
      cwprep 管的是“数据怎么流动”，<br>
      cwtwb 管的是“仪表板怎么生成”。
    </p>
    <div class="mt-6 grid gap-3 md:grid-cols-2">
      <div class="rounded-[18px] border border-primary/10 bg-background px-4 py-3 text-sm text-foreground shadow-sm">可复现</div>
      <div class="rounded-[18px] border border-primary/10 bg-background px-4 py-3 text-sm text-foreground shadow-sm">可验证</div>
      <div class="rounded-[18px] border border-primary/10 bg-background px-4 py-3 text-sm text-foreground shadow-sm">可迁移</div>
      <div class="rounded-[18px] border border-primary/10 bg-background px-4 py-3 text-sm text-foreground shadow-sm">可编排</div>
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
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/20 bg-secondary px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
        核心定位
      </div>
      <h2 class="mt-4 max-w-xl text-4xl font-black tracking-[-0.04em] leading-[1.1] text-foreground md:text-5xl">
        Workbook engineering layer。
      </h2>
      <p class="mt-5 max-w-lg text-lg leading-8 text-muted-foreground">
        它把 Tableau workbook 的生成、校验、迁移和局部重构变成可重复执行的工程动作。
      </p>
    </div>
  </div>

  <div class="rounded-[28px] border border-primary/20 bg-card p-7 text-left shadow-sm">
    <div class="inline-flex items-center gap-2 rounded-full border border-primary/20 bg-background px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
      它的核心价值
    </div>
    <div class="mt-6 grid gap-4">
      <div class="rounded-[20px] border border-primary/10 bg-background px-5 py-4 shadow-sm">
        <div class="text-base font-semibold text-primary">确定性输出</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">结果稳定复现。</div>
      </div>
      <div class="rounded-[20px] border border-primary/10 bg-background px-5 py-4 shadow-sm">
        <div class="text-base font-semibold text-primary">交付可验证</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">能检查，能打开。</div>
      </div>
      <div class="rounded-[20px] border border-primary/10 bg-background px-5 py-4 shadow-sm">
        <div class="text-base font-semibold text-primary">适合迁移项目</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">无需从零重建。</div>
      </div>
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

# cwtwb 典型案例

<div class="mx-auto mt-8 grid max-w-6xl gap-4 md:grid-cols-2">
  <div class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">端到端自动化生成</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">从代码一键生成完整的 TWBX 文件。</p>
  </div>
  <div class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">工作表局部重构</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">只替换特定的 KPI 指标，保留原始排版。</p>
  </div>
  <div class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">跨环境数据源迁移</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">快速适配测试环境与生产环境的数据源变更。</p>
  </div>
  <div class="rounded-[24px] border border-primary/10 bg-card p-6 text-left shadow-sm">
    <h3 class="text-xl font-bold text-foreground">声明式布局管理</h3>
    <p class="mt-2 text-sm leading-7 text-muted-foreground">用 JSON 定义仪表板布局，批量生成看板。</p>
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
      <div class="inline-flex w-fit items-center gap-2 rounded-full border border-primary/20 bg-secondary px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
        未来方向
      </div>
      <h2 class="mt-4 text-4xl font-black tracking-[-0.04em] text-foreground md:text-5xl">
        把这些能力做成在线工具平台，而不只是本地脚本。
      </h2>
      <p class="mt-5 max-w-xl text-base leading-7 text-muted-foreground md:text-lg">
        目标不是把命令简单搬到网页，而是把常见 BI 动作变成更顺手的在线工作台。
        底层共用 Python SDK，前台则把能力包装成更容易使用的在线体验。
      </p>
    </div>
    <div class="mt-8 grid grid-cols-2 gap-3">
      <div class="rounded-[18px] border border-border bg-card p-3 text-sm leading-6 shadow-sm">能在线使用</div>
      <div class="rounded-[18px] border border-border bg-card p-3 text-sm leading-6 shadow-sm">能直接处理文件</div>
      <div class="rounded-[18px] border border-border bg-card p-3 text-sm leading-6 shadow-sm">更低门槛开放给 BI 开发者</div>
      <div class="rounded-[18px] border border-border bg-card p-3 text-sm leading-6 shadow-sm">能从代码能力变成可直接点开用的工具</div>
    </div>
    <div class="mt-6 rounded-[24px] border border-dashed border-primary/25 bg-primary/5 p-5 shadow-sm">
      <div class="text-sm font-semibold text-primary">在线体验的直觉</div>
      <div class="mt-3 flex flex-wrap gap-2 text-sm text-foreground">
        <span class="rounded-full border border-border bg-background px-3 py-1">上传</span>
        <span class="rounded-full border border-border bg-background px-3 py-1">解析</span>
        <span class="rounded-full border border-border bg-background px-3 py-1">预览</span>
        <span class="rounded-full border border-border bg-background px-3 py-1">调整</span>
        <span class="rounded-full border border-border bg-background px-3 py-1">导出</span>
      </div>
    </div>
    <div class="mt-4 text-sm leading-6 text-muted-foreground">
      这不是把 SDK 简单包一层壳，而是把常见 BI 工作流做成更自然的在线操作路径。
    </div>
  </div>
  <div class="rounded-[28px] border border-primary/20 bg-card p-7 shadow-sm">
    <div class="inline-flex items-center gap-2 rounded-full border border-primary/20 bg-background px-3 py-1 text-[11px] font-bold uppercase tracking-[0.22em] text-secondary-foreground">
      现在已经有的两个工具
    </div>
    <div class="mt-4 text-sm leading-6 text-muted-foreground">
      现在的原型已经能覆盖两个很实用的方向，后面可以继续往平台化体验演进。
    </div>
    <div class="mt-6 space-y-4">
      <div class="rounded-[20px] border border-border bg-background p-4 shadow-sm">
        <div class="text-sm font-semibold text-primary">布局解析</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">提取 Tableau workbook 的布局结构，导出 JSON 或布局结果。</div>
      </div>
      <div class="rounded-[20px] border border-border bg-background p-4 shadow-sm">
        <div class="text-sm font-semibold text-primary">KPI 复制</div>
        <div class="mt-2 text-sm leading-6 text-muted-foreground">复制 KPI 工作表，并只替换局部指标，保留原结构和样式。</div>
      </div>
    </div>
    <div class="mt-6 rounded-[20px] border border-dashed border-primary/25 bg-primary/5 px-5 py-4">
      <div class="text-sm font-semibold text-primary">更长远的创想</div>
      <div class="mt-2 text-sm leading-6 text-muted-foreground">
        协作与版本管理可以作为未来方向来想，但它现在更像是一个创想，不是当前要承诺交付的主功能。
      </div>
    </div>
  </div>
</div>

---
layout: quote
---

# 让 Tableau 开发从手艺活，变成工程化工作流。
