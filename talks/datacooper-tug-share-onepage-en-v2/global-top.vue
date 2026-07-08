<template>
  <div class="pointer-events-none fixed inset-0 overflow-hidden">
    <div class="absolute inset-x-0 top-0 h-24 bg-[linear-gradient(180deg,rgba(233,230,220,0.86),rgba(233,230,220,0))]" />
  </div>
</template>

<style>
:root {
  --background: rgb(233, 230, 220);
  --foreground: rgb(58, 51, 39);
  --muted-foreground: rgb(117, 109, 95);
  --primary: #c96442;
  --primary-deep: #9d4526;
  --primary-soft: rgba(201, 100, 66, 0.16);
  --line: rgba(157, 69, 38, 0.14);
  --card: rgba(255, 255, 255, 0.56);
  --card-strong: rgba(255, 255, 255, 0.72);
  --shadow-soft: 0 20px 60px rgba(111, 86, 61, 0.09);
}

@theme inline {
  --color-background: var(--background);
  --color-foreground: var(--foreground);
  --color-primary: var(--primary);
}

@layer base {
  html,
  body,
  .slidev-layout {
    background:
      radial-gradient(circle at 12% 18%, rgba(201, 100, 66, 0.12), transparent 28%),
      radial-gradient(circle at 90% 14%, rgba(201, 100, 66, 0.1), transparent 26%),
      linear-gradient(135deg, rgba(255, 255, 255, 0.28), rgba(255, 255, 255, 0)),
      var(--background);
    color: var(--foreground);
    font-family: Georgia, Cambria, "Times New Roman", Times, serif;
  }

  .slidev-layout {
    padding: 0;
  }

  .page-shell {
    position: relative;
    min-height: 100vh;
    overflow: hidden;
  }

  .page-shell::before {
    content: "";
    position: absolute;
    inset: 26px;
    border: 1px solid var(--line);
    border-radius: 38px;
    pointer-events: none;
  }

  .ambient {
    position: absolute;
    border-radius: 999px;
    filter: blur(8px);
    pointer-events: none;
  }

  .ambient-left {
    left: -40px;
    top: 180px;
    width: 220px;
    height: 220px;
    background: radial-gradient(circle, rgba(201, 100, 66, 0.14), rgba(201, 100, 66, 0));
  }

  .ambient-right {
    right: -30px;
    bottom: 80px;
    width: 280px;
    height: 280px;
    background: radial-gradient(circle, rgba(201, 100, 66, 0.13), rgba(201, 100, 66, 0));
  }

  .eyebrow-row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 1rem;
    flex-wrap: wrap;
  }

  .eyebrow-pill,
  .eyebrow-note {
    border: 1px solid rgba(157, 69, 38, 0.18);
    background: rgba(255, 255, 255, 0.56);
    border-radius: 999px;
    padding: 0.6rem 1rem;
    font-family: "Segoe UI", Arial, sans-serif;
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.24em;
    text-transform: uppercase;
    color: var(--primary-deep);
    box-shadow: var(--shadow-soft);
  }

  .micro-kicker,
  .panel-kicker,
  .card-label,
  .positioning-label,
  .sequence-index {
    font-family: "Segoe UI", Arial, sans-serif;
    letter-spacing: 0.24em;
    text-transform: uppercase;
  }

  .micro-kicker,
  .panel-kicker,
  .positioning-label,
  .card-label {
    color: var(--primary-deep);
    font-size: 0.72rem;
    font-weight: 700;
  }

  .hero-title {
    margin: 0;
    font-size: clamp(3.7rem, 7vw, 6.4rem);
    line-height: 0.92;
    letter-spacing: -0.07em;
    font-weight: 900;
    color: var(--foreground);
  }

  .hero-highlight {
    position: relative;
    display: inline-block;
    z-index: 0;
  }

  .hero-highlight::after {
    content: "";
    position: absolute;
    left: 0;
    bottom: 0.08em;
    width: 100%;
    height: 0.22em;
    border-radius: 999px;
    background: rgba(201, 100, 66, 0.24);
    z-index: -1;
  }

  .hero-copy {
    font-size: 1.18rem;
    line-height: 1.9rem;
    color: var(--muted-foreground);
  }

  .info-card,
  .sequence-card,
  .positioning-box,
  .story-panel {
    box-shadow: var(--shadow-soft);
    backdrop-filter: blur(10px);
  }

  .info-card {
    background: var(--card-strong);
    border: 1px solid rgba(157, 69, 38, 0.14);
    border-radius: 28px;
    padding: 1.25rem;
  }

  .card-title {
    margin-top: 0.9rem;
    font-size: 2rem;
    line-height: 1;
    letter-spacing: -0.05em;
    font-weight: 900;
    color: var(--foreground);
  }

  .card-copy {
    margin-top: 0.8rem;
    font-size: 0.96rem;
    line-height: 1.65;
    color: var(--muted-foreground);
  }

  .story-panel {
    position: relative;
    min-height: 100%;
    border-radius: 34px;
    border: 1px solid rgba(157, 69, 38, 0.16);
    background: var(--card);
    padding: 1.75rem;
  }

  .orbit {
    position: absolute;
    border-radius: 999px;
    border: 1px solid rgba(201, 100, 66, 0.2);
  }

  .orbit-one {
    top: 1.5rem;
    right: 1.4rem;
    width: 6rem;
    height: 6rem;
  }

  .orbit-two {
    top: 2rem;
    right: 2rem;
    width: 6rem;
    height: 6rem;
    border-color: rgba(201, 100, 66, 0.1);
  }

  .sequence-card {
    border-radius: 24px;
    background: rgba(255, 255, 255, 0.68);
    padding: 1.2rem 1.2rem 1.1rem;
  }

  .sequence-index {
    font-size: 0.72rem;
    font-weight: 800;
    color: var(--primary-deep);
  }

  .sequence-title {
    margin-top: 0.5rem;
    font-size: 1.6rem;
    line-height: 1.1;
    letter-spacing: -0.04em;
    font-weight: 900;
    color: var(--foreground);
  }

  .sequence-copy,
  .positioning-copy {
    margin-top: 0.55rem;
    font-size: 0.95rem;
    line-height: 1.7;
    color: var(--muted-foreground);
  }

  .sequence-card-accent {
    background: linear-gradient(135deg, rgba(201, 100, 66, 0.95), rgba(157, 69, 38, 0.92));
  }

  .sequence-card-accent .sequence-index,
  .sequence-card-accent .sequence-title,
  .sequence-card-accent .sequence-copy {
    color: white;
  }

  .sequence-card-accent .sequence-copy {
    opacity: 0.86;
  }

  .positioning-box {
    border: 1px solid rgba(157, 69, 38, 0.14);
    border-radius: 24px;
    background: rgba(255, 255, 255, 0.62);
    padding: 1.2rem 1.25rem;
  }

  .timeline-title {
    margin: 0;
    font-size: clamp(2.65rem, 4.2vw, 4.3rem);
    line-height: 0.96;
    letter-spacing: -0.06em;
    font-weight: 900;
    color: var(--foreground);
  }

  .timeline-intro {
    max-width: 34rem;
    font-size: 1rem;
    line-height: 1.75;
    color: var(--muted-foreground);
  }

  .summary-box,
  .timeline-panel,
  .timeline-card,
  .takeaway-box {
    box-shadow: var(--shadow-soft);
    backdrop-filter: blur(10px);
  }

  .summary-box,
  .takeaway-box {
    border: 1px solid rgba(157, 69, 38, 0.14);
    border-radius: 24px;
    background: rgba(255, 255, 255, 0.64);
    padding: 1.1rem 1.15rem;
  }

  .summary-label {
    font-family: "Segoe UI", Arial, sans-serif;
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.24em;
    text-transform: uppercase;
    color: var(--primary-deep);
  }

  .summary-copy {
    margin-top: 0.6rem;
    font-size: 0.95rem;
    line-height: 1.7;
    color: var(--muted-foreground);
  }

  .timeline-panel {
    position: relative;
    min-height: 100%;
    border-radius: 34px;
    border: 1px solid rgba(157, 69, 38, 0.16);
    background: var(--card);
    padding: 1.6rem;
  }

  .timeline-strip {
    position: relative;
  }

  .timeline-line {
    position: absolute;
    left: 0;
    right: 0;
    top: 1.15rem;
    height: 2px;
    background: linear-gradient(90deg, rgba(201, 100, 66, 0.22), rgba(157, 69, 38, 0.32));
  }

  .timeline-grid {
    position: relative;
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
  }

  .timeline-card {
    position: relative;
    min-height: 11.8rem;
    border-radius: 24px;
    background: rgba(255, 255, 255, 0.72);
    padding: 2.35rem 1rem 1rem;
  }

  .timeline-dot {
    position: absolute;
    top: 0.78rem;
    left: 1rem;
    width: 0.82rem;
    height: 0.82rem;
    border-radius: 999px;
    background: var(--background);
    border: 2px solid var(--primary);
  }

  .timeline-dot-accent {
    background: var(--primary);
  }

  .timeline-date {
    font-family: "Segoe UI", Arial, sans-serif;
    font-size: 0.66rem;
    font-weight: 700;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--primary-deep);
  }

  .timeline-stage {
    margin-top: 0.55rem;
    font-size: 1.35rem;
    line-height: 1.05;
    letter-spacing: -0.04em;
    font-weight: 900;
    color: var(--foreground);
  }

  .timeline-copy {
    margin-top: 0.62rem;
    font-size: 0.87rem;
    line-height: 1.55;
    color: var(--muted-foreground);
  }

  .timeline-card-accent {
    background: linear-gradient(135deg, rgba(201, 100, 66, 0.96), rgba(157, 69, 38, 0.92));
  }

  .timeline-card-accent .timeline-date,
  .timeline-card-accent .timeline-stage,
  .timeline-card-accent .timeline-copy {
    color: white;
  }

  .timeline-card-accent .timeline-copy {
    opacity: 0.88;
  }

  .takeaway-box {
    background: rgba(255, 255, 255, 0.58);
  }

  @media (max-width: 960px) {
    .page-shell::before {
      inset: 16px;
      border-radius: 26px;
    }

    .hero-title {
      font-size: clamp(3.2rem, 12vw, 4.6rem);
    }

    .timeline-grid {
      grid-template-columns: 1fr;
    }

    .timeline-line {
      display: none;
    }

    .timeline-card {
      min-height: auto;
    }
  }
}
</style>
