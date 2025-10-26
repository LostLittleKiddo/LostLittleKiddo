# 🚀 Deploy Your Portfolio to GitHub Pages

This guide will help you deploy your portfolio website to GitHub Pages so it's live and accessible to everyone!

## 📋 Prerequisites

- Git installed on your computer
- A GitHub account
- Your portfolio files ready (index.html, styles.css, script.js)

## 🎯 Step-by-Step Deployment

### Method 1: Deploy from Main Branch (Recommended)

#### Step 1: Initialize Git Repository (if not already done)

Open your terminal/command prompt and navigate to your project folder:

```bash
cd c:\Users\benny\Desktop\LostLittleKiddo
```

If you haven't initialized git yet:

```bash
git init
git add .
git commit -m "Initial commit: Portfolio website"
```

#### Step 2: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com)
2. Click the **"+"** icon in the top right
3. Select **"New repository"**
4. Name it: **`LostLittleKiddo`** (or `yourusername.github.io` for a user site)
5. **DO NOT** initialize with README (you already have one)
6. Click **"Create repository"**

#### Step 3: Connect Local Repository to GitHub

Copy the commands from GitHub's "push an existing repository" section:

```bash
git remote add origin https://github.com/LostLittleKiddo/LostLittleKiddo.git
git branch -M main
git push -u origin main
```

#### Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Click **"Pages"** in the left sidebar
4. Under **"Source"**, select:
   - Branch: **`main`**
   - Folder: **`/ (root)`**
5. Click **"Save"**

#### Step 5: Wait for Deployment

- GitHub will start building your site
- Wait 1-2 minutes
- You'll see a message: **"Your site is published at https://LostLittleKiddo.github.io/LostLittleKiddo/"**

#### Step 6: Access Your Live Site! 🎉

Your portfolio is now live at:
```
https://LostLittleKiddo.github.io/LostLittleKiddo/
```

---

### Method 2: Custom Domain (Optional)

If you want a custom domain like `yourname.com`:

1. Buy a domain from a registrar (Namecheap, GoDaddy, etc.)
2. In your repository, create a file named `CNAME` with your domain:
   ```
   yourname.com
   ```
3. In your domain registrar's DNS settings, add:
   - **A Record**: `185.199.108.153`
   - **A Record**: `185.199.109.153`
   - **A Record**: `185.199.110.153`
   - **A Record**: `185.199.111.153`
4. Wait for DNS propagation (up to 24 hours)

---

## 🔄 Updating Your Website

Whenever you make changes:

```bash
# Stage all changes
git add .

# Commit with a message
git commit -m "Update portfolio content"

# Push to GitHub
git push origin main
```

GitHub Pages will automatically rebuild and deploy your site within 1-2 minutes!

---

## ✅ Quick Checklist

- [ ] Repository created on GitHub
- [ ] Local code pushed to GitHub
- [ ] GitHub Pages enabled in Settings
- [ ] Site is live and accessible
- [ ] All links and images work correctly
- [ ] Mobile responsiveness checked

---

## 🐛 Troubleshooting

### Site Not Loading?

1. **Check the URL**: Make sure you're using the correct URL format
   - User site: `https://username.github.io`
   - Project site: `https://username.github.io/repository-name`

2. **Check Settings**: Verify GitHub Pages is enabled in Settings > Pages

3. **Check File Names**: Ensure your main file is named `index.html` (lowercase)

4. **Check Logs**: Go to Actions tab to see deployment status

5. **Clear Cache**: Try opening in incognito/private mode

### Images Not Showing?

- Use relative paths: `./images/photo.jpg` instead of `/images/photo.jpg`
- Or use absolute URLs: `https://your-site.github.io/repository-name/images/photo.jpg`

### CSS/JS Not Loading?

Update your HTML links to use relative paths:

```html
<!-- Use these -->
<link rel="stylesheet" href="./styles.css">
<script src="./script.js"></script>

<!-- Instead of these -->
<link rel="stylesheet" href="/styles.css">
<script src="/script.js"></script>
```

---

## 🎨 Your GitHub Profile README

Your profile README is automatically shown when someone visits:
```
https://github.com/LostLittleKiddo
```

The `README.md` in your `LostLittleKiddo/LostLittleKiddo` repository will display on your profile!

**Important**: For the profile README to work:
- Repository name MUST match your username exactly
- Repository must be **public**
- File must be named `README.md` in the root

---

## 📱 Share Your Portfolio

Once deployed, share your portfolio:

- 🐦 Twitter: "Check out my new portfolio!"
- 💼 LinkedIn: Add to your profile
- 📧 Email signature: Include the link
- 📄 Resume: Add the URL

---

## 🚀 Next Steps

1. **Analytics**: Add Google Analytics to track visitors
2. **SEO**: Add meta tags for better search visibility
3. **Performance**: Use Lighthouse to optimize load times
4. **Custom Domain**: Consider getting a professional domain
5. **Blog**: Add a blog section to share your thoughts
6. **Projects**: Keep adding new projects as you build them

---

## 💡 Pro Tips

- **Regular Updates**: Update your portfolio every few months
- **Mobile First**: Always test on mobile devices
- **Load Speed**: Optimize images and minimize code
- **Accessibility**: Ensure your site works with screen readers
- **Browser Testing**: Test on Chrome, Firefox, Safari, Edge

---

## 📚 Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
- [Markdown Guide](https://www.markdownguide.org/)

---

## 🆘 Need Help?

If you run into issues:
1. Check the [GitHub Pages troubleshooting guide](https://docs.github.com/en/pages/getting-started-with-github-pages/troubleshooting-404-errors-for-github-pages-sites)
2. Search on Stack Overflow
3. Ask in GitHub Community Discussions

---

**🎉 Congratulations on deploying your portfolio!**

Your hard work is now visible to the world. Keep building, keep learning, and keep sharing your awesome projects!
