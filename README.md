# 🛍️ Etsy AI Automation — Powered by Mesh API

> **Mesh API Hackathon 2026 Submission | Track: Agents & Automation**

## 🎯 What This Does

A fully automated AI pipeline that creates Etsy digital planner listings from scratch:

1. **OpenAI** generates title, description, 7 image prompts + 10 interior page HTML
2. **Mesh API (GPT Image 1.5)** generates 7 premium preview images
3. **PDF.co** converts HTML into a 10-page luxury planner PDF
4. **Etsy API** uploads listing + images + digital file automatically
5. **Instagram + Pinterest** auto-post the new listing
6. **Telegram + Google Sheets** for alerts and data sync

**Zero manual work. One click. Live Etsy listing in minutes.**

## 🤖 Mesh API Integration

```json
POST https://api.meshapi.ai/v1/images/generations
{
  "model": "openai/gpt-image-1.5",
  "prompt": "{{preview_prompt}}, ultra high quality, studio lighting, 8k, luxury brand aesthetic",
  "size": "1024x1024",
  "quality": "high",
  "n": 1,
  "response_format": "b64_json"
}
```

## 🏗️ Architecture
## 💰 Cost Per Listing

| Component | Cost |
|---|---|
| Mesh API (7 images, high quality) | $0.28 (~₹23) |
| OpenAI text | $0.003 (~₹0.25) |
| PDF.co | $0.02 (~₹1.65) |
| Make.com | ~₹12 |
| **Total** | **~₹37/listing** |

**Selling price ₹750 → Net profit ~₹600+ per sale** 🎉

## 📦 Per Run Output

- 📝 AI-generated Etsy listing (title, description, tags)
- 🖼️ 7 high-quality luxury preview images (via Mesh API)
- 📄 10-page interior PDF planner (black/gold/cream theme)
- 📱 Auto Instagram post
- 📌 Auto Pinterest pin
- 📲 Telegram order alert
- 📊 Google Sheets sync

## 🚀 Business Impact

| Metric | Value |
|---|---|
| Listings per month | 85+ |
| Time per listing (manual) | ~2 hours |
| Time per listing (automated) | ~2 minutes |
| Monthly profit potential | ₹13,000+ |
| Time saved per month | 160+ hours |

## 🛠️ Tech Stack

- **Make.com** — Automation orchestration
- **Mesh API** — AI image generation (GPT Image 1.5)
- **OpenAI** — Text/content generation
- **Etsy API** — Listing management
- **PDF.co** — HTML to PDF
- **Dropbox** — File storage
- **Instagram + Pinterest** — Social auto-posting
- **Telegram Bot** — Alerts
- **Google Sheets** — Data sync

## ⚡ Setup

1. Download `blueprint.json`
2. Import into Make.com (... → Import Blueprint)
3. Connect: OpenAI, Mesh API, Etsy, Dropbox, PDF.co
4. Run Once to test
5. Activate for scheduled auto-runs!

## 👨‍💻 About

**Om** — 15-year-old entrepreneur from Maharashtra, India.
- Class 10 CBSE student
- Etsy seller at **OmbrixStudio**
- Built this to automate his digital products business

> *"I built this because I wanted to spend more time studying and less time manually creating listings."*

## 🏆 Hackathon

- **Track:** Agents & Automation
- **Event:** Mesh API Hackathon 2026
