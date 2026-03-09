# BountyWall Articles

This repo powers **articles.bountywall.com** via Cloudflare Pages.

---

## How to add a new article

1. Copy `_template.html` and rename it with a URL-friendly slug, e.g. `what-is-solana.html`
2. Replace the placeholders:
   - `ARTICLE_TITLE` → your article title (appears in browser tab + page heading)
   - `ARTICLE_DESC` → one sentence description (used by Google for search snippets)
   - `ARTICLE_DATE` → e.g. `March 2025`
   - `ARTICLE_BODY` → your article content in HTML (use `<p>`, `<h2>`, `<h3>`, `<ul>`, `<strong>` etc.)
3. Add a card for it in `index.html` — copy an existing `<a class="article-card">` block and update the href, number, title, and description
4. Commit and push — Cloudflare Pages deploys automatically within ~30 seconds

---

## File naming rules

- Use lowercase letters, numbers, and hyphens only
- No spaces, no underscores
- Always end with `.html`
- Good: `how-to-earn-sol.html`
- Bad: `How To Earn SOL.html`

---

## Article body HTML cheatsheet

```html
<p>Normal paragraph text.</p>

<h2>Section heading</h2>

<h3>Sub-heading</h3>

<ul>
  <li>Bullet point</li>
  <li>Another point</li>
</ul>

<ol>
  <li>Numbered step</li>
  <li>Next step</li>
</ol>

<strong>Bold text</strong>

<a href="https://bountywall.com/earn.html">Link text</a>

<blockquote>A highlighted quote or callout.</blockquote>
```
