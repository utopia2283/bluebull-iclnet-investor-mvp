# ICLNet² — Investor Prototype

Single-page interactive credit-report demo. Investors pick a subject (個人 / 機構),
choose a sample applicant or fill in custom data, watch a 4-step encrypted pipeline
run, and get a full TU-format 5-tab credit report — all generated client-side with
synthetic data.

## Flow

1. **Start** — headline + input section appears
2. **Input** — toggle 個人 / 機構, pick one of 4 samples per type, or open
   the 自行輸入 form and fill your own. A sticky confirm bar shows the
   pick and enables the 開始生成 button.
3. **Pipeline** — 4 animated steps (Parse · Query · Score · Render) with
   live readout + progress bar
4. **Result** — full credit report (Summary / Personal / Score / Accounts /
   Inquiries) generated consistent with the chosen input

## Sample data drives the report

The 4 individual samples (Grade A, D, B, J) and 4 institution samples
(Grade A, C, F, D) drive the score, accounts, and inquiries in the
generated report — so investors can see the same system produce
different outputs for different subjects.

## Stack

- Single self-contained `index.html` (~103 KB)
- Vanilla JS for the report generator, pipeline, and input flow
- opencc-js (CDN) for 繁 → 简 live toggle

## Run locally

Open `index.html` in any modern browser.
