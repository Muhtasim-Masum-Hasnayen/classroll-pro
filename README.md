# ClassRoll Pro

Smart card-based attendance website for teachers. Bangla / English, light / dark, guest mode, Excel import and report.

## Structure
```
index.html
css/style.css
js/app.js
assets/favicon.svg
vercel.json
```
Plain HTML, CSS and JavaScript. No build step, no npm install.

## Run locally
Open `index.html` in a browser, or in VS Code use the **Live Server** extension (right click `index.html` > Open with Live Server).

## Deploy: GitHub then Vercel
1. Create a new repository on GitHub, then in this folder run:
   ```
   git init
   git add .
   git commit -m "ClassRoll Pro first version"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/classroll-pro.git
   git push -u origin main
   ```
2. Go to vercel.com, click **Add New > Project**, import the repository.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Click **Deploy**.

## Important notes
- Login and saved data are a **demo**: accounts and data live only in the visitor's browser (localStorage). For real accounts, a backend such as Firebase or Supabase is needed.
- The Excel library (SheetJS) loads from cdnjs, so an internet connection is required.
- SMS, offline sync and payments are shown as Pro features but are not implemented yet.
