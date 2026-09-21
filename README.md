# Cap Permis B

Outil web gratuit de **suivi personnel** pour préparer l'examen pratique du permis de conduire.
Il aide à voir ce qui est acquis, ce qu'il reste à travailler, et à réviser les questions de l'examen.

Site : https://cap-permisb.fr

## Fonctionnalités

- **Bilan** : une jauge de maîtrise globale, avec objectif réglable et compte à rebours avant l'examen.
- **Checklist** : 78 réflexes de conduite à évaluer (À travailler, En progrès, Automatisé), avec notes personnelles.
- **Questions** : les 100 fiches de l'examen (vérification intérieure ou extérieure, sécurité routière, premiers secours). On entre un numéro de 1 à 100 pour afficher les 3 questions, ou on parcourt toutes les fiches.
- **Plan de travail** : les réflexes à travailler à la prochaine leçon, avec une fiche à copier ou télécharger.
- **Évolution** : courbe de progression et journal de conduite.
- **Jour J** : préparation de la veille et du matin, respiration guidée, exercices de confiance.
- **Mode d'emploi**, **mentions légales** et **rappel de sauvegarde**.
- **Contact** : e-mail de l'auteur et lien vers le groupe Facebook « cap-permisb.fr - Réussir Examen Permis B ».

## Confidentialité

Aucune donnée n'est envoyée à un serveur. La progression, les notes et les réglages sont enregistrés
dans le navigateur de l'utilisateur (`localStorage`). Une sauvegarde manuelle est proposée dans les Réglages.

## Structure du dépôt

| Fichier | Rôle |
|---|---|
| `index.html` | Le site (HTML, CSS et JavaScript dans un seul fichier) |
| `mentions-legales.html` | Le texte des mentions légales, chargé par `index.html` |
| `CNAME` | Nom de domaine personnalisé (créé par GitHub Pages) |
| `icon.svg`, `favicon.ico`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png` | Icônes du site |
| `og-image.png` | Image affichée quand on partage le lien |
| `site.webmanifest` | Nom et icônes pour l'installation sur mobile |
| `sitemap.xml` | Liste des pages, pour Google Search Console |
| `robots.txt` | Autorise l'indexation et indique le plan du site |
| `README.md` | Ce fichier |
| `.gitignore` | Fichiers à ne pas publier |

## Utiliser en local

Ouvrir `index.html` dans un navigateur. Aucune installation n'est nécessaire.
En local, les mentions légales s'affichent depuis une copie intégrée à `index.html`.

## Déploiement

Le site est hébergé sur **GitHub Pages** (*Settings → Pages → Deploy from a branch → `main` / `(root)`*).
Le domaine `cap-permisb.fr` est enregistré chez OVH. Sa zone DNS contient quatre enregistrements `A`
vers les adresses de GitHub Pages, et un `CNAME` pour `www`. Voir la documentation GitHub :
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

Pour mettre à jour le site, remplacer le fichier concerné dans le dépôt : GitHub Pages republie automatiquement.

## Modifier le contenu

Dans `index.html` :

- la liste des réflexes est dans la variable `RAW` ;
- les 100 fiches de questions sont dans la variable `QB` ;
- le texte des mentions légales est dans `mentions-legales.html`. Une copie de secours est intégrée dans `index.html`
  (variable `LEGAL_FALLBACK`) : la mettre à jour aussi.

## Contenu et droits

© 2026 l'auteur du site. Tous droits réservés : toute réutilisation du site (code, design, textes) nécessite son accord.

Les questions de l'examen sont issues d'un document officiel. Elles ont été reprises, regroupées et reformulées
pour ce site. Elles ne sont pas couvertes par ces droits réservés.

## Avertissement

Cap Permis B est un outil d'auto-évaluation. Il ne remplace ni une école de conduite, ni les conseils d'un moniteur,
et ne garantit pas la réussite à l'examen. Les contenus peuvent ne plus être à jour : vérifier auprès d'une école
de conduite ou des sources officielles.

## Contact

devby.fou@gmail.com
