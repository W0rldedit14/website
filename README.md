# DevSecOps Portfolio - Yuveer Chetraj

[![Hugo](https://img.shields.io/badge/Hugo-0.140+-blue.svg)](https://gohugo.io)
[![Theme](https://img.shields.io/badge/Theme-Hugo%20Noir-black.svg)](https://github.com/prxshetty/hugo-noir)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

🔗 **Live Site**: [https://yuveerchetraj.dev](https://w0rldedit14.github.io)

A professional portfolio website showcasing my experience in application security, cloud security, and infrastructure automation.

## 🏗️ Built With

This website is built using [Hugo](https://gohugo.io/), a fast and flexible static site generator.

### Theme

The site uses the [Hugo Noir](https://github.com/prxshetty/hugo-noir) theme created by [@prxshetty](https://github.com/prxshetty) - a clean, minimalistic theme perfect for developer portfolios.

**Big thanks to [@prxshetty](https://github.com/prxshetty) for creating this excellent theme!** 🙏

I've made several customizations to the original theme:

---

## 🚀 Quick Start

Want to create your own portfolio using this setup? Follow these steps:

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.92.0 or later)
- [Git](https://git-scm.com/downloads)
- A [GitHub](https://github.com) account

### Installation

1. **Install Hugo Extended**

   ```bash
   # macOS
   brew install hugo
   
   # Windows (using Chocolatey)
   choco install hugo-extended
   
   # Linux
   snap install hugo --channel=extended
   ```

2. **Clone this repository**

   ```bash
   git clone https://github.com/W0rldedit14/website
   cd website
   ```

3. **Initialize the theme submodule**

   ```bash
   git submodule update --init --recursive
   ```

4. **Run the development server**

   ```bash
   hugo server -D
   ```

5. **Open your browser**

   Navigate to `http://localhost:1313` to see your site!

---

## 📁 Project Structure

```
.
├── content/              # Markdown content files
│   ├── _index.md        # Homepage content
│   ├── about.md         # About page
│   ├── experience.md    # Experience page
│   ├── contact.md       # Contact page
│   ├── blog/            # Blog posts
│   └── projects/        # Project pages
├── data/                # Data files (TOML format)
│   └── en/
│       ├── author.toml      # Author information
│       ├── experience.toml  # Work experience with sections
│       ├── projects.toml    # Project highlights
│       ├── tech.toml        # Tech stack carousel
│       └── blogs.toml       # Blog links
├── layouts/             # Custom layout overrides
│   ├── _default/
│   │   └── experience.html  # Custom experience layout
│   └── partials/
├── static/              # Static assets
│   ├── images/          # Images
│   └── favicon_io/      # Favicon files
├── themes/              # Hugo themes
│   └── hugo-noir/       # Theme submodule
├── .github/
│   └── workflows/
│       └── hugo.yaml    # GitHub Actions deployment
├── hugo.toml            # Site configuration
└── README.md            # This file
```

---

## ⚙️ Configuration

### Site Settings (`hugo.toml`)

Edit `hugo.toml` to customize your site:

```toml
baseURL = "https://yourusername.github.io/"
languageCode = "en-us"
title = "Your Name - DevSecOps Portfolio"
theme = "hugo-noir"

[params]
  name = "Your Name"
  location = "Your City, Country"
  description = "Your professional tagline"
  profile_image = "/images/profile.jpg"
  
  # Social links
  github = "https://github.com/yourusername"
  linkedin = "https://linkedin.com/in/yourusername"
  email = "your.email@example.com"
```

### Content Configuration

#### 1. Author Information (`data/en/author.toml`)

```toml
[author]
  name = "Your Name"
  location = "Your City"
  description = "Your bio"
  profile_image = "/images/profile.jpg"
  github = "https://github.com/yourusername"
  linkedin = "https://linkedin.com/in/yourusername"
  email = "your.email@example.com"
```

#### 2. Tech Stack (`data/en/tech.toml`)

```toml
row1 = [
  { icon = "devicon-kubernetes-plain", name = "Kubernetes" },
  { icon = "devicon-docker-plain", name = "Docker" },
  # Add more technologies...
]

row2 = [
  { icon = "devicon-python-plain", name = "Python" },
  # Add more technologies...
]
```

Icons use [Devicon](https://devicon.dev/) - browse available icons there.

#### 3. Experience (`data/en/experience.toml`)

```toml
[[experience]]
  role = "Your Role"
  company = "Company Name"
  company_link = "https://company.com"
  period = "Jan 2020 - Present"
  country = "Country"
  
  # Technical Skills
  [[experience.technical_skills]]
    category = "Skill Category"
    skills = "Skill 1 • Skill 2 • Skill 3"
  
  # Responsibility Sections
  [[experience.sections]]
    icon = "🔐"
    title = "Section Title"
    items = [
      "Responsibility or achievement 1",
      "Responsibility or achievement 2"
    ]
```

#### 4. Projects (`data/en/projects.toml`)

```toml
[[projects]]
  title = "Project Name"
  description = "Project description"
  image = "/images/projects/project.jpg"
  tags = ["Tag1", "Tag2"]
  link = "/projects/project-slug"
  highlights = [
    "Key achievement 1",
    "Key achievement 2"
  ]
```

---

## 🎨 Customization Guide

### Adding Custom Layouts

Create files in `layouts/` to override theme layouts:

```bash
# Custom experience page
layouts/_default/experience.html

# Custom partials
layouts/partials/header.html
```

### Styling

The theme uses Tailwind CSS. To modify styles, edit:
- `themes/hugo-noir/assets/css/main.css` (in your fork)
- Or add custom CSS in `assets/css/custom.css`

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

The Hugo Noir theme is also licensed under the MIT License.

---

## 🙏 Acknowledgments

- **[Hugo](https://gohugo.io)** - The amazing static site generator
- **[@prxshetty](https://github.com/prxshetty)** - For creating the beautiful Hugo Noir theme
- **[Devicon](https://devicon.dev/)** - For the technology icons
- **[GitHub Pages](https://pages.github.com/)** - For hosting
- **[Porkbun](https://porkbun.com/)** - For domain management
