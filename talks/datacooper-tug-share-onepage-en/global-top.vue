<template>
  <div class="pointer-events-none fixed inset-x-0 top-0 z-40 h-28 bg-[linear-gradient(180deg,rgba(233,230,220,0.9),rgba(233,230,220,0))]" />
</template>

<style>
:root {
  --background: rgb(233, 230, 220);
  --foreground: rgb(61, 57, 41);
  --card: rgba(255, 255, 255, 0.52);
  --card-strong: rgba(255, 255, 255, 0.7);
  --muted-foreground: rgb(120, 116, 101);
  --primary: #c96442;
  --primary-deep: #9d4526;
  --border: rgba(201, 100, 66, 0.28);
  --shadow-soft: 0 18px 50px rgba(125, 94, 70, 0.09);
}

@theme inline {
  --color-background: var(--background);
  --color-foreground: var(--foreground);
  --color-primary: var(--primary);
  --color-border: var(--border);
}

@layer base {
  html,
  body,
  .slidev-layout {
    background:
      radial-gradient(circle at 10% 10%, rgba(201, 100, 66, 0.12), transparent 28%),
      radial-gradient(circle at 92% 14%, rgba(201, 100, 66, 0.1), transparent 26%),
      linear-gradient(135deg, rgba(255, 255, 255, 0.32), rgba(255, 255, 255, 0)),
      var(--background);
    color: var(--foreground);
    font-family: Georgia, Cambria, "Times New Roman", Times, serif;
  }

  .slidev-layout {
    padding: 0;
  }

  .poster-shell {
    position: relative;
    min-height: 100vh;
    overflow: hidden;
  }

  .poster-shell::before {
    content: "";
    position: absolute;
    inset: 30px;
    border: 1px solid rgba(157, 69, 38, 0.12);
    border-radius: 36px;
    pointer-events: none;
  }

  .kicker {
    color: var(--primary-deep);
    letter-spacing: 0.36em;
    text-transform: uppercase;
    font-family: "Segoe UI", Arial, sans-serif;
  }

  .headline-display {
    color: var(--foreground);
    font-family: Georgia, Cambria, "Times New Roman", Times, serif;
    letter-spacing: -0.06em;
    line-height: 0.92;
  }

  .accent-stroke {
    position: relative;
  }

  .accent-stroke::after {
    content: "";
    position: absolute;
    left: 0;
    bottom: 0.08em;
    width: 100%;
    height: 0.22em;
    background: rgba(201, 100, 66, 0.22);
    z-index: -1;
    border-radius: 999px;
  }

  .glass-card {
    background: var(--card);
    border: 1px solid var(--border);
    box-shadow: var(--shadow-soft);
    backdrop-filter: blur(10px);
  }

  .metric-card {
    background: var(--card-strong);
    border: 1px solid rgba(157, 69, 38, 0.16);
    box-shadow: var(--shadow-soft);
  }
}
</style>
