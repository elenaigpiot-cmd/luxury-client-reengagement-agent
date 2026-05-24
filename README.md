# 💎 Luxury Client Re-engagement Agent
> Built with n8n + Claude API (Anthropic) · Autonomous luxury retail automation

**[▶ Watch the demo](#)** ← *(to add Loom link after recording)* !!

---

## The problem
Luxury brands lose high-value clients to silence. A Platinum client hasn't purchased in 90 days — someone needs to reach out, personally, in a way that feels handcrafted. At scale, that's impossible to do manually without it feeling like a mass email.

## What it does
Runs automatically on a schedule. Scans the client database, identifies dormant Platinum clients (90+ days since last purchase), and generates a personalised outreach message for each one — using their name, nationality, purchase history, preferred category, and relationship notes.

**Every message is different. Every message feels personal.**

## How it works

Schedule Trigger (daily)
↓
Google Sheets — reads full client database
↓
Filter — Platinum tier AND 90+ days since last purchase
↓
Claude API — generates personalised outreach per client
↓
Google Sheets — logs messages to Daily Briefing tab

## Sample output

**For Sophie Marchand (Paris, Couture):**
> "Chère Sophie, I've been thinking of you and wanted to share that several pieces from our new arrival have quietly found their way into our atelier before the official launch..."

**For Ahmed Al Rashidi (Leather Goods):**
> "Dear Ahmed, as the spring season unveils a remarkable collection of pieces we have personally reserved with your family in mind..."

**For Tariq Hassan (Timepieces):**
> "Good evening, Mr. Hassan — I have been thinking of you and wanted to reach out personally, as several remarkable timepieces have arrived..."

## Client data used for personalisation
- First name, nationality, city
- VIP tier and total spend
- Last purchase item and amount
- Preferred category and contact channel
- Relationship notes and engagement history
- Birthday

## Tech stack
- **n8n** — workflow orchestration and scheduling
- **Anthropic Claude API** — personalised message generation
- **Google Sheets** — client database and output log
- **Railway** — n8n hosting

## Why this matters
This replaces what would take a client relations team hours every morning. The messages don't read like automation — they read like a personal stylist who knows the client. That's the gap AI closes here.

## About this project
Built as part of my AI engineering portfolio focused on Forward Deployed Engineer roles.

I come from a business background in CX and CRM in luxury retail. I know this problem from the inside. This is me building the solution.

[LinkedIn](https://www.linkedin.com/in/elena-piot-crm) · [GitHub](https://github.com/elenaigpiot-cmd)
