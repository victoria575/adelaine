# Adelaine — AI Tarot Reader

Powered by Altiora. Built on Claude.

## Deploy to Vercel in 3 steps

### 1. Push to GitHub
Create a new GitHub repo and push these files:
```
adelaine/
  api/chat.js
  index.html
  vercel.json
  README.md
```

### 2. Connect to Vercel
- Go to https://vercel.com/new
- Import your GitHub repo
- Click Deploy

### 3. Add your API key
- In Vercel dashboard → Settings → Environment Variables
- Add: `ANTHROPIC_API_KEY` = your key from console.anthropic.com
- Redeploy

That's it. Adelaine is live.

## To embed on Altiora website
```html
<iframe src="https://your-adelaine-url.vercel.app" width="100%" height="700px" frameborder="0"></iframe>
```

## To capture emails to Google Sheets
In `index.html`, find the `unlock()` function and add a fetch call to your Google Apps Script webhook.
