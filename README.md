# Personal Academic Website

This is a simple personal website built with Jekyll for GitHub Pages.

## Setup Instructions

### 1. Create GitHub Repository

1. Go to GitHub and create a new repository named `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
2. Initialize it as a public repository

### 2. Upload These Files

Clone your new repository and copy all these files into it:

```bash
git clone https://github.com/yourusername/yourusername.github.io.git
cd yourusername.github.io
# Copy all files from this folder
git add .
git commit -m "Initial commit"
git push origin main
```

### 3. Enable GitHub Pages

1. Go to your repository settings on GitHub
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select "main" branch
4. Click "Save"

Your site will be live at `https://yourusername.github.io` in a few minutes!

## Editing Your Website

### Update Your Information

Edit `_config.yml` to change:
- `title`: Your name
- `url`: Your actual GitHub Pages URL

### Update Your About Section and Publications

Edit `index.md` to:
- Replace the placeholder text in the "Welcome" section with your actual bio
- Add/remove publications in the Publications section
- Update contact information at the bottom

### Making Updates

Whenever you want to update your site:

1. Edit the `index.md` file
2. Commit your changes:
   ```bash
   git add index.md
   git commit -m "Updated publications"
   git push origin main
   ```
3. Wait 1-2 minutes for GitHub Pages to rebuild your site

## Customization

This site uses the default "minima" theme. You can:
- Change the theme by editing `_config.yml`
- Add custom CSS by creating `assets/css/style.scss`
- Add more pages by creating new `.md` files

## Testing Locally (Optional)

To preview your site before pushing:

```bash
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000` in your browser.
