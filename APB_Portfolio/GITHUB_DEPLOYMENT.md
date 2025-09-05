# GitHub Pages Deployment Guide

## Step-by-Step Instructions

### 1. Create a New Repository on GitHub

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **"+"** button in the top right corner
3. Select **"New repository"**
4. Name your repository: `Portfolio` or `yousef-albawab-portfolio`
5. Make sure it's set to **Public** (required for free GitHub Pages)
6. **DO NOT** initialize with README, .gitignore, or license (we already have these files)
7. Click **"Create repository"**

### 2. Upload Your Files

**Option A: Using GitHub Web Interface (Easiest)**
1. On your new repository page, click **"uploading an existing file"**
2. Drag and drop ALL files from your `APB_Portfolio` folder:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md`
   - `package.json`
   - `LICENSE`
   - `DEPLOYMENT.md`
   - `GITHUB_DEPLOYMENT.md`
3. Write a commit message: "Initial portfolio upload"
4. Click **"Commit changes"**

**Option B: Using Git Commands (Advanced)**
```bash
# Open PowerShell in your APB_Portfolio folder
cd "C:\Users\Yousef\Desktop\APB_Portfolio"

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial portfolio upload"

# Add your GitHub repository as origin (replace with your actual repo URL)
git remote add origin https://github.com/YousefAlbawab/Portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **"Settings"** tab (at the top of the repo)
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select **"Deploy from a branch"**
5. Choose **"main"** branch
6. Leave folder as **"/ (root)"**
7. Click **"Save"**

### 4. Access Your Live Portfolio

After a few minutes, your portfolio will be live at:
```
https://YousefAlbawab.github.io/Portfolio
```

(Replace `YousefAlbawab` with your actual GitHub username and `Portfolio` with your repository name)

### 5. Update Your Resume and LinkedIn

Once live, update:
- Your resume with the new portfolio URL
- Your LinkedIn profile to include the portfolio link
- Any job applications with the live portfolio URL

## Troubleshooting

### If GitHub Pages isn't working:
1. Check that your repository is **public**
2. Make sure your main file is named `index.html` (not `Index.html`)
3. Wait 5-10 minutes for changes to propagate
4. Check the Pages settings are correctly configured

### If you need to make changes:
1. Edit files directly on GitHub (click the pencil icon)
2. Or upload new versions of files
3. Changes will automatically update your live site within minutes

### Custom Domain (Optional):
1. Purchase a domain from a registrar (GoDaddy, Namecheap, etc.)
2. In repository Settings > Pages, add your custom domain
3. Update your domain's DNS settings to point to GitHub Pages

## Next Steps After Deployment

1. **Test your live site** thoroughly on different devices
2. **Share the URL** with your network
3. **Submit to job applications** and include in your resume
4. **Monitor traffic** using GitHub's built-in analytics
5. **Update content** as needed by editing files on GitHub

## Quick Reference URLs

- **Your Repository**: `https://github.com/YousefAlbawab/Portfolio`
- **Your Live Site**: `https://YousefAlbawab.github.io/Portfolio`
- **GitHub Pages Docs**: [docs.github.com/pages](https://docs.github.com/pages)

---

🎉 **Congratulations!** Your professional portfolio is now live and accessible worldwide!
