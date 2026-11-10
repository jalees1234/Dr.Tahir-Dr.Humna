# Tahir & Humna wedding invitation

The latest invitation with larger/bolder hero and ending text, lighter Mehndi/Barat overlays, champagne Walima, animations, countdown, music controls and scroll progress. All starter media are included. This is a standalone React + Vite project configured for Vercel; no database, login or environment variables required.

## Deploy on Vercel
This folder is the project root: `package.json` and `vercel.json` are here. Push this folder's contents to GitHub, then import that repository in Vercel. Vercel uses the included Vite settings to run `npm run build` and serve `dist`. The project requires Node.js 22.12 or newer; select a compatible Node.js version in Vercel's project settings if needed. No environment variables are required.

To push to a new, empty GitHub repository from PowerShell:

```powershell
git init
git add .
git commit -m "Initial wedding website"
git branch -M main
git remote add origin https://github.com/USERNAME/REPOSITORY.git
git push -u origin main
```

Replace `USERNAME/REPOSITORY` with your GitHub account and repository name. In Vercel, choose **Add New > Project**, import the repository, and deploy. Future pushes to `main` trigger deployments automatically.

Official guide: https://vercel.com/docs/frameworks/frontend/vite

## Local preview on Windows
Install Node.js 22.12 or newer. Open this folder in VS Code and run:

```bash
npm ci
npm run dev
```

Open the local URL printed in the terminal. Do not double-click index.html.
To verify the production build:

```bash
npm run build
npm run preview
```

## Personalise
Edit public/wedding-config.json and put replacement media in public/media.
- song: /media/your-song.mp3
- backgroundPhoto: /media/your-couple-photo.jpg
- events: video, poster, time, venue and description for each event.
- countdownTo: currently midnight 18 December 2026 in Pakistan (+05:00).

Use H.264 MP4 video and MP3 audio. The supplied videos are animated starter venue photos and the music is a starter instrumental; replace them with your choices. Music begins after tapping to open; some phones may require tapping the music button. Venues and timings currently say To be announced.

The main invitation is src/App.tsx. Styles are src/styles.css. Push edits to GitHub to trigger a new Vercel deployment. File names and letter casing must match the config exactly. No RSVP is included.
