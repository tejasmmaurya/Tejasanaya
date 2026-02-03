# Tejasanaya 💖

A beautiful Valentine's Day themed interactive webpage.

## 🚨 Quick Start - Deploy to GitHub Pages NOW

**Can't see your HTML at the URL?** Follow these exact steps:

### Step 1: Merge This PR (if working in a branch)
If you're viewing this from a Pull Request, merge it to your default branch.

### Step 2: Enable GitHub Pages (REQUIRED)
1. Go to **https://github.com/tejasmmaurya/Tejasanaya/settings/pages**
2. Under **"Build and deployment"** section:
   - **Source**: Select **"GitHub Actions"** (NOT "Deploy from a branch")
3. Click **Save** (if there's a save button)

### Step 3: Trigger the Deployment
Option A - Automatic (after committing this change):
- The workflow will run automatically when you push this commit

Option B - Manual trigger:
1. Go to **https://github.com/tejasmmaurya/Tejasanaya/actions**
2. Click on **"Deploy static content to Pages"** workflow
3. Click the **"Run workflow"** button (top right)
4. Select your branch (copilot/publish-html-via-github-pages or main)
5. Click **"Run workflow"**

### Step 4: Wait and Access
- Wait 1-2 minutes for deployment to complete
- Your site will be live at: **https://tejasmmaurya.github.io/Tejasanaya/**
- If you see a 404, wait another minute and refresh

---

## ⏱️ Display Timing

**Question: "How much time would it take to display?"**

The page uses the following timing configuration:

| Element | Duration | Description |
|---------|----------|-------------|
| **Loading Screen** | 3.5 seconds (3500ms) | Time before the main card appears |
| Loading Fade Out | 600ms | Smooth transition when loading completes |
| Message Typing | 120ms per character | Speed of typing animation for "I ❤️ You Sanaya!" |
| Yes Messages | 2200ms interval | Time between each celebration message |
| Floating Hearts | 7000ms | How long hearts float on screen |

### Customizing Timing

You can easily adjust these timings by editing the `TIMING` configuration object at the top of the `<script>` section in `index.html`:

```javascript
const TIMING = {
  LOADING_DISPLAY_TIME: 3500,    // Loading screen duration
  LOADING_FADE_OUT: 600,         // Fade transition
  TYPING_SPEED: 120,             // Character typing speed
  YES_MESSAGE_INTERVAL: 2200,    // Message interval
  HEART_LIFETIME: 7000           // Heart duration
};
```

---

## 🔧 Troubleshooting

**Still can't see the page?**

1. ✅ **Check Pages is enabled**: Go to Settings → Pages → Source should be "GitHub Actions"
2. ✅ **Check workflow ran**: Go to Actions tab - you should see a successful green checkmark
3. ✅ **Check the URL**: Must be exactly `https://tejasmmaurya.github.io/Tejasanaya/` (with capital T and capital S)
4. ✅ **Wait**: GitHub Pages can take 2-5 minutes on first deployment
5. ✅ **Clear browser cache**: Try Ctrl+Shift+R (or Cmd+Shift+R on Mac)

---

Made with ❤️ by Tejas Maurya