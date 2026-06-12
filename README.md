# Blue Bull Capital · ICLNet² — Investor MVP

A bilingual (繁體/简体) investor brief for Blue Bull Capital's ICLNet² — Hong Kong's
proposed third credit seat. The centerpiece is a fully interactive, fully synthetic
credit-report prototype modelled on the TransUnion HK format (5 tabs: Summary,
Personal, Score, Accounts, Inquiries) generated client-side.

## What the prototype does

- **Credit Report Viewer** — click any of the 5 tabs to navigate, click "生成新報告"
  to regenerate. All names, HKIDs, phones, addresses, and account numbers are
  client-side random — they do not correspond to any real person.
- **FinancialGPT Decision Engine** — pick a loan scenario, watch the 4-step
  compliance pipeline run, see the decision card.
- **GBA Cross-Border Flow** — auto-play walks an encrypted handoff through 5 gates.
- **Returns Calculator** — drag the sliders for capital commitment, IRR, hold, hurdle.
- **繁/简 switcher** — toggle the entire page (including dynamically-rendered
  report content) between Traditional and Simplified Chinese.

## Stack

- Single self-contained `index.html` (~100 KB)
- No build step
- Vanilla JS for the report generator, decision engine, GBA flow, calculator
- opencc-js (CDN) for live 繁 → 简 conversion

## Run locally

Open `index.html` in any modern browser, or:

```bash
npx serve .
```

## Deploy

Already deployed to Vercel (auto-deploys from `main`).
