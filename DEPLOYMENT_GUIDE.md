# 🚀 Free Website Deployment Guide

This guide will help you deploy your Luxury Budget Room website for FREE using popular hosting platforms.

## 📋 Table of Contents
- [Option 1: GitHub Pages (Recommended)](#option-1-github-pages-recommended)
- [Option 2: Netlify](#option-2-netlify)
- [Option 3: Vercel](#option-3-vercel)
- [Option 4: Cloudflare Pages](#option-4-cloudflare-pages)
- [Post-Deployment Steps](#post-deployment-steps)

---

## Option 1: GitHub Pages (Recommended)

### ✅ Pros:
- Completely free
- Easy to set up
- Automatic deployment from GitHub
- Custom domain support

### 📝 Steps:

1. **Create a GitHub Account** (if you don't have one)
   - Go to https://github.com
   - Sign up for free

2. **Create a New Repository**
   - Click the "+" icon → "New repository"
   - Name it: `luxury-budget-room` (or any name)
   - Make it **Public**
   - Click "Create repository"

3. **Upload Your Files**
   
   **Option A: Using GitHub Web Interface**
   - Click "uploading an existing file"
   - Drag and drop all your files:
     - `index.html`
     - `style.css`
     - `images/` folder
   - Click "Commit changes"

   **Option B: Using Git Command Line**
   ```bash
   # Open Terminal and navigate to your project folder
   cd /Users/chutchai.p/Code/House
   
   # Initialize git
   git init
   
   # Add all files
   git add .
   
   # Commit
   git commit -m "Initial commit"
   
   # Add your GitHub repository (replace YOUR_USERNAME)
   git remote add origin https://github.com/YOUR_USERNAME/luxury-budget-room.git
   
   # Push to GitHub
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click "Settings"
   - Scroll to "Pages" in the left sidebar
   - Under "Source", select "main" branch
   - Click "Save"

5. **Your Website is Live! 🎉**
   - URL: `https://YOUR_USERNAME.github.io/luxury-budget-room/`
   - It may take 2-5 minutes to go live

### 🌐 Custom Domain (Optional)
- Buy a domain from Namecheap, GoDaddy, etc.
- In GitHub Pages settings, add your custom domain
- Update DNS records at your domain registrar

---

## Option 2: Netlify

### ✅ Pros:
- Super fast deployment
- Drag-and-drop interface
- Automatic SSL certificate
- Form handling (useful for contact forms)

### 📝 Steps:

1. **Sign Up**
   - Go to https://netlify.com
   - Sign up with GitHub, Email, or GitLab

2. **Deploy**
   
   **Method 1: Drag and Drop (Easiest)**
   - Click "Add new site" → "Deploy manually"
   - Drag your entire `House` folder to the drop zone
   - Done! Your site is live in seconds

   **Method 2: Connect to GitHub**
   - Click "Add new site" → "Import an existing project"
   - Choose "GitHub"
   - Select your repository
   - Click "Deploy site"

3. **Your Website is Live! 🎉**
   - Netlify gives you a random URL like: `random-name-123.netlify.app`
   - You can change this in Site settings → Domain management

### 🌐 Custom Domain
- Go to "Domain settings"
- Click "Add custom domain"
- Follow the instructions

---

## Option 3: Vercel

### ✅ Pros:
- Lightning fast global CDN
- Excellent performance
- Easy GitHub integration

### 📝 Steps:

1. **Sign Up**
   - Go to https://vercel.com
   - Sign up with GitHub (recommended)

2. **Deploy**
   - Click "Add New" → "Project"
   - Import your GitHub repository
   - Click "Deploy"
   - That's it!

3. **Your Website is Live! 🎉**
   - URL: `your-project.vercel.app`

---

## Option 4: Cloudflare Pages

### ✅ Pros:
- Global CDN
- Unlimited bandwidth
- Free SSL
- Very fast

### 📝 Steps:

1. **Sign Up**
   - Go to https://pages.cloudflare.com
   - Create a free account

2. **Deploy**
   - Click "Create a project"
   - Connect to GitHub
   - Select your repository
   - Click "Begin setup" → "Save and Deploy"

3. **Your Website is Live! 🎉**
   - URL: `your-project.pages.dev`

---

## 🎯 Post-Deployment Steps

### 1. Update Your Links
After deployment, update these in your `index.html`:

- **LINE Link**: Replace `https://line.me/ti/p/~yourlineid` with your actual LINE ID
- **Google Maps**: The current map shows Jing Jai Market. Update if needed:
  1. Go to Google Maps
  2. Find your exact location
  3. Click "Share" → "Embed a map"
  4. Copy the iframe code
  5. Replace the existing iframe in `index.html`

### 2. Replace Images
The website currently uses placeholder images. Replace them:

```html
<!-- In index.html, find these and replace the URLs: -->
<img src="https://nftcalendar.io/storage/uploads/2022/02/21/image-not-found_0221202211372462137974b6c1a.png" />

<!-- Replace with your actual images: -->
<img src="images/bedroom.jpg" />
```

**Upload Your Images:**
- Take photos of: bedroom, bathroom, kitchen, living area, building, location
- Name them: `bedroom.jpg`, `bathroom.jpg`, `kitchen.jpg`, etc.
- Upload to the `images/` folder in your repository
- Update the image paths in `index.html`

### 3. Update Contact Information
- Phone number: Already set to `0931817616`
- Address: Update if the current address is incorrect
- LINE ID: Change `~yourlineid` to your actual LINE ID

### 4. Test Your Website
- Open on mobile phone
- Open on tablet/iPad
- Open on desktop
- Test all buttons and links
- Check image loading

### 5. SEO Improvements
After deployment:
- Submit to Google Search Console: https://search.google.com/search-console
- Submit sitemap (optional)
- Share on social media to get initial traffic

---

## 📱 Quick Comparison

| Platform | Speed | Ease | Custom Domain | Best For |
|----------|-------|------|---------------|----------|
| **GitHub Pages** | ⭐⭐⭐⭐ | Easy | Free | Beginners |
| **Netlify** | ⭐⭐⭐⭐⭐ | Easiest | Free | Everyone |
| **Vercel** | ⭐⭐⭐⭐⭐ | Easy | Free | Developers |
| **Cloudflare** | ⭐⭐⭐⭐⭐ | Medium | Free | Advanced |

---

## 🆘 Troubleshooting

### Website not loading?
- Wait 5-10 minutes after deployment
- Clear browser cache (Ctrl/Cmd + Shift + R)
- Check if files are uploaded correctly

### Images not showing?
- Check file paths (case-sensitive!)
- Ensure images are in the `images/` folder
- Verify image URLs in `index.html`

### CSS not applying?
- Check if `style.css` is in the same folder as `index.html`
- Verify the link tag in HTML: `<link rel="stylesheet" href="style.css" />`

---

## 🎉 Recommended: Netlify (Easiest for Beginners)

**Why Netlify:**
1. Drag-and-drop - No coding needed
2. Instant deployment
3. Free SSL certificate
4. Easy to update (just drag new files)

**Quick Start:**
1. Go to https://netlify.com
2. Sign up
3. Drag your `House` folder to Netlify
4. Done! Your site is live!

---

## 📞 Need Help?

If you encounter any issues:
1. Check the platform's documentation
2. Search on Google/YouTube
3. Ask in developer communities (Stack Overflow, Reddit)

---

**Good luck with your deployment! 🚀**

Your website will look amazing and attract many potential tenants! 🏠✨
