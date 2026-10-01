# apps-legal

Pages légales publiques de toutes mes apps iOS (politique de confidentialité, assistance), publiées via GitHub Pages :
<https://kevinabrioux.github.io/apps-legal/>

Le repo est public parce que GitHub Pages l'exige (plan gratuit) ; il ne contient aucun code d'app.

## Organisation

```
assets/style.css            style commun (clair/sombre), lié par toutes les pages
index.html                  liste des apps
<app>/index.html            politique de confidentialité  → …/apps-legal/<app>/
<app>/support/index.html    assistance + FAQ              → …/apps-legal/<app>/support/
```

- `<app>` en minuscules, sans espace (`macrodaily`). Une fois publié, **ce chemin ne change plus** : il est saisi dans App Store Connect (« Privacy Policy URL », « Support URL ») et écrit dans le code de l'app.
- Pages bilingues EN + FR sur une seule page (ancres `#en` / `#fr`), comme les apps.
- Ajouter l'app dans `index.html`.
- Toute évolution de ce que l'app collecte (analytics, HealthKit, service tiers) → mettre à jour sa politique **et** le `PrivacyInfo.xcprivacy` de l'app.

## Historique

MacroDaily a encore ses pages dans le repo dédié `kevinabrioux/macrodaily-legal` (créé avant ce repo). Elles migreront ici lors d'une mise à jour de l'app (MacroDaily #292) , puis l'ancien repo sera archivé.
