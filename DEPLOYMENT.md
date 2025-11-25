# Deployment Guide

This guide will help you deploy your personal website to GitHub Pages with automatic updates.

## Step 1: Merge Your Changes to Main

1. Go to your GitHub repository: `https://github.com/arjun-b-mohan/site`
2. You should see a notification about the recent push to branch `claude/personal-website-setup-01Vk6hE6zKzUmMRfAcLmQ9mf`
3. Click **"Compare & pull request"** or create a new pull request
4. Review the changes and click **"Create pull request"**
5. Once created, click **"Merge pull request"** to merge to main
6. Click **"Confirm merge"**

## Step 2: Enable GitHub Pages

1. In your GitHub repository, click **Settings** (top menu)
2. In the left sidebar, click **Pages**
3. Under **"Source"**, select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait a few moments, then refresh the page
6. You'll see a message: "Your site is live at `https://arjun-b-mohan.github.io/site/`"

Your website is now deployed!

## Step 3: Making Updates (Edit → Push → Auto-Deploy)

Whenever you want to update your website (add a new book, update your bio, etc.):

### Option A: Edit on GitHub (Easiest)

1. Go to your repository on GitHub
2. Navigate to the file you want to edit (e.g., `books.html`)
3. Click the pencil icon (Edit this file)
4. Make your changes
5. Scroll down and click **"Commit changes"**
6. Your site will automatically update in 1-2 minutes!

### Option B: Edit Locally (More Control)

1. Make your changes to any file locally
2. Commit your changes:
   ```bash
   git add .
   git commit -m "Add new book to reading list"
   ```
3. Push to main:
   ```bash
   git push origin main
   ```
4. GitHub Pages will automatically rebuild and deploy your site in 1-2 minutes!

## Common Updates

### Adding a New Book

Edit `books.html` and add:
```html
<div class="book-item">
    <h3>Book Title</h3>
    <p class="author">by Author Name</p>
    <p>Your thoughts about the book.</p>
</div>
```

### Adding a New Blog Post

Edit `writing.html` and add:
```html
<article class="writing-item">
    <h3><a href="https://your-blog-url.com">Article Title</a></h3>
    <p class="date">Published: January 2025</p>
    <p>Brief description of your article.</p>
</article>
```

### Updating Your Bio

Edit `index.html` and modify the text in the `<section class="bio">` section.

### Adding Your Resume

1. Add your resume PDF file to the repository root as `resume.pdf`
2. Commit and push the file
3. The download link on your homepage will automatically work

## Troubleshooting

**Site not updating?**
- Wait 1-2 minutes for GitHub Pages to rebuild
- Check the "Actions" tab in your repository to see build status
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)

**404 Error?**
- Make sure GitHub Pages is enabled in Settings → Pages
- Verify the source is set to `main` branch and `/ (root)` folder

**Changes not showing?**
- Confirm your changes were pushed to the `main` branch
- Check that the files were actually modified in the repository

## Your Website URL

Once deployed, your website will be available at:
**https://arjun-b-mohan.github.io/site/**

Share this URL on your LinkedIn, resume, or anywhere else!
