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

```
---
title: "Your Article Title Here"
category: "Tax Strategy"
date: 2026-05-15
excerpt: "A 1-2 sentence summary that appears on the homepage card."
image: "https://full-url-to-your-image.jpg"
slug: your-article-url-slug
tags: [tag-one, tag-two, tag-three]
---

Your article content starts here...
```

---

## ⚠️ IMPORTANT: How to Add Images

**Images MUST use full `https://` URLs.** Relative paths like `images/day_04.jpg` will NOT work on the live blog because the blog fetches your Markdown from GitHub and renders it — it has no access to local files.

### Option 1 — Use a Free Image from Unsplash (Easiest)
Go to [unsplash.com](https://unsplash.com), find a photo, right-click → Copy Image Address, and paste the full URL:
```
image: "https://images.unsplash.com/photo-1554224155-6726b3ff858f?w=1200&q=80"
```

### Option 2 — Upload to GitHub and Use the Raw URL
1. In your GitHub repo, create an `images/` folder
2. Upload your image file there (e.g., `images/day_04.jpg`)
3. Click the image in GitHub, then click **"Raw"**
4. Copy the full URL (starts with `https://raw.githubusercontent.com/...`)
5. Use that URL in your frontmatter:
```
image: "https://raw.githubusercontent.com/financialadvisor1906-design/hj-blog-articles/main/images/day_04.jpg"
```

### Option 3 — Use Any Public Image URL
Any image URL that starts with `https://` will work:
- WordPress media uploads: `https://hutchersonjones.blog/wp-content/uploads/...`
- Stock photo CDNs
- Any publicly accessible image link

### In the article body
The same rule applies to images inside the article text:
```
![Alt text](https://full-url-to-image.jpg)   ✅ Works
![Alt text](images/day_04.jpg)               ❌ Broken — relative path
```

---

## Frontmatter Field Reference

| Field | Required | Example |
|-------|----------|---------|
| `title` | ✅ Yes | `"No Tax on Tips: A Game Changer"` |
| `category` | ✅ Yes | `"Tax Strategy"` (see list below) |
| `date` | ✅ Yes | `2026-05-15` |
| `excerpt` | Recommended | `"Short 1-2 sentence summary..."` |
| `image` | Recommended | `"https://images.unsplash.com/..."` |
| `slug` | Recommended | `no-tax-on-tips-2025` |
| `tags` | Optional | `[tax-strategy, 2025-taxes]` |

---

## Valid Categories

Use one of these exactly (spelling and capitalization matter):

- `Tax Strategy`
- `New Tax Law`
- `Bookkeeping`
- `IRS Compliance`
- `Small Business`
- `Financial Health`

---

## Complete Example

```markdown
---
title: "5 Tax Deductions Every Small Business Owner Misses"
category: "Tax Strategy"
date: 2026-05-20
excerpt: "Most small business owners leave money on the table at tax time. Here are five deductions you may be overlooking."
image: "https://images.unsplash.com/photo-1554224155-6726b3ff858f?w=1200&q=80"
slug: 5-tax-deductions-small-business-owners-miss
tags: [tax-strategy, small-business, deductions]
---

Your article content here...

## Section Heading

Paragraph text here.

- Bullet point one
- Bullet point two

![Caption for image](https://images.unsplash.com/photo-1554224155-6726b3ff858f?w=800&q=80)
```
