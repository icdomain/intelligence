# Independent Compute Domain Intelligence Bureau

GitHub Pages site for the Independent Compute Domain Intelligence Bureau (ICDIB). Built with Jekyll.

---

## Directory Structure

```
/
├── index.md              # Language detection & redirect only (no content)
├── _config.yml           # Jekyll config
├── _layouts/
│   ├── default.html      # Base layout
│   └── post.html         # Post layout
├── _templates/           # Source of truth for new files (see below)
│   ├── page-ja.md        # Template for new pages
│   └── post-ja.md        # Template for new posts
├── _posts/               # All posts (mixed formats — see below)
├── en/                   # English section pages
│   ├── index.md
│   ├── archives.md
│   ├── strategic-forecasting.md
│   └── information-discernment.md
└── ja/                   # Japanese section pages (mirrors en/)
    └── (same structure)
```

---

## Language Routing

`index.md` at the root detects the browser language (`navigator.language`) and redirects to `/en/` or `/ja/`. It contains no content.

Each post/page declares its language via the `lang:` front matter field. Section pages (under `en/` and `ja/`) filter posts by `lang` using Liquid.

---

## Post Format — New (Canonical)

New posts come in **pairs**: one `-en.md` and one `-ja.md` with the same slug.

```
_posts/YYYY-MM-DD-slug-en.md
_posts/YYYY-MM-DD-slug-ja.md
```

Use `_templates/post-ja.md` as the starting point and create both files. Key front matter:

```yaml
layout: post
title: ...
description: ...              # under 120 characters
permalink: /ja/archives/YYYY/MM/DD/slug/
lang: ja                      # or "en" for the English file
alt_lang_url: /en/archives/YYYY/MM/DD/slug/   # points to the other language
date: YYYY-MM-DDTHH:MM:SSZ
last_modified_at: YYYY-MM-DDTHH:MM:SSZ
author: founder
categories: [CATEGORY]        # see Categories below
tags: [tag1, tag2]
```

For the `-en.md` file, swap `lang: ja` → `lang: en`, and swap the `permalink` / `alt_lang_url` paths accordingly (`/ja/` ↔ `/en/`).

---

## Post Format — Legacy (Exception)

Posts created before the `-en/-ja` naming convention are **single files** with no `-en` or `-ja` suffix. They have no `alt_lang_url` field.

These are archived records and should not be used as a template for new content.

---

## Categories

| Category | Used for |
|---|---|
| `strategic-forecasting` | Strategic forecasting reports and analyses |
| `information-discernment` | Information literacy content for the age of AI |

---

## Adding New Content

1. Copy `_templates/post-ja.md` for posts, `_templates/page-ja.md` for section pages.
2. Create both `-en.md` and `-ja.md` files.
3. Fill in `title`, `description`, `permalink`, `alt_lang_url`, `date`, `categories`, `tags`.
4. Write the body in the appropriate language for each file.
