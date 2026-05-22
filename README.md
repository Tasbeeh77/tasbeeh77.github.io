# Tasbeeh Gamal Eissa — Portfolio

A fast, single-file personal portfolio. No build step, no frameworks — just open `index.html`.
Designed to be hosted **free** on GitHub Pages.

---

## ✏️ How to edit (the only thing you need to know)

Everything you'll ever change lives in **one place**: the `DATA = { ... }` object inside the
`<script>` near the bottom of `index.html`. It's clearly marked:

```
⬇⬇⬇  EDIT EVERYTHING HERE  ⬇⬇⬇
```

From there you can change your intro, about text, experience bullets, skills, and projects
without touching any layout or CSS.

**To add a project**, copy one block inside `projects: [ ... ]` and edit it:

```js
{ name:"My New Project", lang:"C#", repo:"https://github.com/Tasbeeh77/repo-name", live:"",
  desc:"One or two sentences about what it does and what you built." },
```

- `repo` → link to the GitHub code (leave as `""` to hide the Code link)
- `live` → link to a live demo (leave as `""` to hide the Live link)

**To change theme colors**, edit the `:root { --accent: ... }` values at the top of the `<style>` block.

---

## 📄 Updating your CV download

The **Download CV** button serves the file at `assets/Tasbeeh_Gamal_Eissa_CV.pdf`.
To update it, just replace that PDF with a new one of the **same name** (or change the
`cv:` path in the `DATA.links` object).

---

## 🚀 Publish it free on GitHub Pages (≈10 minutes)

This gives you a permanent URL: **https://tasbeeh77.github.io**

1. On GitHub, create a **new public repository** named exactly:
   ```
   Tasbeeh77.github.io
   ```
   (Your username, then `.github.io` — this special name makes it your main site.)

2. Upload these files to the repo (keep the folder structure):
   ```
   index.html
   README.md
   assets/Tasbeeh_Gamal_Eissa_CV.pdf
   ```
   Either drag-and-drop in the GitHub web UI ("Add file → Upload files"), or push from your terminal:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/Tasbeeh77/Tasbeeh77.github.io.git
   git push -u origin main
   ```

3. In the repo: **Settings → Pages**. Under "Build and deployment", set
   **Source = Deploy from a branch**, **Branch = `main`**, folder = `/ (root)`. Save.

4. Wait 1–2 minutes, then visit **https://tasbeeh77.github.io** 🎉

Every time you push a change to `main`, the live site updates automatically.

---

## 🔗 Add it to your CV and LinkedIn

Once live, add `tasbeeh77.github.io` to your CV header and your LinkedIn "Website" field.

---

Built with plain HTML/CSS/JS. Fonts: Fraunces + IBM Plex (Google Fonts).
