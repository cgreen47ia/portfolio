# Vibe Coding Portfolio

A static Bold Canvas portfolio site. Each project lives in its own folder with a case study page and assets.

## Adding a new project page

### 1. Create the project folder

```
{slug}/
  assets/          # images for this project
  content.md       # project copy (source of truth)
  index.html       # generated case study page
```

Use a **slug** from the title: lowercase, spaces → hyphens (e.g. `Monthly Budget Web App` → `budget`).

### 2. Add assets

Place images in `{slug}/assets/`:

| File pattern | Used for |
|---|---|
| `cover_*.png` | Home page project card |
| `mockup_hero_*.png` | Hero on project page |
| `*_visual_*.png` | Designs section screenshots |
| `user_flow_*.png` | Process section (after paragraph 1) |
| `site_map_*`, `descriptives_*` | Process section (after paragraph 2) |
| `*design_system*`, `moodboard.png` | Process section (design system step) |

### 3. Write `content.md`

Copy the structure from `budget/content.md` or `sweat-equity/content.md`. Required sections:

- **Frontmatter** — title, category, badge, description, year, role, tools, `live_url`, `github_url`
- **Overview** → **Problem** → **Process** → **Solution** → **Designs** → **Reflections**

Process notes:
- First line under `## Process` is the pipeline (e.g. `User Tasks > User Flows > Site Map > …`), split on `>`.
- Each `###` under `## Designs` becomes one screen/feature with a screenshot.

### 4. Generate the page with Cursor

Open this folder in **Cursor**, start a new **Agent** chat, and prompt:

```
Generate a portfolio project page for [Project Title]
```

Or, if the folder already exists:

```
/portfolio-project-page [slug]
```

The agent will read `content.md`, build `{slug}/index.html` matching the budget layout, and add a card to the home page `index.html`.

If `content.md` is empty, the agent will create a template and ask you to fill it in first.

### 5. Review and tweak

Canonical references:

- `budget/index.html` + `budget/content.md` — layout and content schema
- `sweat-equity/index.html` + `sweat-equity/content.md` — mobile screenshots, multi-image designs

After generation, open `{slug}/index.html` in a browser and check images, links, and mobile layout.

---

## Cursor skill: `portfolio-project-page`

This project uses a custom Cursor skill to generate consistent case study pages.

### Where it lives

| Location | Path |
|---|---|
| **Your machine (primary)** | `C:\Users\cgreen\.cursor\skills\portfolio-project-page\` |
| **On any OS** | `~/.cursor/skills/portfolio-project-page/` |

Skill files:

- `SKILL.md` — workflow the agent follows
- `content-template.md` — starter `content.md` schema
- `layout-reference.md` — section order and image mapping
- `components.md` — HTML/CSS patterns
- `project-page-template.html` — page skeleton

### If you change accounts or machines

1. Copy the entire `portfolio-project-page` folder to the new machine’s `~/.cursor/skills/` directory.
2. Or re-create it: in Cursor, ask the agent to *“create a skill called portfolio-project-page”* and point it at `budget/content.md` and `budget/index.html` as the canonical examples.

Skills are **not** stored in this git repo by default — back up `~/.cursor/skills/portfolio-project-page/` if you want them in version control.

### What you need to run it

- **Cursor** (desktop app) with Agent mode
- This project folder opened as the workspace
- **No install step** — no `npm install` or CLI required to generate pages
- A filled-in `{slug}/content.md` and assets in `{slug}/assets/`

The site is plain HTML/CSS. To preview locally, open `index.html` in a browser, or use any static file server (e.g. VS Code / Cursor Live Server extension).

### Example prompts

```
Generate a portfolio project page for Nutrition Tracker
```

```
Update the nutrition project page from content.md
```

```
Add a project card on the home page for budget
```

---

## Project structure (quick reference)

```
Portfolio-project/
  index.html          # home page + projects grid
  DESIGN.md           # Bold Canvas design system
  budget/             # example project (canonical layout)
  sweat-equity/       # example project (mobile + extended process)
  {your-project}/
    content.md
    index.html
    assets/
```
