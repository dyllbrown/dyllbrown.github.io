# Design Engineer Portfolio — Site

A plain HTML/CSS/JS static website. No build step, no dependencies, no install required.

## How to view it

Just double-click `index.html` to open it in your browser. All links are relative, so everything works
locally without a web server.

## How to edit content

- **Case study text**: edit directly in each `case-studies/*.html` file. The full drafted copy also lives in
  `../Portfolio_Case_Study_Drafts.md` (one level up) if you want to compare/revise there first.
- **Name, email, LinkedIn, headshot, resume**: already filled in with your real info (`assets/images/headshot.jpg`,
  `assets/resume/resume.pdf`). Re-run the resume-to-PDF conversion and swap the headshot file if either changes.
- **Styling**: all shared styles are in `css/styles.css`. Colors and sizing are defined as CSS variables at the
  top of that file (`:root { ... }`) if you want to re-theme the site.

## Images

All 7 case studies now have real photos/renders, organized in subfolders under `assets/images/` (one per
case study). Two optional slots still use the shared placeholder graphic (`assets/images/placeholder.svg`):
the D14 v1 design comparison shot, and the Cell Wash individual-lane servicing detail shot. See
`VISUAL_EXPORT_CHECKLIST.md` if you want to track down those last two.

## How to publish it (when you're ready)

This site currently lives inside your Tesla OneDrive-synced CAD folder. **Before doing anything below, get
sign-off from your manager / Tesla's IP-disclosure process** — this content was created on company time and
describes real Tesla production equipment, even though it's been sanitized.

Once cleared:
1. Move the `Portfolio/` folder out of OneDrive to a personal location (e.g., a folder in your personal
   Documents, or a personal GitHub repo).
2. The simplest free hosting options for a static site like this are **GitHub Pages** or **Netlify** (drag-and-drop
   deploy — no command line needed for Netlify).
3. Do one more full read-through of every page for anything you want to generalize further before it goes live.

## Folder structure

```
Portfolio/
  index.html                 Home page (hero, skills, case study grid)
  about.html                 About / Skills / Resume & Contact
  case-studies/               One page per case study
  assets/
    images/                  Per-case-study image subfolders, plus headshot.jpg and placeholder.svg
    resume/resume.pdf        Your resume, auto-converted from the .docx
  css/styles.css             All shared styles
  js/main.js                 Mobile nav toggle (only script on the site)
```
