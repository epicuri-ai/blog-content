# Setup Instructions for Blog Content Repository

## 🚀 Quick Setup

### Option 1: Using GitHub CLI (Recommended)

1. **Authenticate with GitHub CLI:**

   ```bash
   gh auth login
   ```

2. **Create the repository:**

   ```bash
   gh repo create epicuri-ai/blog-content --public --description "Blog content for Epicuri website"
   ```

3. **Initialize and push content:**
   ```bash
   cd blog-content-setup
   git init
   git add .
   git commit -m "Initial blog content setup"
   git branch -M main
   git remote add origin https://github.com/epicuri-ai/blog-content.git
   git push -u origin main
   ```

### Option 2: Using GitHub Web Interface

1. **Go to GitHub:** https://github.com/orgs/epicuri-ai/repositories
2. **Click "New repository"**
3. **Repository details:**
   - Name: `blog-content`
   - Description: `Blog content for Epicuri website`
   - Visibility: Public
   - Initialize: Don't check any boxes
4. **Create repository**
5. **Upload files:**
   - Upload all files from `blog-content-setup/` folder
   - Commit message: "Initial blog content setup"

## 📁 Repository Structure

After setup, your repository will have:

```
epicuri-ai/blog-content/
├── README.md
├── posts/
│   ├── 2024-01-15-breaking-ais-last-mile.md
│   └── 2024-01-10-economics-autonomous-commerce.md
└── images/
    ├── featured/
    └── inline/
```

## ✅ Verification

After creating the repository, verify it works:

1. **Check the API endpoint:**

   ```
   https://api.github.com/repos/epicuri-ai/blog-content/contents/posts
   ```

2. **Test a blog post:**

   ```
   https://api.github.com/repos/epicuri-ai/blog-content/contents/posts/2024-01-15-breaking-ais-last-mile.md
   ```

3. **Visit your website:**
   - Homepage should show the featured post
   - `/blog` should list all posts
   - Individual post pages should work

## 🔧 Next Steps

1. **Create the repository** using one of the methods above
2. **Test the integration** by visiting your website
3. **Create your first real blog post** in the new repository
4. **Set up team access** for content contributors

## 🎯 Content Workflow

Once set up, creating new blog posts is simple:

1. **Create new `.md` file** in `/posts/` directory
2. **Add frontmatter** with all required fields
3. **Write content** in Markdown
4. **Commit and push** (or create via GitHub web interface)
5. **Content appears automatically** on your website!

## 📞 Need Help?

If you encounter any issues:

- Check that the repository is public
- Verify the API endpoints are accessible
- Ensure frontmatter format is correct
- Test with a simple post first

The GitHub CMS is already configured to point to `epicuri-ai/blog-content` repository!
