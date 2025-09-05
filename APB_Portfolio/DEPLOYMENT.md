# Deployment Guide

## Quick Deploy Options

### 1. GitHub Pages (Recommended)
1. Create a new repository on GitHub
2. Upload all files to the repository
3. Go to Settings > Pages
4. Select "Deploy from a branch" and choose "main"
5. Your site will be available at `https://yourusername.github.io/repository-name`

### 2. Netlify
1. Visit [netlify.com](https://netlify.com)
2. Drag and drop the entire portfolio folder
3. Your site will be live with a custom URL
4. Optional: Connect to GitHub for automatic deployments

### 3. Vercel
1. Visit [vercel.com](https://vercel.com)
2. Import from GitHub or upload files
3. Deploy with zero configuration
4. Automatic HTTPS and global CDN

### 4. Firebase Hosting
```bash
# Install Firebase CLI
npm install -g firebase-tools

# Login and initialize
firebase login
firebase init hosting

# Deploy
firebase deploy
```

### 5. Custom Domain Setup
After deploying to any platform:
1. Purchase a domain from a registrar
2. Update DNS settings to point to your hosting provider
3. Configure SSL certificate (usually automatic)

## Pre-Deployment Checklist

- [ ] Test all links and navigation
- [ ] Verify responsive design on different devices
- [ ] Check loading speed and optimize if needed
- [ ] Update contact information
- [ ] Test form submissions (if any)
- [ ] Validate HTML and CSS
- [ ] Check accessibility compliance
- [ ] Optimize images for web
- [ ] Set up analytics (Google Analytics)
- [ ] Configure SEO meta tags

## Local Testing
```bash
# Option 1: Python (if installed)
python -m http.server 8000

# Option 2: Node.js serve
npx serve .

# Option 3: VS Code Live Server extension
# Install Live Server extension and right-click index.html
```

## Performance Optimization
- Minify CSS and JavaScript for production
- Compress images (use WebP format when possible)
- Enable gzip compression on server
- Set up caching headers
- Use a CDN for static assets

## Monitoring
After deployment, monitor:
- Site uptime and performance
- User analytics and behavior
- Contact form submissions
- SEO rankings and traffic

## Backup Strategy
- Keep source code in version control (Git)
- Regular backups of the live site
- Document any custom configurations
- Save deployment credentials securely
