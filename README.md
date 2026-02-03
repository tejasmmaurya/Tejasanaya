# Tejasanaya 💖

A beautiful Valentine's Day themed interactive webpage.

## 🚨 Quick Start - Deploy to GitHub Pages NOW

**Can't see your HTML at the URL?** Follow these exact steps:

### Step 1: Merge This PR to Main Branch (REQUIRED!)
**IMPORTANT**: GitHub Pages deployment only works from the `main` branch due to environment protection rules.

1. If you're viewing this from a Pull Request, **merge it to the `main` branch**
2. The workflow will NOT deploy from feature branches like `copilot/publish-html-via-github-pages`

### Step 2: Enable GitHub Pages (REQUIRED)
1. Go to **https://github.com/tejasmmaurya/Tejasanaya/settings/pages**
2. Under **"Build and deployment"** section:
   - **Source**: Select **"GitHub Actions"** (NOT "Deploy from a branch")
3. Click **Save** (if there's a save button)

### Step 3: Trigger the Deployment
After merging to `main`, the deployment will happen automatically:
- The workflow runs automatically when you push to `main` branch
- Check deployment status at: **https://github.com/tejasmmaurya/Tejasanaya/actions**
- Look for "Deploy static content to Pages" with a green checkmark ✓

**Manual Trigger** (only works from `main` branch):
1. Go to **https://github.com/tejasmmaurya/Tejasanaya/actions**
2. Click on **"Deploy static content to Pages"** workflow
3. Click the **"Run workflow"** button (top right)
4. Select **`main`** branch (not feature branches)
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

1. ✅ **Check you're on main branch**: Deployment only works from `main` branch, not feature branches
2. ✅ **Check Pages is enabled**: Go to Settings → Pages → Source should be "GitHub Actions"
3. ✅ **Check workflow ran**: Go to Actions tab - you should see a successful green checkmark on `main` branch
4. ✅ **Check the URL**: Must be exactly `https://tejasmmaurya.github.io/Tejasanaya/` (with capital T and capital S)
5. ✅ **Wait**: GitHub Pages can take 2-5 minutes on first deployment
6. ✅ **Clear browser cache**: Try Ctrl+Shift+R (or Cmd+Shift+R on Mac)

**Getting "Branch is not allowed to deploy" error?**

This means you're trying to deploy from a feature branch. Solution:
1. Merge your PR to the `main` branch
2. The workflow will automatically deploy from `main`
3. GitHub's environment protection rules only allow deployment from `main` branch

---

Made with ❤️ by Tejas Maurya