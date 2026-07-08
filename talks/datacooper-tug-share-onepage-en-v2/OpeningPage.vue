<template>
  <div class="page-shell">
    <div class="ambient ambient-left"></div>
    <div class="ambient ambient-right"></div>

    <div class="mx-auto flex min-h-screen max-w-[1380px] flex-col px-8 py-8 md:px-14 md:py-10">
      <div class="eyebrow-row">
        <div class="eyebrow-pill">Datacooper · Tableau User Group</div>
        <div class="eyebrow-note">English Timeline Slide</div>
      </div>

      <div class="mt-8 grid grid-cols-12 gap-8">
        <div class="col-span-12 md:col-span-4">
          <p class="micro-kicker">cwtwb Development History</p>
          <h1 class="timeline-title mt-4">
            A Four-Month Shift
            <br />
            from Prototype
            <br />
            to Engineering Toolkit
          </h1>
          <p class="timeline-intro mt-6">
            This timeline shows how cwtwb evolved from a basic Tableau workbook generator into an AI-oriented workbook engineering toolkit, then narrowed back toward a more stable core.
          </p>

          <div class="summary-box mt-7">
            <div class="summary-label">Core Arc</div>
            <p class="summary-copy">
              Build the foundation, expand into agent workflows, strengthen validation and packaging, experiment with guided authoring, then converge back to dependable workbook engineering.
            </p>
          </div>
        </div>

        <div class="col-span-12 md:col-span-8">
          <div class="timeline-panel">
            <div class="panel-kicker">Timeline</div>

            <div class="timeline-strip mt-8">
              <div class="timeline-line"></div>

              <div class="timeline-grid">
                <article class="timeline-card">
                  <div class="timeline-dot"></div>
                  <div class="timeline-date">2026-02-27 → 2026-02-28</div>
                  <h2 class="timeline-stage">Foundation</h2>
                  <p class="timeline-copy">
                    The project starts with TWB editing, chart creation, dashboard support, and the first MCP surface.
                  </p>
                </article>

                <article class="timeline-card">
                  <div class="timeline-dot"></div>
                  <div class="timeline-date">2026-03-02 → 2026-03-06</div>
                  <h2 class="timeline-stage">Productization</h2>
                  <p class="timeline-copy">
                    Zero-config templates, runtime validation, test DSLs, and module refactors turn a scriptable idea into a usable package.
                  </p>
                </article>

                <article class="timeline-card">
                  <div class="timeline-dot"></div>
                  <div class="timeline-date">2026-03-06 → 2026-03-17</div>
                  <h2 class="timeline-stage">Agent-First Expansion</h2>
                  <p class="timeline-copy">
                    Skills, capability catalogs, recipe APIs, styling controls, and richer charting make the toolkit far more AI-friendly.
                  </p>
                </article>

                <article class="timeline-card">
                  <div class="timeline-dot"></div>
                  <div class="timeline-date">2026-03-17 → 2026-04-22</div>
                  <h2 class="timeline-stage">Validation and Packaging</h2>
                  <p class="timeline-copy">
                    TWBX support, XSD validation, safe save flows, and migration tooling push the project toward reliable delivery.
                  </p>
                </article>

                <article class="timeline-card">
                  <div class="timeline-dot"></div>
                  <div class="timeline-date">2026-03-21 → 2026-06-27</div>
                  <h2 class="timeline-stage">Guided Authoring Experiment</h2>
                  <p class="timeline-copy">
                    The project explores datasource-first guided runs, execution plans, and human-in-the-loop authoring before later shrinking that surface.
                  </p>
                </article>

                <article class="timeline-card timeline-card-accent">
                  <div class="timeline-dot timeline-dot-accent"></div>
                  <div class="timeline-date">2026-06-18 → 2026-06-27</div>
                  <h2 class="timeline-stage">Convergence to Core</h2>
                  <p class="timeline-copy">
                    Cloud validation and REST semantic checks mature the output pipeline, while dormant guided authoring is removed to keep the package focused.
                  </p>
                </article>
              </div>
            </div>

            <div class="takeaway-box mt-8">
              <div class="positioning-label">Talk Takeaway</div>
              <p class="positioning-copy">
                The most important pattern is not feature growth alone. It is the repeated move from capability expansion back to product focus, reliability, and clearer boundaries.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
