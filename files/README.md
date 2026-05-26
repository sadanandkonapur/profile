# Sadanand Konapur — AI Portfolio

Personal portfolio with a Claude-powered AI chat assistant.

## Deploy to Vercel (Free)

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### 2. Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) → **Sign up with GitHub**
2. Click **"Add New Project"** → Import your repo
3. Click **"Deploy"** (no build settings needed)

### 3. Add your API Key
1. In Vercel dashboard → your project → **Settings → Environment Variables**
2. Add:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** `sk-ant-your-key-here`
3. Click **Save** → Go to **Deployments** → **Redeploy**

Done! Your site is live with a working AI chat. 🎉

Get your API key: https://console.anthropic.com/keys

## File Structure
```
portfolio/
├── index.html       ← Your portfolio page
├── api/
│   └── chat.js      ← Serverless function (proxy to Anthropic)
├── vercel.json      ← Vercel config
├── .gitignore       ← Keeps .env out of GitHub
└── README.md
```
