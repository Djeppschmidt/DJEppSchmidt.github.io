# DJEppSchmidt.github.io

This repository hosts Dietrich Epp Schmidt's personal website using GitHub Pages.

## About

This is a GitHub Pages website that showcases research projects, publications, and professional information. The site is automatically built and deployed by GitHub using Jekyll.

## Setting Up Your Own GitHub Pages Website

### Prerequisites
- A GitHub account
- A repository named `<username>.github.io` (where `<username>` is your GitHub username)

### Initial Setup

1. **Create a GitHub Pages Repository**
   - Create a new repository on GitHub named `<yourusername>.github.io`
   - Make sure the repository is public (required for free GitHub Pages)

2. **Enable GitHub Pages**
   - Go to your repository's Settings
   - Navigate to the "Pages" section in the left sidebar
   - Under "Source", select the branch you want to use (typically `main` or `master`)
   - Click "Save"
   - Your site will be published at `https://<yourusername>.github.io/`

3. **Choose a Theme**
   - In the repository, create a `_config.yml` file
   - Add a Jekyll theme (example from this repo):
     ```yaml
     theme: jekyll-theme-modernist
     title: Your Site Title
     description: Your site description
     ```
   - Available themes can be found at: https://pages.github.com/themes/

4. **Add Content**
   - Create an `index.md` file as your homepage
   - Use Markdown to write your content
   - GitHub Pages will automatically convert it to HTML

### Customizing This Website

#### Editing the Homepage
- Edit `index.md` to change the main content
- Use Markdown syntax for formatting
- Changes are automatically published when you commit to the main branch

#### Changing Site Configuration
Edit `_config.yml` to modify:
- `theme`: The Jekyll theme to use
- `title`: The site title shown in the browser tab
- `description`: The site description used in headers

#### Adding New Pages
1. Create a new `.md` file in the repository (e.g., `about.md`, `projects.md`)
2. Add front matter at the top of the file:
   ```markdown
   ---
   title: Page Title
   ---
   
   # Your content here
   ```
3. Link to it from other pages: `[Link Text](page-name)`

### File Structure

```
.
├── _config.yml    # Jekyll configuration file
├── index.md       # Homepage content
└── README.md      # This file (documentation)
```

### Local Development (Optional)

To preview your site locally before publishing:

1. **Install Ruby and Jekyll**
   ```bash
   # Install Ruby (if not already installed)
   # Then install Jekyll and bundler
   gem install jekyll bundler
   ```

2. **Create a Gemfile** (if not present)
   ```ruby
   source 'https://rubygems.org'
   gem 'github-pages', group: :jekyll_plugins
   ```

3. **Install Dependencies**
   ```bash
   bundle install
   ```

4. **Run Jekyll Locally**
   ```bash
   bundle exec jekyll serve
   ```
   
5. **View Your Site**
   - Open your browser to `http://localhost:4000`
   - The site will auto-reload when you make changes

### Publishing Changes

1. **Make Your Changes**
   - Edit `index.md`, `_config.yml`, or other content files
   
2. **Commit and Push**
   ```bash
   git add .
   git commit -m "Description of changes"
   git push origin main
   ```

3. **Wait for Deployment**
   - GitHub Pages automatically builds and deploys your site
   - This usually takes 1-2 minutes
   - Check the "Actions" tab to see the deployment status

### Helpful Resources

- **GitHub Pages Documentation**: https://docs.github.com/en/pages
- **Jekyll Documentation**: https://jekyllrb.com/docs/
- **Markdown Guide**: https://www.markdownguide.org/
- **Jekyll Themes**: https://pages.github.com/themes/
- **GitHub Pages Themes**: https://github.com/pages-themes

### Troubleshooting

**Site not showing up?**
- Make sure your repository is named exactly `<username>.github.io`
- Check that GitHub Pages is enabled in repository Settings > Pages
- Verify the repository is public
- Wait a few minutes for the initial deployment

**Changes not appearing?**
- Check the Actions tab for build errors
- Clear your browser cache
- Wait a few minutes for GitHub to rebuild the site

**Theme not working?**
- Verify the theme name is correct in `_config.yml`
- Make sure you're using a supported GitHub Pages theme
- Check for YAML syntax errors in `_config.yml`

## License

This website and its content are personal materials. Please contact the repository owner for permissions regarding use or distribution.
