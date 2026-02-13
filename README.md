# Edo Cohen-Karlik - Jekyll Portfolio

A modern, editorial-style academic portfolio built with Jekyll.

## 📁 File Structure

```
├── _config.yml                 # Jekyll configuration
├── _layouts/
│   └── default.html           # Main layout template
├── _data/
│   ├── publications.yml       # Publications data
│   └── teaching.yml           # Teaching experience data
├── assets/
│   ├── css/
│   │   └── style.css         # Main stylesheet
│   └── js/
│       └── script.js         # JavaScript for animations
└── index.md                   # Homepage content
```

## 🚀 Setup Instructions

### Option 1: GitHub Pages (Recommended)

1. **Upload files to your repository** with this structure:
   - Copy all files to the root of your `edocoh87.github.io` repository
   - Maintain the folder structure shown above

2. **Enable GitHub Pages**:
   - Go to Settings → Pages
   - Source: Deploy from branch
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`

3. **Wait for deployment**: GitHub will automatically build and deploy your site

### Option 2: Local Development

1. **Install Jekyll**:
   ```bash
   gem install bundler jekyll
   ```

2. **Create a Gemfile** in the root directory:
   ```ruby
   source "https://rubygems.org"
   gem "jekyll", "~> 4.3"
   gem "webrick", "~> 1.8"
   ```

3. **Install dependencies**:
   ```bash
   bundle install
   ```

4. **Run locally**:
   ```bash
   bundle exec jekyll serve
   ```

5. **View in browser**: Visit `http://localhost:4000`

## ✏️ Editing Content

### Update Publications

Edit `_data/publications.yml`:

```yaml
- year: 2026
  title: "Your Paper Title"
  authors: "<strong>E. Cohen-Karlik</strong>, Other Authors"
  venue: "Conference Name"
  url: "https://link-to-paper.pdf"
```

### Update Teaching

Edit `_data/teaching.yml`:

```yaml
- name: "Course Name"
  years: "2020–2023"
```

### Update Bio

Edit the hero section in `index.md`

## 🎨 Customization

### Colors

Edit CSS variables in `assets/css/style.css`:

```css
:root {
    --ink: #0a0a0f;           /* Text color */
    --paper: #faf8f3;         /* Background */
    --accent: #d63447;        /* Accent color */
    --accent-soft: #ff6b7a;   /* Soft accent */
    --gray: #6b7280;          /* Secondary text */
}
```

### Fonts

The design uses:
- **Fraunces** (serif) for headlines
- **Instrument Sans** for body text

Change fonts in `_layouts/default.html` by modifying the Google Fonts link.

## 📱 Features

- ✨ Smooth scroll animations
- 📱 Fully responsive design
- 🎨 Editorial typography
- 🔗 Dynamic content from YAML data files
- ⚡ Fast loading with minimal dependencies

## 🛠️ Troubleshooting

**Site not updating?**
- Clear browser cache
- Check GitHub Actions tab for build errors
- Wait 2-3 minutes after pushing changes

**Styles not loading?**
- Ensure folder structure matches exactly
- Check that CSS file is in `assets/css/style.css`

**Liquid errors?**
- Verify YAML formatting in data files
- Ensure proper indentation (use spaces, not tabs)

## 📄 License

Feel free to use and modify for your own academic portfolio!
