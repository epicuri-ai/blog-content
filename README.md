# Epicuri Blog Content

This repository contains all blog content for the [Epicuri website](https://www.epicuri.ai). Content is written in Markdown with YAML frontmatter and automatically synced to the main website.

## 📁 Repository Structure

```
├── README.md
├── posts/
│   ├── 2024-01-15-breaking-ais-last-mile.md
│   ├── 2024-01-10-economics-autonomous-commerce.md
│   └── ...
└── images/
    ├── featured/
    └── inline/
```

## ✍️ Writing Blog Posts

### File Naming Convention

Use the format: `YYYY-MM-DD-slug.md`

Examples:

- `2024-01-15-breaking-ais-last-mile.md`
- `2024-02-01-future-of-ai-agents.md`

### Frontmatter Format

Each blog post must include YAML frontmatter at the top:

```yaml
---
title: "Your Blog Post Title"
slug: "your-blog-post-slug"
excerpt: "A compelling excerpt that appears in previews and social shares..."
featured: false # Set to true for homepage featured post (only ONE at a time)
published: true # Set to false for drafts
publishedDate: "2024-01-15T10:00:00Z"
authorName: "Author Name"
metaDescription: "SEO meta description for search engines..."
tags: ["AI", "Technology", "Blockchain"]
readingTimeMinutes: 8 # Optional - auto-calculated if not provided
featuredImageUrl: "https://images.unsplash.com/photo-..."
---
```

### Content Guidelines

- Use **Markdown** for formatting
- Include a compelling **excerpt** (150-200 characters)
- Add relevant **tags** for categorization
- Use high-quality **featured images** (1200x630px recommended)
- Write engaging **meta descriptions** for SEO

## 🎯 Featured Posts

- **Only ONE post** should have `featured: true` at a time
- Featured posts appear:
  - In the homepage hero section
  - At the top of the blog index page
- To change the featured post:
  1. Set current featured post to `featured: false`
  2. Set new post to `featured: true`

## 📝 Content Workflow

### For Team Members:

1. **Fork** this repository
2. **Create** a new blog post in `/posts/`
3. **Follow** the naming convention and frontmatter format
4. **Submit** a pull request
5. **Review** and merge process

### For Direct Contributors:

1. **Clone** the repository
2. **Create** new posts in `/posts/`
3. **Commit** and **push** changes
4. Content appears on the website automatically

## 🖼️ Images

### Featured Images

- Use high-quality images (1200x630px recommended)
- Host on reliable CDN (Unsplash, Cloudinary, etc.)
- Include in `featuredImageUrl` frontmatter field

### Inline Images

- Store in `/images/inline/` directory
- Reference with relative paths: `![Alt text](../images/inline/image.jpg)`
- Optimize for web (WebP format recommended)

## 🚀 Publishing

### Drafts

- Set `published: false` for work-in-progress posts
- Drafts won't appear on the live website
- Perfect for collaboration and review

### Going Live

1. Set `published: true`
2. Add proper `publishedDate`
3. Commit and push
4. Content appears automatically on the website

## 📊 Content Guidelines

### Writing Style

- **Clear and engaging** - Write for your audience
- **Technical but accessible** - Explain complex concepts simply
- **Action-oriented** - Include clear takeaways
- **SEO-friendly** - Use relevant keywords naturally

### Post Length

- **Minimum**: 800 words
- **Optimal**: 1,200-2,000 words
- **Maximum**: 3,000 words (consider breaking into series)

### Topics

Focus on:

- Autonomous systems and AI agents
- Blockchain and decentralized technologies
- Future of commerce and digital transactions
- Technical deep-dives and case studies
- Industry insights and analysis

## 🔧 Technical Details

This content is consumed by the main website via GitHub API:

- **Repository**: `epicuri-ai/blog-content`
- **API Endpoint**: GitHub Contents API
- **Update Frequency**: Real-time (on page load)
- **Caching**: Browser-level caching applied

## 📞 Support

For questions about content creation or technical issues:

- **Content Questions**: Create an issue in this repository
- **Technical Issues**: Contact the development team
- **Urgent Updates**: Reach out directly to the content team

---

**Ready to contribute?** Check out our [content guidelines](https://github.com/epicuri-ai/blog-content/wiki) and start writing!
