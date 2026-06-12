# ICLNet² Credit Report Prototype

A single-page interactive demo for investors: click start, watch a 4-step
encrypted credit-report pipeline run, get a full TU-format (5-tab) credit
report generated entirely client-side with synthetic data.

## What it does

1. **Start screen** — logo + big "▶ 開始生成信貸報告" button
2. **Click** — animated 4-step pipeline (Parse · Query · Score · Render) runs ~7s
3. **Result** — full credit report appears with 5 tabs: Summary / Personal / Score / Accounts / Inquiries
4. **Replay** — click 重新開始 to roll another synthetic report

All names, HKIDs, phones, addresses, and account numbers are client-side
random — they do not correspond to any real person.

## Stack

- Single self-contained `index.html` (~78 KB)
- Vanilla JS for the report generator and pipeline animation
- opencc-js (CDN) for 繁 → 简 live toggle

## Run locally

Open `index.html` in any modern browser.

## Deploy

Live on Vercel, auto-deploys from `main`.
