# Shahnoor Studio — Vercel Deploy

This is a plain static site (one self-contained `index.html`, no build step),
so Vercel needs zero configuration.

## Fastest way — Vercel Drop (no account setup, no CLI, no Git)
1. Go to https://vercel.com/drop
2. Drag this whole folder (or the zip) onto the page
3. Click Deploy — you get a live `yourproject.vercel.app` URL instantly

## Vercel CLI
```
npm i -g vercel
cd this-folder
vercel        # preview deploy
vercel --prod # production deploy
```

## GitHub + Vercel (best if you'll keep editing it)
1. Push this folder to a new GitHub repo
2. On vercel.com → Add New → Project → Import the repo
3. Vercel auto-detects it as a static site — just click Deploy
4. Every future `git push` auto-redeploys

Note: Vercel Drop creates a new project each time you drop — for repeat
updates to the *same* URL, use the GitHub method or the CLI.
