# Binom — binom.fr

One-page de Binom : sous-traitance dev (web, applications, backend) pour agences, studios et ESN.

HTML + CSS statiques, aucune dépendance, aucun build, aucune ressource externe (police Inter hébergée dans `assets/fonts`, licence OFL).

## Structure

```
index.html            la page (7 sections, ancres #offre #methode #pourquoi #equipe #contact)
mentions-legales.html mentions légales (servie sur /mentions-legales)
styles.css            styles mobile-first
assets/               favicon, photo de Tom, image de partage (og.png), police
vercel.json           cache des assets + en-têtes de sécurité
```

## Développement local

```bash
npx serve .          # ou : python3 -m http.server
```

## Déploiement Vercel

Importer le repo dans Vercel → Framework Preset : **Other**, pas de build command, output directory : racine.
Puis ajouter le domaine `binom.fr` dans *Settings → Domains*.

## À compléter plus tard

- **Mentions légales** : ajouter nom complet d'Antoine et les SIRET des deux micro-entreprises une fois l'immatriculation terminée (`mentions-legales.html`).
- **Photo d'Antoine** : déposer `assets/antoine.jpg` et remplacer le `<span class="person-mark">` par un `<img class="person-photo">`.
- **Nom de domaine** : le site tourne sur l'adresse gratuite `*.vercel.app`. Si un domaine est acheté plus tard, l'ajouter dans Vercel (*Settings → Domains*) et mettre à jour `og:image` dans `index.html`.
