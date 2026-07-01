# Neil Xu Blog

This is a standalone Quarto blog intended to be published at:

<https://blog.neilzxu.me>

## Local editing

Install Quarto from:

<https://quarto.org/docs/get-started/>

Install the VS Code extension:

<https://quarto.org/docs/tools/vscode/>

Then preview the site:

```bash
quarto preview
```

The source files are `.qmd` documents. They support Markdown, TeX math,
citations, executable code blocks, and Quarto's visual editor in VS Code.

## Writing a post

Create a folder under `posts/`:

```text
posts/my-post/index.qmd
```

Use front matter like:

```yaml
---
title: "Post title"
description: "Short summary for listings and social cards."
author: "Neil Xu"
date: "2026-07-01"
categories: [statistics, machine-learning]
---
```

Math works with `$...$` and `$$...$$`.

## Deployment

Create a GitHub repository named `neilzxu-blog`, push this directory as the
repository root, and enable GitHub Pages. The included workflow publishes to
the `gh-pages` branch on every push to `main`.

In the repository Pages settings, set the custom domain to:

```text
blog.neilzxu.me
```

In Namecheap DNS for `neilzxu.me`, add:

```text
Type:  CNAME Record
Host:  blog
Value: neilzxu.github.io
TTL:   Automatic
```

After DNS propagates, enable "Enforce HTTPS" in GitHub Pages settings.
