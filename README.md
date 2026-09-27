# Binom — binom.fr

One-page de Binom : sous-traitance dev (web, applications, backend) pour agences, studios et ESN.

HTML + CSS statiques, aucune dépendance, aucun build. Seule ressource externe : la police Inter (Google Fonts).

## Structure

```
index.html            la page (7 sections, ancres #offre #methode #pourquoi #equipe #contact)
styles.css            styles mobile-first
assets/               favicon + photos placeholder
vercel.json           cache des assets + en-têtes de sécurité
```

## Développement local

```bash
npx serve .          # ou : python3 -m http.server
```

## Déploiement Vercel

Importer le repo dans Vercel → Framework Preset : **Other**, pas de build command, output directory : racine.
Puis ajouter le domaine `binom.fr` dans *Settings → Domains*.

## À faire avant la mise en ligne

- **Photos** : déposer `assets/tom.jpg` et `assets/antoine.jpg` (carré, ~480×480) et remplacer les `src` des deux `<img class="person-photo">` dans `index.html`.
- **Mentions légales** : obligatoires pour une activité pro en France (identité, SIRET, hébergeur Vercel). À ajouter en pied de page.
- **Email** : tous les CTA pointent vers `tom.lemenand@gmail.com` (sujet « Renfort dev — [nom entreprise] » + trame de message pré-remplie). Un rechercher/remplacer suffit pour passer à une adresse `@binom.fr`.
