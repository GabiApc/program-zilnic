# Cum pui aplicația pe GitHub Pages

## Fișiere necesare (toate în folderul program-app/)
- index.html
- manifest.json
- sw.js
- icon-192.png
- icon-512.png

---

## Pași

### 1. Creează un repo pe GitHub
Mergi pe github.com → New repository
- Name: `program-zilnic` (sau orice vrei)
- Public (obligatoriu pentru GitHub Pages gratuit)
- Nu bifa nimic altceva → Create repository

### 2. Inițializează și push din terminal
```bash
cd calea/spre/program-app
git init
git add .
git commit -m "init"
git branch -M main
git remote add origin https://github.com/USERNAME/program-zilnic.git
git push -u origin main
```
Înlocuiește USERNAME cu username-ul tău de GitHub.

### 3. Activează GitHub Pages
- Mergi în repo → Settings → Pages
- Source: Deploy from a branch
- Branch: main / (root)
- Save

### 4. Accesează aplicația
După ~1 minut aplicația e live la:
`https://USERNAME.github.io/program-zilnic`

---

## Instalare pe telefon (PWA)

### Android (Chrome)
- Deschide linkul în Chrome
- Apare automat un banner "Adaugă pe ecranul principal"
- Sau: meniu (⋮) → "Adaugă pe ecranul principal"

### iPhone (Safari)
- Deschide linkul în Safari (nu Chrome)
- Apasă butonul Share (pătratul cu săgeată)
- "Add to Home Screen"

---

## Update aplicație în viitor
Când vrei să modifici ceva, editezi fișierele și dai din nou:
```bash
git add .
git commit -m "update"
git push
```
GitHub Pages se actualizează automat în ~30 secunde.
