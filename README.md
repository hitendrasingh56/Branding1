# Hitendra B. Singh — Personal Branding Website

## Important: correct GitHub upload structure
This ZIP has the website files directly at its root. After extracting, the folder you upload/deploy must contain these items immediately:
- `index.html`
- `package.json`
- `vite.config.js`
- `src/main.jsx`
- `src/App.jsx`
- `src/styles.css`
- `src/data/profile.js`
- `public/profile.jpg`
- `public/Hitendra-Singh-CV.pdf`

Do **not** upload a parent folder that contains another nested project folder. In GitHub, these files must appear at the repository's top level, with `src` and `public` as folders beside `index.html`.

## Run locally
1. Install Node.js LTS: https://nodejs.org/
2. Extract the ZIP.
3. Open a terminal in the extracted folder (the folder containing `package.json`).
4. Run:
   ```bash
   npm install
   npm run dev
   ```
5. Open the localhost address printed by Vite, usually `http://localhost:5173`.

## Production build
```bash
npm run build
npm run preview
```
The output is generated in `dist/`.

## GitHub
Upload the **contents** of the extracted project folder to the repository root, not an extra enclosing folder. Or use Git:
```bash
git init
git add .
git commit -m "Add personal branding website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

## Vercel project settings
- Framework Preset: `Vite`
- Root Directory: `./`
- Build Command: `npm run build`
- Output Directory: `dist`
- Install Command: `npm install`

The Vercel Root Directory must point to the folder that contains `package.json` and `index.html`. If the project is nested one level inside your GitHub repository, set Root Directory to that nested folder instead.

## Personalise
Edit `src/data/profile.js` for your profile text, experience, projects, education and contact links. Your supplied photo and CV are already included:
- `public/profile.jpg`
- `public/Hitendra-Singh-CV.pdf`

Review all content and confirm project details are approved for public disclosure before publishing.
