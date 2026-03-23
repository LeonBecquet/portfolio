# Portfolio — Léon Becquet

## Déployer sur Vercel

### 1. Push sur GitHub
```bash
git init
git add .
git commit -m "portfolio"
git branch -M main
git remote add origin https://github.com/LeonBecquet/portfolio.git
git push -u origin main
```

### 2. Déployer
1. Va sur [vercel.com](https://vercel.com) → **Sign up with GitHub**
2. **Add New Project** → importe `LeonBecquet/portfolio`
3. Laisse tout par défaut → **Deploy**
4. Ton site est live en 30 secondes sur `portfolio-xxx.vercel.app`

### 3. Domaine personnalisé
1. Sur Vercel : **Settings** → **Domains** → ajoute `leonbecquet.dev`
2. Vercel te donne un record DNS à configurer (type A ou CNAME)
3. Va chez ton registrar (Cloudflare/Porkbun) → ajoute le record DNS
4. Attends 5 min → `leonbecquet.dev` est live avec HTTPS auto

## Structure
```
portfolio/
├── index.html      ← Le portfolio
├── vercel.json     ← Config Vercel
├── .gitignore
└── README.md
```

## Mettre à jour
Modifie `index.html` → push sur GitHub → Vercel redéploie automatiquement.
