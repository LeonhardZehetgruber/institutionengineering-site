# Institution Engineering Site

The website source for the site [institutionengineering.com](institutionengineering.com).

## 🧪 Local Development Setup for Content Editors

This guide explains how to set up and run the Hugo site locally for editing and adding content.

### 🔧 Prerequisites

1. Git

2. Hugo
```bash
cd /tmp
wget https://github.com/gohugoio/hugo/releases/download/v0.147.8/hugo_extended_0.147.8_linux-amd64.tar.gz
tar -xvzf hugo_extended_0.147.8_linux-amd64.tar.gz
sudo mv hugo /usr/local/bin/

# Check version in a new bash session (must be v0.146.0 or newer)
hugo version
```

---

### 🗂️ Project Setup

```bash
git clone git@github.com:LeonhardZehetgruber/institutionengineering-site.git
cd institutionengineering-site
git submodule update --init --recursive
```

---

### 🚀 Running the Site Locally

Start the Hugo development server:

```bash
hugo serve
```

Now, the website is hosted on [localhost](http://localhost:1313/), hot reloading any changes made.
