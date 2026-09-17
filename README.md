# sethdaviespatrick.au

Personal IT/cybersecurity portfolio site. Plain HTML/CSS, no build step,
hosted on GitHub Pages.

## Structure

```
/index.html              Home
/about.html
/skills.html
/contact.html
/resume.pdf               Downloadable resume
/projects/
  index.html               Projects overview
  homelab.html              Flagship project — Cybersecurity Home Lab
  savestate.html             SaveState (WIP)
  uni-coursework.html        Uni coursework write-ups
/writing/
  index.html                Writing index (empty for now)
/assets/
  css/style.css              Stylesheet
  img/                        (empty — add photos/diagrams here)
```

## Getting it live

1. **Create a GitHub repo** named `sethdaviespatrick.github.io`
   (this exact naming is required for GitHub Pages to serve it at the
   root of that github.io URL).
2. Push everything in this folder to the `main` branch of that repo.
3. In the repo's **Settings → Pages**, set the source to `main` branch,
   `/ (root)`. Your site will be live at
   `https://sethdaviespatrick.github.io` within a few minutes.
4. **Test everything** on that URL — all links, mobile view, the resume
   download — before touching the domain.
5. **Once the domain is registered** (sethdaviespatrick.au via
   VentraIP):
   - Add a file named `CNAME` (no extension) to the root of this repo
     containing exactly: `sethdaviespatrick.au`
   - In VentraIP's DNS settings for the domain, add the DNS records
     GitHub specifies for custom domains (an ALIAS/ANAME or A records
     pointing at GitHub's IPs, plus a CNAME for `www` if wanted) — see
     GitHub's "Managing a custom domain for your GitHub Pages site"
     docs for the exact current records.
   - Back in repo Settings → Pages, enter the custom domain and enable
     "Enforce HTTPS" once it's available (can take a few hours after
     DNS propagates).

## To-do before this is "done"

- [ ] Replace `resume.pdf` with the latest version whenever the resume changes
- [ ] Add real content to `projects/homelab.html` once the December
      rebuild is finished (photos, diagrams, before/after)
- [ ] Add the video series once filmed and uploaded (unlisted YouTube)
- [ ] Add uni coursework write-ups once assessments are marked
- [ ] Write first post in `/writing/` (LinkedIn healthcare SME post,
      rewritten as original content)
- [ ] Update `skills.html` certifications section once AZ-900 is done
- [ ] Swap placeholder social/contact links for final versions if any change

## Notes

- Font: IBM Plex Sans / IBM Plex Mono, loaded from Google Fonts.
- No JS framework — plain HTML/CSS only, by design, to keep this fast
  and simple to maintain.
- Color palette and "rack unit" section styling are intentional design
  choices tied to the actual 6U rack build — see `assets/css/style.css`
  for the token definitions if you want to adjust colors later.
