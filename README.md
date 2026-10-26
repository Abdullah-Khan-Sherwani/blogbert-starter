# BlogBERT Starter Blog Template

A Jekyll blog in the BlogBERT style. Copy it with **Use this template**, publish it free on GitHub Pages, and connect it to BlogBERT so new posts arrive by themselves.

---

## Set up in five minutes

### 1. Create Your Repository
Click the green **"Use this template"** button at the top of this repository (or choose **Create a new repository**) to copy this template into your own GitHub account.

### 2. Enable GitHub Pages
In your newly created repository:
1. Navigate to **Settings** &gt; **Pages** (in the left sidebar).
2. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`.
   - **Branch**: Select `main` (or your default branch) and `/ (root)`.
3. Click **Save**.
Your blog will be live at `https://<your-username>.github.io/<your-repo-name>/` (or `https://<your-username>.github.io` for user/organization pages) a minute or two later.

### 3. Connect to BlogBERT
1. Sign in at [blogbert.inferya.com](https://blogbert.inferya.com/login) with Google and fill in your site.
2. Under **Publishing**, click **Connect GitHub**.
3. Install the official **BlogBERT GitHub App** on your account and grant access to your new blog repository.
4. When prompted for the publishing preset, choose **Jekyll**.
   - Posts Directory: `_posts`
   - Images Directory: `assets/images/blog`
   - Image URL Prefix: `/assets/images/blog`
   - URL Pattern: `/blog/{slug}/`
5. BlogBERT researches topics, writes each post with its sources, and commits it to `_posts/`. GitHub Pages rebuilds the site on every commit.

The full guide is at [blogbert.inferya.com/help/new-blog](https://blogbert.inferya.com/help/new-blog).

---

## Customizing Your Blog

All site metadata and branding live in `_config.yml`:

```yaml
title: "My Blog"              # Your blog's name
description: "My insights..."  # Short tagline for search engines & social cards
author: "Your Name"           # Used in footer & copyright
url: ""                       # e.g. "https://username.github.io"
baseurl: ""                   # e.g. "/my-blog" if repository is not username.github.io
accent_color: "#b3122b"       # Hex color for brand accents & links
```

### Writing Posts Manually
If you want to write posts by hand alongside BlogBERT's autopilot:
1. Create a Markdown file in `_posts/` with the naming format `YYYY-MM-DD-your-slug.md`.
2. Add the standard YAML front matter keys:
   ```yaml
   ---
   title: "Your Post Title"
   description: "A short 1-2 sentence summary for search engines."
   date: 2026-10-26 12:00:00 +0000
   slug: "your-slug"
   image: "/assets/images/blog/your-hero-image.jpg"
   image_alt: "Descriptive alt text for the hero image"
   canonical: "https://yourdomain.com/blog/your-slug/"
   tags:
     - Technology
     - Guides
   ---
   ```
3. Commit and push to `main`. GitHub Pages handles the rest.

---

## Architecture & Features

- **GitHub Pages Safe Mode**: Only uses plugins on GitHub's official Pages allowlist:
  - `jekyll-seo-tag`: Automated OpenGraph, Twitter Cards, and schema markup
  - `jekyll-feed`: Atom RSS feed at `/feed.xml`
  - `jekyll-sitemap`: XML sitemap generated at `/sitemap.xml`
- **Zero JavaScript**: High performance, zero tracking cookies, fast loading.
- **Responsive Layout**: Designed for mobile (360px), tablet (768px), and desktop (1280px).
- **Dark Mode**: Built-in support for OS light/dark appearance preferences.

---

## License

This starter template is open source and available under the [MIT License](LICENSE).
