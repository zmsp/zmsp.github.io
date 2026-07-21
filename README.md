# zmsp.github.io

---

## 🚀 Quick Start & How to Serve

### 1. Installation

Ensure you have Ruby, Bundler, and Node.js installed on your system.

```bash
# Install Ruby dependencies
bundle install

```

### 2. Run Local Development Server

To preview the website locally with auto-regeneration on file changes:

```bash
bundle exec jekyll serve
```

Or run with LiveReload for automatic browser refreshing:

```bash
bundle exec jekyll serve --livereload
```

Once running, access the local site at **[http://127.0.0.1:4000/](http://127.0.0.1:4000/)**.

---

## ✅ Pre-commit Check

Run the following checks before committing changes to ensure no Liquid syntax errors or broken site builds:

```bash
# 1. Build check (validates site generation & template syntax)
bundle exec jekyll build

# 2. Jekyll doctor check (detects configuration warnings & URL conflicts)
bundle exec jekyll doctor

# 3. Build JS assets (if you modified any JavaScript source files under assets/js/)
npm run build:js

# 4. Check git status to ensure only intended files are staged
git status
```

---

## 📁 Repository Structure

```text
.
├── _config.yml         # Global site configuration & metadata
├── _data/              # Data files (navigation, UI text, site data)
├── _includes/          # Reusable Liquid template components
├── _layouts/           # Custom page layouts (home, categories, single post, etc.)
├── _pages/             # Standalone site pages (Home, Blogs, Categories, etc.)
├── _posts/             # Blog posts & TIL articles
├── _projects/          # Project showcase pages & metadata
├── _sass/              # SASS custom styling and overrides
└── assets/             # Images, static media, icons, and compiled JS/CSS
```