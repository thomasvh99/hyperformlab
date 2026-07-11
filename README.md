# Hyperform.Lab — site web

Site statique (HTML/CSS pur, aucune dépendance, aucun build nécessaire).

## Structure

```
index.html              → sélecteur de langue (racine)
style.css                → feuille de style partagée par tout le site
fr/                       → version française
  index.html
  avancees-scientifiques.html
  carrousel-zanini-2025.html
en/                       → version anglaise
  index.html
  scientific-advances.html
  carousel-zanini-2025.html
assets/
  slides-fr/               → images du carrousel (FR), slide-01.png à slide-08.png
  slides-en/                → images du carrousel (EN), slide-01.png à slide-08.png
```

## Ajouter une nouvelle étude

Pour chaque nouvelle étude : générer les images de slides (FR + EN), les déposer dans
`assets/slides-<langue>/`, puis dupliquer le pattern d'une carte dans
`avancees-scientifiques.html` / `scientific-advances.html` (image de couverture,
résumé, lien DOI) et créer la page de visionneuse correspondante sur le modèle de
`carrousel-zanini-2025.html`.

## Déploiement

Site 100% statique — déployable tel quel sur Netlify, Vercel, GitHub Pages, ou Bolt.new
(pas d'étape de build, pas de `package.json` requis).
