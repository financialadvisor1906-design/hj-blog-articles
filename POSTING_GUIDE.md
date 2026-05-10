# Hutcherson Jones Blog — Article Posting Guide

## How to Post a New Article

1. Write your article as a `.md` (Markdown) file
2. Go to your GitHub repo: https://github.com/financialadvisor1906-design/hj-blog-articles
3. Click **"Add file"** → **"Upload files"**
4. Drag your `.md` file in
5. Click **"Commit changes"**
6. Done — the article appears on hutchersonjones.blog within seconds

---

## Article File Format

Every article file must start with a **frontmatter block** (between the `---` lines):

```markdown
---
title: "Your Article Title Here"
slug: your-article-url-slug
category: Tax Strategy
excerpt: "A 1-2 sentence summary of the article that appears on the homepage and in search results."
date: 2026-05-09
readTime: 5
image: https://optional-image-url.com/photo.jpg
---

Your article content starts here...

## Section Heading

More content...
```

---

## Field Reference

| Field | Required | Description | Example |
|-------|----------|-------------|---------|
| `title` | Yes | Article headline. Use quotes if it contains a colon. | `"No Tax on Tips: What It Means"` |
| `slug` | Yes | URL-friendly version of the title (lowercase, hyphens, no spaces) | `no-tax-on-tips-2025` |
| `category` | Yes | Must match one of the nav categories exactly | `Tax Strategy` |
| `excerpt` | Yes | 1-2 sentence summary for homepage cards and SEO | `"Learn how the new..."` |
| `date` | Yes | Publication date in YYYY-MM-DD format | `2026-05-09` |
| `readTime` | No | Estimated reading time in minutes | `5` |
| `image` | No | URL to a header image (leave blank to use a default) | `https://...` |

---

## Available Categories

- `Tax Strategy`
- `New Tax Law`
- `Bookkeeping`
- `IRS Compliance`
- `Small Business`
- `Financial Health`

---

## Markdown Formatting Tips

```markdown
# Heading 1 (use for main title — usually skip this since title is in frontmatter)
## Heading 2 (use for major sections)
### Heading 3 (use for subsections)

**Bold text** for emphasis
*Italic text* for subtle emphasis

> Blockquote for important callouts or quotes

- Bullet point
- Another bullet point

1. Numbered list
2. Second item

| Column 1 | Column 2 |
|----------|----------|
| Data     | Data     |
```

---

## Example Article File

```markdown
---
title: "5 Bookkeeping Mistakes That Cost Small Businesses Money"
slug: bookkeeping-mistakes-small-business
category: Bookkeeping
excerpt: "Most small business owners don't realize they're losing money to simple bookkeeping errors. Here are the five most common mistakes — and how to fix them."
date: 2026-05-15
readTime: 4
---

Running a small business means wearing many hats. But when bookkeeping falls through the cracks, the financial consequences can be serious.

## 1. Mixing Personal and Business Finances

One of the most common mistakes is using a personal bank account for business transactions...

## 2. Not Reconciling Monthly

Bank reconciliation catches errors before they become problems...
```
