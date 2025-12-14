# AffiliateLedger AI™  
_Autonomous Affiliate Commission Accountant_

AffiliateLedger AI™ is an autonomous AI agent concept designed to **track affiliate-driven sales**, **apply commission rules**, and **generate clean monthly payout reports** so founders, course creators, and agencies can pay affiliates accurately and on time—without spreadsheet chaos.

This repository currently contains a **single-page wow-demo UI (`index.html`)** that showcases the vision and feel of the product: an AI-powered **Affiliate Control Room** with a hero section, metrics, and a visual payout snapshot.

---

## 🌌 Overview

**AffiliateLedger AI™** is built to behave like an **AI affiliate accountant**:

- Watches affiliate links, coupon codes, and referral IDs.
- Listens to real-time sales events from platforms like Stripe.
- Reconciles commissions (including recurring, refunds, and disputes).
- Closes the books every month with payout-ready reports.

The current `index.html` focuses on the **front-door experience** – a landing/hero screen that makes visitors say “Wow” and instantly understand the power of an autonomous commission engine.

---

## ✨ Current Demo (Single-File UI)

The current version is a **static, single-file prototype**:

- `index.html`  
  - Full-screen **background image + gradient overlay** for a cinematic, financial-control-room feel.  
  - Glassmorphism cards with neon accents (gold, cyan, magenta, violet).  
  - Bold hero headline: _“Turn affiliate chaos into one-click payouts.”_  
  - Dual CTA buttons:
    - **Launch Live Demo**
    - **Watch 60-Second Overview**
  - Stripe-native / AI / GitHub→Vercel→Firebase badges.
  - Animated **weekly revenue vs commission chart**.
  - “Monthly Payout Snapshot” card with:
    - Top affiliate
    - Average commission rate
    - Refunded amounts
    - On-time payout status
    - AI-style anomaly note.

This page is intentionally designed to act as a **launchpad** for the full SaaS build (Next.js + Firebase + Stripe).

---

## 🧱 Vision for the Full Stack Build

The long-term vision is a multi-tenant SaaS app:

- **GitHub → Vercel → Firebase → Stripe** pipeline.
- **Firebase Auth** for user login.
- **Firestore** to store:
  - Program settings (commission rules, cookie windows).
  - Affiliate records (IDs, coupons, ref params).
  - Transactions (pulled from Stripe webhooks).
  - Commission entries (calculated per transaction).
- **Stripe**:
  - Source of truth for sales events.
  - Billing engine for the SaaS subscription itself.
- **AI Layer (LLM)**:
  - Summarizes monthly reports.
  - Flags anomalies or suspicious activity.
  - Generates plain-language explanations for payout decisions.

The `index.html` serves as the **visual and emotional anchor** for this system.

---

## 🧩 Tech Stack (Current)

Right now, this is a **pure front-end prototype**:

- **HTML5** single-page layout.
- **CSS**:
  - Custom gradients, glow effects, and glassmorphism.
  - Animated grid and bar chart effects.
  - Fully responsive (desktop → mobile).
- **JavaScript (vanilla)**:
  - Simple click handlers for the primary buttons (placeholder alerts).
- **External assets**:
  - Google Fonts: `Space Grotesk`.
  - Font Awesome icons.
  - Background image from Unsplash (remote URL).

No build tools, no bundlers – just open `index.html` in a browser or serve it as a static file.

---

## 📁 File Structure

Current minimal repo structure:

```text
AffiliateLedger-AI/
  ├── index.html       # Wow-demo single-page UI
  └── README.md        # This file
