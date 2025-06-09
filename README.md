# Institution Engineering Site

The website source for the site [institutionengineering.com](institutionengineering.com).

## 🧪 Local Development Setup for Content Editors

This guide explains how to set up and run the Hugo site locally for editing and adding content.

### 🔧 Prerequisites

1. **Install Git**
   Download and install from: [https://git-scm.com/downloads](https://git-scm.com/downloads)

2. **Install Hugo (Extended Version)**
   Follow installation instructions: [https://gohugo.io/getting-started/install/](https://gohugo.io/getting-started/install/)

   > ✅ Make sure you install **Hugo Extended**, version **v0.146.0 or newer**

   Check installation:

   ```bash
   hugo version
   ```

   Output should include `extended` and a version `>= v0.146.0`.

---

### 🗂️ Project Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   cd YOUR_REPO_NAME
   ```

2. **Initialize theme submodules (if required)**

   ```bash
   git submodule update --init --recursive
   ```

---

### 🚀 Running the Site Locally

Start the Hugo development server:

```bash
hugo serve
```

Then open your browser to:
👉 `http://localhost:1313`

Changes are live-reloaded as you edit files.

---

### ✏️ Adding or Editing Content

#### ➕ Create a new article

```bash
hugo new posts/my-article-title.md
```

You can also use other sections:

```bash
hugo new policy/universal-basic-income.md
```

#### 📝 Edit the Markdown file

* Open the newly created `.md` file in a text editor (e.g., VS Code).
* Example front matter:

  ```yaml
  ---
  title: "Universal Basic Income"
  date: 2025-06-09
  tags: ["policy", "economy"]
  categories: ["politics"]
  draft: true
  ---
  ```
* Set `draft: false` to publish the article.
* Use Markdown to add headings, links, images, etc.

---

### 📂 Directory Structure Overview

```
content/
├── _index.md           # Home page content (optional)
├── posts/              # Blog posts
├── policy/             # Policy articles
├── about.md            # About page
```

---

### ✅ Commit and Push Changes (Optional)

If you’re working with Git:

```bash
git add .
git commit -m "Added new article on UBI"
git push origin main
```

---

### ❓ Troubleshooting

* Run `hugo version` — must be **extended** and version `>= v0.146.0`
* Ensure submodules are initialized with:

  ```bash
  git submodule update --init --recursive
  ```
* Check for typos in `config.toml`

---
