# Vinayak Vijay — Personal Academic Website

Personal academic website built on [al-folio](https://github.com/alshedivat/al-folio) and hosted with [GitHub Pages](https://pages.github.com/).

* **Live URL:** [https://vinayakvijay.github.io/](https://vinayakvijay.github.io/)
* **Full Documentation & Maintenance Guide:** [`docs/MAINTENANCE.md`](docs/MAINTENANCE.md)

---

## Quick Controls: Taking Site Offline & Bringing It Back

### Shut Down Website (Offline)
```bash
git push origin --delete gh-pages
gh workflow disable deploy.yml
```

### Bring Website Back Online
```bash
gh workflow enable deploy.yml
gh workflow run deploy.yml
```

---

## Directory Structure

```text
├── _bibliography/     # BibTeX citations for publications (papers.bib)
├── _data/
│   ├── cv.yml         # Education, experience, and skills
│   └── socials.yml    # Google Scholar, GitHub, LinkedIn, X, email links
├── _news/             # Announcements & updates shown on homepage
├── _pages/
│   ├── about.md       # Homepage bio, research interests, and office info
│   ├── blog.md        # Blog list page
│   ├── cv.md          # Curriculum vitae page
│   └── publications.md# Full publications listing
├── _posts/            # Blog posts (with colorful callout styling and MathJax)
├── assets/
│   └── img/           # Profile photo and blog images
└── docs/
    └── MAINTENANCE.md # Detailed operations & editing guide
```

---

## Content Editing Cheatsheet

| Task | File | Notes |
| :--- | :--- | :--- |
| **Update Bio / Interests** | `_pages/about.md` | Markdown formatted with frontmatter |
| **Add New Paper** | `_bibliography/papers.bib` | Standard BibTeX entry (`selected={true}` to feature on home) |
| **New Blog Post** | `_posts/YYYY-MM-DD-title.md` | Supports `{: .block-tip}`, `{: .block-warning}`, Mermaid & LaTeX |
| **Add News Item** | `_news/` | Short inline markdown notice |
| **Update CV** | `_data/cv.yml` | Structured YAML entries |
| **Change Social Links** | `_data/socials.yml` | Handles for Scholar, GitHub, LinkedIn, etc. |

For detailed formatting examples and guides, see [`docs/MAINTENANCE.md`](docs/MAINTENANCE.md).
