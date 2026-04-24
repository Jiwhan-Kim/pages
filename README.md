# Jiwhan Kim Academic Homepage

This is a simple static personal academic homepage for GitHub Pages. It uses only plain HTML and CSS, with no framework, build step, npm package, or bundler.

## Files

- `index.html`: Main homepage content
- `style.css`: Visual design and responsive layout
- `assets/`: Folder for profile photos and other images

## Recommended Repository Name

For a personal GitHub Pages site, use:

```text
username.github.io
```

Replace `username` with your GitHub username. For example, if your GitHub username is `jiwhankim`, the repository should be named:

```text
jiwhankim.github.io
```

## How to Upload to GitHub

1. Create a new GitHub repository named `username.github.io`.
2. Upload these files to the root of the repository:
   - `index.html`
   - `style.css`
   - `README.md`
   - `assets/`
3. Commit the files to the `main` branch.

You can also upload with Git:

```bash
git init
git add .
git commit -m "Create academic homepage"
git branch -M main
git remote add origin https://github.com/username/username.github.io.git
git push -u origin main
```

## How to Enable GitHub Pages

For a repository named `username.github.io`, GitHub usually publishes it automatically.

If it does not appear:

1. Open the repository on GitHub.
2. Go to **Settings**.
3. Open **Pages** in the left sidebar.
4. Under **Build and deployment**, choose:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/** root
5. Save the settings.

Your site should appear at:

```text
https://username.github.io/
```

## How to Edit Content

Open `index.html` and edit the text inside each section:

- Home / About
- Education
- Experience
- Publications
- Projects
- Skills
- Honors / Awards
- Contact

The file includes comments showing where to add new entries, such as:

```html
<!-- Add new publication here -->
<!-- Add new project here -->
```

To add a new publication, copy an existing publication `<article class="entry">...</article>` block and paste it above the `<!-- Add new publication here -->` comment.

To add a new project, copy an existing project `<article class="card">...</article>` block and paste it above the `<!-- Add new project here -->` comment.

## How to Add a Profile Image

1. Add your image to the `assets/` folder.
2. Recommended filename:

```text
assets/profile.jpg
```

3. In `index.html`, find the profile placeholder near the top of the Home section.
4. Replace the placeholder block with:

```html
<img class="profile-photo" src="assets/profile.jpg" alt="Jiwhan Kim">
```

Square images work best. The CSS will crop the image into a circle.

## Customizing the Design

Edit `style.css` to adjust colors and spacing. The easiest values to change are at the top of the file:

```css
:root {
  --bg: #f7f9fb;
  --surface: #ffffff;
  --accent: #1f7a8c;
  --text: #1d2730;
}
```

Changing `--accent` updates the main highlight color across the site.
