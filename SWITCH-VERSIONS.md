# How to Switch Between README Versions

Your folder contains two README versions. Only one can be active at a time —
GitHub always reads the file named exactly `README.md`.

---

## Version A — Activity Graph (currently active)
File: `README.md`
- No workflow setup required
- Contribution section renders as a clean area chart automatically
- Recommended if you want a simpler, lower-maintenance setup

## Version B — Snake Animation
File: `README-snake.md`
- Requires the snake workflow to run first (see below)
- Contribution section shows an animated snake eating your commits

---

## To switch to the Snake version

1. Rename `README.md` → `README-activity.md`
2. Rename `README-snake.md` → `README.md`
3. Go to your repo's Actions tab → Run the "Generate Snake" workflow manually
4. Commit and push

## To switch back to the Activity Graph version

1. Rename `README.md` → `README-snake.md`
2. Rename `README-activity.md` → `README.md`
3. Commit and push (no workflow needed)

---

## One-time setup for Snake (do this after pushing)

1. Go to repo Settings → Actions → General
2. Set Workflow permissions to "Read and write permissions"
3. Go to Actions tab → Generate Snake → Run workflow
4. Wait ~30 seconds — the output branch will be created automatically
