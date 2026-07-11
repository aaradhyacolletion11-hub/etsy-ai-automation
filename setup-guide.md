# Setup Guide — Etsy AI Automation

## Prerequisites
- Make.com account (Basic plan minimum)
- Mesh API account (meshapi.ai)
- OpenAI API account (platform.openai.com)
- Etsy seller account
- Dropbox account
- PDF.co account
- Telegram account (for alerts)
- Google account (for Sheets)

## Step 1 — Get API Keys

### Mesh API Key
1. Go to meshapi.ai
2. Sign up / Login
3. Dashboard → API Keys → Create New Key
4. Copy the key (starts with `mesh_sk_...`)

### OpenAI API Key
1. Go to platform.openai.com
2. API Keys → Create New Key
3. Copy the key (starts with `sk-...`)

### PDF.co API Key
1. Go to pdf.co
2. Sign up → Dashboard → API Key
3. Copy the key

### Telegram Bot Token
1. Open Telegram → search @BotFather
2. Send `/newbot`
3. Follow instructions → copy token
4. Get your Chat ID from @userinfobot

## Step 2 — Import Blueprint in Make.com
1. Download `blueprint.json` from this repo
2. Open Make.com
3. Click "Create a new scenario"
4. Bottom left → `...` → "Import Blueprint"
5. Upload `blueprint.json`

## Step 3 — Connect All Services
After import, connect each module:
- OpenAI module → Add OpenAI connection
- HTTP module (Mesh API) → Add your Mesh API key in Authorization header
- Etsy module → OAuth login with your Etsy account
- Dropbox module → OAuth login
- PDF.co module → Add PDF.co API key
- Telegram module → Add bot token + your chat ID
- Google Sheets → OAuth login + select your sheet

## Step 4 — Test Run
1. Click "Run Once"
2. Check each module for green ticks
3. Verify listing created on Etsy
4. Verify PDF uploaded as digital file
5. Verify 7 images uploaded to listing

## Step 5 — Activate
Once test is successful:
1. Set schedule (recommended: every 8 hours)
2. Toggle scenario ON
3. Sit back and watch listings auto-create! 🎉
