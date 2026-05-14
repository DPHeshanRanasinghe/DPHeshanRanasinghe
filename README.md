# 🚀 README Setup Guide

## Step 1 — Create your profile repository

GitHub treats a repo whose name **matches your username exactly** as a special "profile repo." Its `README.md` shows up on your GitHub profile page.

1. Go to: <https://github.com/new>
2. Repository name: **`DPHeshanRanasinghe`** (must match your username exactly — case-sensitive)
3. Set it to **Public**
4. Check ✅ **"Add a README file"**
5. Click **Create repository**

## Step 2 — Replace the README

1. Open the new repo on GitHub
2. Click the pencil icon ✏️ to edit `README.md`
3. Delete everything inside, paste the contents of the `README.md` I generated
4. Commit to `main`

## Step 3 — Enable the contribution snake (animated, updates every 12h)

The snake animation in your README points to an SVG that doesn't exist yet — a GitHub Action will generate and refresh it for you automatically.

1. Inside the same repo (`DPHeshanRanasinghe/DPHeshanRanasinghe`), create a folder: `.github/workflows/`
2. Inside that folder, add the `snake.yml` file I generated
3. Commit to `main`
4. Go to the repo's **Actions** tab → enable workflows if prompted
5. Click **"Generate Contribution Snake"** in the left sidebar → click **"Run workflow"** to trigger the first run manually (otherwise it waits up to 12 hours)
6. After it finishes (~30 seconds), a new branch called `output` will appear with the SVG files. The README will start displaying them.

## Step 4 — Verify everything renders

Visit <https://github.com/DPHeshanRanasinghe> and check:

- ✅ Animated banner waves at the top
- ✅ Typing animation cycles through your taglines
- ✅ Profile views counter shows (it starts incrementing immediately)
- ✅ GitHub stats cards render with tokyonight theme
- ✅ Streak stats card shows your contribution streak
- ✅ Top languages card shows your language breakdown
- ✅ Activity graph renders below
- ✅ Trophy row shows below activity
- ✅ Snake animation eats contribution squares (after Step 3 completes)

If anything looks broken, it's almost always one of:

- **Stats cards show "Could not fetch user"** → wait 1–2 minutes, the Vercel servers cache. Refresh.
- **Snake says "image not found"** → the Action hasn't run yet. Trigger it manually in the Actions tab.
- **Profile views stuck at 0** → komarev.com counts unique IPs, so opening in incognito/mobile will increment it.

## Optional — Pin your best repos

Underneath the README, GitHub shows up to 6 pinned repositories. Go to your profile → **Customize your pins** → pick your strongest work (CranioVision, FPGA-Detection, etc).

## Theme customization

If you want a different color scheme, search-and-replace `tokyonight` in `README.md` with one of:

`dark` · `radical` · `merko` · `gruvbox` · `tokyonight` · `onedark` · `cobalt` · `synthwave` · `highcontrast` · `dracula`

The accent color `58a6ff` (GitHub blue) appears throughout — replace it globally if you want a different highlight color (e.g. `bb9af7` for purple, `7ee787` for green, `f78166` for orange).
