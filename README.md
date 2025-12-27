# Pranav Mehta Portfolio

A simple, fast portfolio site deployed on GitHub Pages.

## File Structure

```
/index.html    ← The template (rarely needs editing)
/data.json     ← Your content (edit this!)
/README.md     ← You're reading it
```

## How to Update Your Portfolio

### Adding a new project/article/research item

1. Open `data.json`
2. Find the relevant role (`economist`, `policymaker`, `researcher`, or `writer`)
3. Add a new item to the `items` array:

```json
{
  "title": "Your Project Title",
  "description": "One-line description of the project.",
  "date": "2025",
  "href": "https://link-to-project.com"
}
```

### Updating Education or Experience

Find the `education` or `experience` arrays and add/edit entries:

```json
{
  "title": "Job Title",
  "org": "Organization Name",
  "url": "https://org-website.com",
  "description": "Brief description",
  "years": "2024–26"
}
```

### Adding a new role category

Add a new object to the `roles` array:

```json
{
  "key": "advisor",
  "label": "Advisor",
  "article": "an",
  "sectionTitle": "Advisory Work",
  "items": [...]
}
```

Note: Roles appear in the order they're listed in the array.

### Updating basic info

Edit these fields at the top of `data.json`:
- `name` — Your name
- `email` — Contact email
- `github` — GitHub profile URL
- `linkedin` — LinkedIn profile URL
- `tagline` — The intro paragraph under "Hi, I'm Pranav!"

## Quick Edit via GitHub

You can edit `data.json` directly in GitHub's web interface:

1. Go to your repo on github.com
2. Click on `data.json`
3. Click the pencil icon (Edit)
4. Make your changes
5. Commit directly to `main`

Changes deploy automatically via GitHub Pages (usually within 1-2 minutes).

## Local Development

Just open `index.html` in a browser. Note: You'll need to serve it from a local server for the JSON fetch to work:

```bash
# Python 3
python -m http.server 8000

# Then open http://localhost:8000
```

## Troubleshooting

**Content not updating?**
- Hard refresh: `Cmd+Shift+R` (Mac) or `Ctrl+Shift+R` (Windows)
- Check that `data.json` is valid JSON (no trailing commas, proper quotes)

**Blank page?**
- Open browser console (F12) to check for errors
- Make sure `data.json` is in the same folder as `index.html`
