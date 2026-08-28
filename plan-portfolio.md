# Plan complet pour créer le Portfolio

## Objectif & positionnement

### Qui ?

Un freelance web/design basé à La Réunion, capable de concevoir des identités visuelles, des sites web modernes et des expériences numériques claires, rapides et adaptées aux usages locaux.

### Pour qui ?

- Entrepreneurs et indépendants qui lancent ou professionnalisent leur activité.
- TPE, commerces, restaurants, hébergements touristiques et associations de La Réunion.
- Marques locales qui souhaitent mieux valoriser leur savoir-faire en ligne.
- Structures ayant besoin d’un site vitrine, d’une landing page ou d’une refonte de leur présence digitale.

### Promesse de résultat

Créer des supports web et visuels élégants, utiles et performants, qui transforment une activité locale en présence digitale crédible, mémorable et génératrice de contacts — avec une approche simple, humaine et orientée résultats.

### Territoire de marque

Le portfolio adopte un style **Tropical / Minimaliste** : une interface lumineuse et aérée, inspirée des paysages de l’île sans tomber dans le décoratif excessif. Les formes organiques, les touches végétales et une palette naturelle renforcent la proximité, tandis que la hiérarchie minimaliste maintient une lecture professionnelle.

## Sitemap

```text
Accueil
├── À propos
├── Services
├── Portfolio
│   └── Détail d’un projet
├── Témoignages
├── Contact / WhatsApp
└── Blog (optionnel)
```

## Structure de la page d'accueil

| Section | Contenu | Objectif |
|---|---|---|
| Hero | Phrase de positionnement, sous-titre orienté bénéfice, visuel tropical minimaliste et CTA principal « Parlons de votre projet » | Comprendre immédiatement l’offre et encourager le premier contact |
| Preuve rapide | Chiffres clés, secteurs accompagnés, années d’expérience ou logos clients | Rassurer en quelques secondes |
| Problème → Solution | Situations fréquentes des prospects puis méthode proposée pour y répondre | Montrer que le freelance comprend les enjeux avant de vendre une prestation |
| Services | 3 à 5 services présentés dans des cards : site vitrine, identité visuelle, landing page, UI/UX, maintenance | Clarifier l’offre et orienter chaque visiteur |
| Portfolio preview | 3 à 4 projets mis en avant avec image, catégorie, courte description et lien « Voir le projet » | Prouver la qualité du travail par des exemples concrets |
| Témoignages | Citations courtes, nom, activité et éventuellement photo ou logo | Apporter une preuve sociale authentique |
| CTA final | Résumé de la promesse, invitation à échanger et boutons Contact / WhatsApp | Convertir les visiteurs intéressés en prospects |
| Footer | Coordonnées, liens de navigation, réseaux sociaux, zone géographique, mentions légales et copyright | Faciliter l’accès aux informations essentielles et renforcer la confiance |

## Page Portfolio (galerie de projets)

### Filtres par catégorie

Prévoir des filtres visibles et accessibles au clavier pour permettre une exploration rapide :

- **Tous les projets**
- Sites vitrines
- E-commerce / réservation
- Identité visuelle
- Landing pages
- UI/UX et direction artistique

Le filtre doit rester simple sur mobile : boutons ou onglets déroulants, état actif clairement identifiable et possibilité de revenir à « Tous les projets ».

### Grid de cards

La galerie peut utiliser une grille responsive de 1 colonne sur mobile, 2 colonnes sur tablette et 3 colonnes sur grand écran. Chaque card projet comprend :

- Une image de couverture optimisée, avec ratio homogène.
- Le nom du projet et le secteur d’activité.
- Une catégorie sous forme de badge.
- Une phrase présentant l’enjeu principal.
- Un lien ou bouton « Découvrir le projet ».

### Détail d'un projet

Chaque étude de cas doit raconter une histoire et mettre en évidence la valeur créée :

1. **Problème** : contexte du client, public cible et difficultés rencontrées.
2. **Solution** : démarche, choix UX/UI, identité visuelle, fonctionnalités et accompagnement.
3. **Résultat chiffré** : données disponibles et vérifiables, par exemple +35 % de demandes, temps de chargement inférieur à 3 secondes ou nombre de réservations générées.
4. **Screenshots** : vues desktop et mobile, détails d’interface et, si pertinent, avant/après.
5. **Lien live** : bouton vers le site en ligne, ouvert dans un nouvel onglet, lorsque le projet est public.
6. **CTA** : invitation à demander une réalisation similaire via le formulaire ou WhatsApp.

## Composants UI réutilisables

- **Bouton primaire — Willow Green** : bouton principal d’action, fond vert doux Willow Green, texte contrasté, angles légèrement arrondis, états hover/focus visibles et libellé explicite.
- **Bouton WhatsApp flottant — Blackberry Cream** : bouton circulaire ou pilule fixé en bas de l’écran, en Blackberry Cream avec icône WhatsApp, accessible sur mobile sans masquer le contenu et accompagné d’un libellé ou d’une infobulle.
- **Card projet** : composant réutilisable avec image, badge de catégorie, titre, résumé, éventuel indicateur de résultat et lien d’action.
- **Badge — Tea Green** : petite étiquette Tea Green destinée aux catégories, technologies ou secteurs ; texte suffisamment contrasté et taille lisible.
- **Section title — Midnight Violet Poppins Bold** : titre de section en Poppins Bold, couleur Midnight Violet, avec une accroche courte et un espacement généreux pour structurer la page.

## Stack technique recommandée

| Besoin | Option simple | Option pro |
|---|---|---|
| Site | Webflow, Framer ou WordPress avec un thème léger | Next.js / Astro avec composants sur mesure et CMS headless |
| Hébergement | Hébergement mutualisé fiable ou plan Webflow/Framer | Vercel ou Netlify avec CDN, déploiement Git et prévisualisations |
| Formulaire contact | Formulaire natif Webflow/Framer ou Formspree | API serverless, Resend ou service transactionnel avec anti-spam et suivi des conversions |
| Images | WebP/AVIF compressées avec Squoosh ou ImageOptim | Pipeline automatisé d’optimisation, images responsives et CDN avec lazy loading |

Le choix final doit privilégier la facilité de mise à jour, les performances, l’accessibilité et l’autonomie du freelance. Une option simple est pertinente pour lancer rapidement le portfolio ; l’option pro devient intéressante lorsque le volume de projets ou les besoins éditoriaux augmentent.

## Étapes de production

1. **Contenu** : définir le positionnement, rédiger les textes, sélectionner 4 à 6 projets et recueillir les résultats, témoignages et visuels autorisés.
2. **Wireframe** : organiser les blocs de la home, du portfolio et du contact avant de travailler les détails graphiques.
3. **Design HD avec charte** : fixer la palette Tropical / Minimaliste, les typographies, les espacements, les composants, les états interactifs et la direction photo.
4. **Développement mobile-first** : construire les pages en partant des petits écrans, puis enrichir l’expérience tablette et desktop.
5. **Intégration WhatsApp** : ajouter un CTA de contact direct, un bouton flottant accessible et un message prérempli adapté au contexte.
6. **Tests responsive** : vérifier les breakpoints, la navigation, les formulaires, les images, les contrastes et les interactions sur plusieurs appareils.
7. **SEO local** : optimiser les titres, méta-descriptions, données structurées, pages de services, mentions de La Réunion, fiche Google Business Profile et maillage interne.
8. **Mise en ligne + domaine** : connecter le domaine, activer HTTPS, configurer les redirections, les pages légales et les sauvegardes.
9. **Analytics** : installer une solution de mesure respectueuse de la vie privée, définir les événements importants et suivre les clics WhatsApp, formulaires et projets consultés.

## Checklist avant lancement

- [ ] Bouton WhatsApp visible sur mobile sans gêner la lecture.
- [ ] Temps de chargement inférieur à 3 secondes sur une connexion mobile réaliste.
- [ ] 4 à 6 projets présentés avec des résultats concrets et, lorsque possible, chiffrés.
- [ ] Formulaire fonctionnel : réception testée, message de confirmation et protection anti-spam actifs.
- [ ] Responsive testé sur mobile, tablette et desktop, avec navigation au clavier.
- [ ] Cohérence de la charte graphique : couleurs Willow Green, Blackberry Cream, Tea Green et Midnight Violet, typographies et composants homogènes.
- [ ] Liens, boutons, filtres, liens live et réseaux sociaux vérifiés.
- [ ] Images compressées, textes alternatifs renseignés et titres structurés.
- [ ] Mentions légales, politique de confidentialité et consentement analytics vérifiés si nécessaires.

## Prochaines étapes possibles

Deux livrables peuvent servir à passer rapidement à la réalisation :

- Un **wireframe texte détaillé de la home**, section par section, avec les contenus, CTA, indications de hiérarchie et variantes mobile/desktop.
- Le **code HTML/CSS/Tailwind** du portfolio, avec une base responsive, les composants UI réutilisables, la palette Tropical / Minimaliste et les emplacements prévus pour les projets.
