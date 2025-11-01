# GitHub Pages Setup Instructions

Your Wikipedia vs Grokipedia comparison analysis is now ready for GitHub Pages!

## ✅ Completed Setup

The following files have been configured:

- ✅ `index.html` - Professional landing page with stats and navigation
- ✅ `_config.yml` - GitHub Pages configuration
- ✅ `.nojekyll` - Disables Jekyll processing
- ✅ `.gitignore` - Excludes internal files from publishing
- ✅ `README.md` - Comprehensive documentation
- ✅ Git repository initialized and pushed to GitHub

## 🚀 Enable GitHub Pages (5 steps)

### Step 1: Go to Repository Settings
1. Navigate to https://github.com/davidorban/pedia
2. Click the **Settings** tab (top right)

### Step 2: Access Pages Settings
1. In the left sidebar, click **Pages** (under "Code and automation")

### Step 3: Configure Source
1. Under **Source**, select **Deploy from a branch**
2. Under **Branch**, select:
   - Branch: **main**
   - Folder: **/ (root)**
3. Click **Save**

### Step 4: Wait for Deployment (2-5 minutes)
GitHub will automatically build and deploy your site. You'll see:
- 🟡 Yellow dot = Building
- 🟢 Green dot = Live

### Step 5: Visit Your Site
Your site will be live at:
**https://davidorban.github.io/pedia**

## 📊 What's Published

### Main Landing Page
- `index.html` - Interactive comparison with stats and tables
- Clean design with blue/orange gradient theme
- Mobile-responsive layout

### V2 Analysis (Quality-Focused)
- `/v2_analysis/V2_SYNTHESIS_REPORT.md` - Comprehensive synthesis
- `/v2_analysis/BLOG_POST.md` - Blog-ready post
- `/v2_analysis/eval_*.md` - 7 individual evaluations
- All supporting JSON data files

### V1 Analysis (Coverage-Focused)
- `/output/synthesis_report.md` - Original analysis
- `/output/eval_*.md` - 5 evaluations
- All V1 data files

## 🔗 Key URLs (once live)

**Main Site:**
https://davidorban.github.io/pedia

**V2 Synthesis:**
https://davidorban.github.io/pedia/v2_analysis/V2_SYNTHESIS_REPORT.md

**Blog Post:**
https://davidorban.github.io/pedia/v2_analysis/BLOG_POST.md

**Individual Evaluations:**
- https://davidorban.github.io/pedia/v2_analysis/eval_bitcoin.md
- https://davidorban.github.io/pedia/v2_analysis/eval_cryptocurrency.md
- (etc.)

## 📝 Optional: Custom Domain

If you want to use a custom domain (e.g., pedia.davidorban.com):

1. In GitHub Pages settings, add your custom domain
2. In your DNS provider, add a CNAME record:
   ```
   pedia.davidorban.com → davidorban.github.io
   ```
3. Enable **Enforce HTTPS** in GitHub Pages settings

## 🔄 Updating the Site

Any changes you push to the `main` branch will automatically rebuild the site:

```bash
cd ~/Dev/pedia
git add .
git commit -m "Update analysis"
git push
```

GitHub will automatically redeploy (2-5 minutes).

## 🎨 Customization

### Update Colors
Edit the CSS variables in `index.html`:
```css
:root {
    --blue-primary: #2563eb;
    --orange-primary: #f97316;
    /* etc. */
}
```

### Update Content
- Main page: Edit `index.html`
- Documentation: Edit `README.md`
- Analysis: Edit files in `v2_analysis/` or `output/`

### Add New Sections
Add new cards to `index.html` grid sections for additional content.

## 📊 Analytics (Optional)

To track visitors, add Google Analytics:

1. Get your GA4 tracking ID
2. Add to `index.html` in `<head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## ✅ Verification Checklist

After enabling GitHub Pages, verify:

- [ ] Site loads at https://davidorban.github.io/pedia
- [ ] Landing page displays correctly
- [ ] All internal links work
- [ ] V2 synthesis report is accessible
- [ ] Blog post is accessible
- [ ] Individual evaluations load
- [ ] Mobile responsive (test on phone)
- [ ] No 404 errors

## 🐛 Troubleshooting

### Site Not Loading
- Wait 5 minutes after enabling Pages
- Check Settings > Pages for deployment status
- Ensure `_config.yml` baseurl is `/pedia`

### Broken Links
- All links in markdown files are relative
- Use `/pedia/v2_analysis/file.md` format for absolute links

### Styling Issues
- Clear browser cache
- Check browser console for errors
- Verify `index.html` CSS loaded

### 404 Errors
- Ensure file names match case-sensitivity
- Check `.gitignore` isn't excluding needed files
- Verify files are in the repository

## 📞 Support

If you encounter issues:
1. Check GitHub Pages deployment logs in Settings > Pages
2. Review [GitHub Pages documentation](https://docs.github.com/en/pages)
3. Open an issue in the repository

---

## 🎉 Ready to Go!

Your comparison analysis is fully configured and ready for GitHub Pages. Just enable it in Settings > Pages and your research will be live in minutes!

**Repository:** https://github.com/davidorban/pedia
**Future URL:** https://davidorban.github.io/pedia
