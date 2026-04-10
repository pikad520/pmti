# PMTI

PMTI is a fan-made, non-commercial monster-themed personality test built as a single static page.

It is designed as a lightweight web experience: answer a set of questions, get a themed personality result, view your top matches, and export a share image.

## Status

This project is intentionally small and mostly complete.

- Static HTML only
- No backend
- No account system
- No analytics
- No planned long-term maintenance

## Features

- 15 personality dimensions
- 30 quiz questions
- 16 themed result types
- Result card with lore-style descriptions
- Top 3 similar types
- Extra worldbuilding results
- PNG share image export

## Run Locally

You can open the project directly in a browser:

1. Open `index.html`

If your browser handles downloads more reliably over HTTP than `file://`, you can also serve it locally with any static server.

Example:

```bash
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Deploy

### Cloudflare Pages

This project works well on Cloudflare Pages because it is a plain static site with no build step.

Suggested settings:

- Framework preset: `None`
- Build command: leave empty
- Build output directory: `/`

Typical deployment flow:

1. Push this folder to a Git repository
2. Open Cloudflare Pages
3. Create a new project from that repository
4. Use the static-site settings above
5. Deploy from the repository root

If the UI insists on a build command, you can use:

```bash
echo "static site"
```

### Other Static Hosts

This project can also be deployed to other static hosting providers such as GitHub Pages, GitLab Pages, Netlify, or Vercel.

Recommended risk-reduction choices:

- Keep the site non-commercial
- Keep the site static
- Avoid adding official images, logos, or screenshots
- Prefer low-discovery deployment and avoid active promotion as an "official-looking" product
- Keep the included `robots.txt` and the page-level `noindex` meta tag if you want lower search exposure

## Fan Project Notice

This is an unofficial, fan-made project for entertainment only.

It is not affiliated with, endorsed by, sponsored by, or approved by Nintendo, GAME FREAK, Creatures Inc., or The Pokemon Company.

This project is intended to be non-commercial.

## Content and IP Notes

- Do not present this project as official
- Do not claim endorsement or authorization
- Do not use official logos as branding
- Do not sell access, memberships, ads, or sponsored placements around it

## About Character Images

Using recognizable franchise-related images increases legal and platform risk.

Safer options:

- Use fully original abstract visuals
- Use silhouettes or icon-like designs you created yourself
- Use commissioned original fan-style illustrations that do not copy official artwork files

Higher-risk options:

- Official artwork
- Game screenshots
- Official card art
- Official promotional images
- Official logos or branded UI assets

If you choose to include character images, the lowest-risk version is usually original fan-made artwork created specifically for this project, while still keeping the project clearly unofficial and non-commercial.

## Tech

- HTML
- CSS
- Vanilla JavaScript

## License

No license is granted for any third-party franchise-related intellectual property.

Code and original project-specific text in this repository are shared only as part of this non-commercial fan project unless a separate license is later added.
