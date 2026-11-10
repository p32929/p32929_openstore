# OpenStore listing template

This is the **`template`** branch of [p32929/p32929_openstore](https://github.com/p32929/p32929_openstore): the clean starter for an [OpenStore](https://github.com/p32929/openstore_maintainers) listing. (The `main` branch is p32929's own listing, a real example.)

**Get it** into a new **public** repo of yours, either way:

- **Download** [the template as a ZIP](https://github.com/p32929/p32929_openstore/archive/refs/heads/template.zip), unzip it, and push the files to your new repo.
- **Or clone just this branch:**
  ```bash
  git clone -b template --single-branch https://github.com/p32929/p32929_openstore.git my-openstore
  cd my-openstore && git remote set-url origin https://github.com/your-github-name/your-repo.git
  git branch -m template main && git push -u origin main
  ```

```
your-github-name/your-repo
├── profile.yaml        ← optional: avatar, website, location
├── validate.mjs        ← checks everything: node validate.mjs
├── .github/workflows/  ← runs that same check on GitHub on every push
├── images/             ← optional: icons and screenshots, used by path (images/app1-icon.png)
└── apps/
    ├── app1.md         ← one file per app; becomes /app/your-github-name/app1
    └── app2.md
```

## Steps

1. **Edit the files.** Replace `apps/app1.md` and `apps/app2.md` with your own apps (one `.md` file per app, any number), and edit or delete `profile.yaml`.
2. **Check them:** `node validate.mjs` (needs only [Node.js](https://nodejs.org)) lists every problem as `file:line`; fix them until it says *All good*, then push. GitHub runs the same check on every push (your repo's **Actions** tab) and marks problems on the exact lines.
3. **Join, once:** open a pull request on [p32929/openstore_maintainers](https://github.com/p32929/openstore_maintainers) adding `- your-github-name/your-repo` to `maintainers.yaml`. It's checked automatically: your repo must pass, and the pull request must come from your own account.

```
$ node validate.mjs

  ✓ profile.yaml
  ✗ apps/app1.md
      apps/app1.md:4  unknown field "tag" (check the spelling)
      apps/app1.md:15  platforms.Web.0.url: Invalid URL
  ✓ apps/app2.md  → /app/your-github-name/app2

2 problems. Fix them and run again.
```

After that, just push here: add a file to `apps/` for a new app, add a release at the top of a platform's list, delete a file to remove an app. The store picks up changes on its next build and downloads only the files that changed.

## What goes in the files

**`apps/<name>.md`**: a YAML header between `---` lines, then the description. [`apps/app1.md`](apps/app1.md) and [`apps/app2.md`](apps/app2.md) use every field.

| Field | | What |
|---|---|---|
| `title` | required | The app's name |
| `icon` | required | An image: a path in your repo (`images/icon.png`, from the repo root) or an `https://` link |
| `screenshots` | required | One or more images, same as `icon` |
| `category` | required | Exactly one, from the list below |
| `platforms` | required | One or more, from the list below. Each is either **a link** (`Web: https://…`, where to get it) or **a list of releases, newest first**, or nothing (*listed, no release yet*) |
| a release | `url` required; `version`, `date`, `changelog` optional | `url` is where to get it; `date` like `2026-10-01` (dates must go backwards down the list) |
| `summary` | optional | One line (160 characters) for cards; default: the description's first line |
| `tags` | optional | Up to 10 free keywords, for search |
| `website`, `source`, `license` | optional | Shown on the app page; `source` as a *Source code* link |
| `video` | optional | One link, shown as a *Watch video* button |
| description | required | Markdown below the header (see the Markdown rules); line breaks are kept as written |

**`profile.yaml`** (optional, every field too) turns your `/dev` page into a small portfolio:

| Field | What |
|---|---|
| `name`, `bio` | Display name (default: your GitHub username) and a one-line tagline (160 characters) |
| `avatar` | An image, like `icon` (default: your GitHub avatar) |
| `location`, `website`, `email` | Shown in your header; `email` as an Email button |
| `skills`, `skillsOrder` | Up to 30, shown as tags; `skillsOrder: alphabetical` sorts them A–Z (default `as-written`) |
| `links` | Up to 10 `label: https://…` pairs (GitHub, LinkedIn…) |
| `about` | Markdown, same rules as app descriptions; line breaks are kept as written |

## Rules

- **Your username** on the store is your GitHub name; one repo per account.
- **An app's link** is its file name: lowercase letters, digits and `-` (`my-app.md`). Renaming the file changes the link.
- **Platforms and categories** must be from the lists below (exact spelling and capitals). Each file must be under 1 MB.
- **Image paths** start at the repo root and must exist in the repo; `validate.mjs` checks them.
- **Description Markdown** (below the `---` header) is limited to safe formatting:

  | Allowed | Not allowed |
  |---|---|
  | paragraphs, `##` to `####` headings, **bold**, *italic*, ~~strike~~, lists, `> quotes`, `---` dividers, tables, `inline code` and code blocks | any raw HTML (`<script>`, `<img>`, `<iframe>`, `<details>`, comments…), `#` headings (the page shows your title), `#####` and deeper |
  | links to `https://…` and `mailto:…` | other links (`http://`, `javascript:`, `data:`…), images (use `screenshots`) |

  `validate.mjs` reports anything not allowed with its line.
- **If the rules change**, take the latest `validate.mjs` from this branch.

## Allowed values

<!-- allowed-values: generated by the store's pnpm build:validator -->

**Platforms:** `iOS`, `Android`, `Windows`, `MacOS`, `Web`, `CLI`, `Library`, `Extension`, `Automation`

<details>
<summary><b>Categories</b> (61)</summary>

- `Art & Design`
- `Auto & Vehicles`
- `Beauty`
- `Books & Reference`
- `Business`
- `Comics`
- `Communication`
- `Dating`
- `Education`
- `Entertainment`
- `Events`
- `Finance`
- `Food & Drink`
- `Health & Fitness`
- `House & Home`
- `Libraries & Demo`
- `Lifestyle`
- `Maps & Navigation`
- `Medical`
- `Music & Audio`
- `News & Magazines`
- `Parenting`
- `Personalization`
- `Photography`
- `Productivity`
- `Shopping`
- `Social`
- `Sports`
- `Tools`
- `Travel & Local`
- `Video Players & Editors`
- `Wear OS by Google`
- `Weather`
- `Books`
- `Developer Tools`
- `Graphics & Design`
- `Social Networking`
- `Utilities`
- `Family & Kids`
- `Government`
- `Multimedia Design`
- `Personal Finance`
- `Security`
- `Software Development`
- `Action Game`
- `Adventure Game`
- `Arcade Game`
- `Board Game`
- `Card Game`
- `Casino Game`
- `Casual Game`
- `Educational Game`
- `Music Game`
- `Puzzle Game`
- `Racing Game`
- `Role Playing Game`
- `Simulation Game`
- `Sports Game`
- `Strategy Game`
- `Trivia Game`
- `Word Game`

</details>

<!-- /allowed-values -->

A real example: the [`main` branch](https://github.com/p32929/p32929_openstore) of this repo.
