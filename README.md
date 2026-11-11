# WEDA — RIMC Landing Page

One-page landing site for **WEDA – The Winning Edge Defence Academy**, promoting
preparation for the **Rashtriya Indian Military College (RIMC) entrance examination**,
Class VIII entry.

Sibling of the Sainik School / RMS page (`weda-sainik-rms-landing`, branch
`sainik-rms-2026`) — same design system, same logo, same policy pages.

## Two actions only

| Button | Goes to |
|---|---|
| **Apply for Admission** (nav, hero, final CTA, mobile bar) | WhatsApp, pre-filled |
| **Enquire about RIMC** (both course cards) | WhatsApp, naming written vs viva |
| **Register Now** | the Razorpay Payment Page |

No forms, no backend. Three HTML pages, one stylesheet, images.

## Configure

Everything editable lives in the `const WEDA = { … }` block near the bottom of
`index.html`: WhatsApp and phone numbers, the Razorpay Payment Page URL, social
links, policy page paths and the pre-filled WhatsApp messages.

## Images

| File | Where | Status |
|---|---|---|
| `assets/hero-cadets.webp` | Hero | present |
| `assets/rimc-campus.webp` | About RIMC | present — **low-resolution source (515x388)**, replace when a larger one exists |
| `assets/video-thumb.webp` | Video thumbnail | present (from the YouTube video) |

Drop a file in and it appears; no code change needed.

## Facts used on this page

Checked against public RIMCEE sources, November 2026:

- Class VIII entry only, at RIMC Dehradun
- Open to boys and girls
- Entrance twice a year (June and December exams; January and July terms)
- Written examination (Mathematics, English, General Knowledge) → viva voce → medical
- Conducted by the National Testing Agency
- Feeder institution for the NDA and Indian Naval Academy
- Seats are few and allotted state and UT-wise

**No seat count is published on the page.** Sources disagree — 25 per term in older
notices, 35 per term (25 boys, 10 girls) in RIMCEE 2026. Confirm against the current
official notification before putting a number on the page.

## Deploy

Pushes to branch `rimc-2026` are deployed to the Vercel project `weda-rimc-2026`.
