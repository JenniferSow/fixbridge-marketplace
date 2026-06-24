# 🔗 FixBridge — On-Demand Business Support Marketplace

> Connect your business to vetted experts on demand. No contracts. Pay per engagement.

**[🚀 Live Demo](https://JenniferSow.github.io/fixbridge-marketplace/fixbridge-v2.html)** &nbsp;|&nbsp; Built by Jennifer Sowell

---

## 📌 Overview

FixBridge is a full-stack single-page web application that simulates a B2B service marketplace — connecting businesses that need help to expert service providers across IT, Legal, Accounting, HR, Marketing, and Operations. Businesses pay only for what they use, with no long-term contracts required.

This project was designed and built from scratch as a portfolio piece showcasing UI/UX design, JavaScript application architecture, API integration, and product thinking.

---

## ✨ Features

### 🔐 Authentication System
- Sign In and Create Account flows
- Role-based onboarding: **Business Owner** or **Service Provider**
- Demo login buttons for instant exploration of both user types
- Session-aware navigation — sidebar and pages adjust based on role

### 🤖 AI-Powered Provider Matching
- Integrated with the **Anthropic Claude API** (claude-sonnet-4-6)
- Business submits a trouble ticket with title, description, category, budget, and urgency
- Claude analyzes the issue and returns the **top 3 ranked providers** with match scores (0–100%) and specific reasoning
- Real-time streaming with animated loading state

### 💳 Payment Flow
- Three payment methods: **Credit/Debit Card**, **ACH Bank Transfer**, **Mobile Wallet**
- Itemized invoice: hourly rate × hours + 5% platform fee
- Escrow protection model — funds held until work is confirmed complete
- Payment confirmation screen with unique reference number

### 🔧 Provider Portal (Dual-Role Platform)
- Separate dashboard for service providers
- Incoming request feed with Accept / Decline actions
- Earnings dashboard with animated weekly bar chart
- Profile editor: update services, hourly rate, skills, availability, and tags

### 🛒 Business Marketplace
- Browse 8 vetted provider cards across 6 categories
- Filter by category, search by keyword, sort by rating / price / response time
- Provider detail modal with skills, SLA, job history, and direct connect
- Save providers to favorites
- Submit trouble tickets with urgency levels (Low / Medium / High)
- Active ticket tracker with status indicators (Open / In Progress / Resolved)
- Live provider count with real-time animation

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox, animations) |
| Logic | Vanilla JavaScript (ES6+) |
| AI Integration | Anthropic Claude API (`claude-sonnet-4-6`) |
| Fonts | Google Fonts — Sora + Inter |
| Hosting | GitHub Pages |

> No frameworks, no build tools, no dependencies — fully self-contained in a single HTML file.

---

## 🚀 Getting Started

### View it live
Visit the live demo link at the top of this README.

### Run it locally
```bash
git clone https://github.com/JenniferSow/fixbridge-marketplace.git
cd fixbridge-marketplace
open fixbridge-v2.html
```
No install needed — just open the file in any modern browser.

---

## 💡 How the AI Matching Works

When a business submits a ticket, the app sends a structured prompt to the Claude API containing the issue details and full provider list. Claude returns the top 3 ranked providers with match scores and specific reasoning.
