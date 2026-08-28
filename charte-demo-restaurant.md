# Charte graphique — Démo "Site avec Fonctionnalité Métier" (restaurant, réservation de table)
### Appétence × Chaleur vive × Prise de RDV sans friction

Projet démo pour l'offre **Site avec Fonctionnalité Métier**. Palette définie par l'utilisateur (Verdigris / Deep Space Blue / Canary Yellow / Tangerine Dream / Watermelon) — remplace l'ancienne piste teal/blush/corail. Secteur resserré sur le **restaurant** (la palette, très "appétit" — jaune canari, tangerine, pastèque — s'y prête mieux qu'au salon de coiffure envisagé initialement). Hérite de la charte mère (`CHARTE~1.MD`) pour la grille, l'espacement, les animations, l'accessibilité et le SEO (sections 3/4/6/8) — seules la palette et la typographie changent ci-dessous.

---

## 1. Palette

| Rôle | Nom | HEX | Usage |
|---|---|---|---|
| Texte corps / dominante sombre | Deep Space Blue | `#0B3142` | Texte courant, header/footer, texte sur fonds clairs de la palette |
| Fond principal | Blanc chaud | `#FFFBF2` *(ajouté, hors palette fournie)* | Fond par défaut — nécessaire comme base neutre, aucune des 5 couleurs fournies n'est assez neutre pour de grandes zones de texte |
| Fond d'accent / surlignage | Canary Yellow | `#FFFD82` | Sections menu/promo, encarts mis en avant — toujours avec texte Deep Space Blue |
| Fond chaleureux secondaire | Tangerine Dream | `#FF9B71` | Cartes, badges, hover — toujours avec texte Deep Space Blue |
| CTA principal | Watermelon | `#E84855` | Bouton "Réserver une table" — voir contrainte de taille ci-dessous |
| Accent restreint | Verdigris | `#1B998B` | Icônes, bordures, petits accents décoratifs — **jamais en texte courant** |

### Contrastes vérifiés (WCAG, formule officielle)

| Combinaison | Ratio | Verdict |
|---|---|---|
| Deep Space Blue sur Blanc chaud | 13.70:1 | ✅ AAA — texte courant |
| Deep Space Blue sur Canary Yellow | 12.80:1 | ✅ AAA |
| Deep Space Blue sur Tangerine Dream | 6.64:1 | ✅ AA normal |
| Blanc sur Tangerine Dream | 2.06:1 | ❌ Échoue — ne jamais mettre de texte blanc sur ce fond |
| **Blanc sur Watermelon** (CTA) | 3.82:1 | ⚠️ Large/UI uniquement |
| Deep Space Blue sur Watermelon (CTA) | 3.58:1 | ⚠️ Large/UI uniquement, quasi identique |
| Blanc sur Verdigris | 3.51:1 | ⚠️ Large/UI uniquement |
| Deep Space Blue sur Verdigris | 3.90:1 | ⚠️ Large/UI uniquement |

**Règle d'or de cette démo** : Watermelon et Verdigris sont des couleurs à luminance moyenne — ni le blanc ni le Deep Space Blue n'y passent le seuil de texte courant (4.5:1), seulement le seuil large/UI (3:1). Conséquence concrète : **le bouton CTA "Réserver une table" doit toujours utiliser un texte en gras ≥ 18px (ou 14px bold)** — jamais de petit texte fin sur ces deux couleurs, peu importe la teinte choisie (blanc ou foncé).

---

## 2. Typographie

- **Titres (H1–H3)** : Fraunces, variante italique autorisée pour les accroches — chaleureux et personnel, évoque le plaisir de table plutôt que la technique.
- **Corps / UI** : Inter, 400–500.
- Le formulaire de réservation reste en Inter uniquement, jamais de serif sur un champ de formulaire.

---

## 3. Personnalité & ton

Vif, appétissant, convivial — la palette la plus saturée des trois démos, assumée comme telle pour un restaurant (contraste volontaire avec la sobriété du cabinet de conseil et le sérieux du plombier). Le Deep Space Blue ancre l'ensemble et garde le site lisible malgré la vivacité des accents. Le formulaire de réservation, cœur technique de cette démo, reste néanmoins d'une clarté absolue : un champ par ligne, label toujours visible, feedback de validation immédiat — la gaieté est dans le design, la rigueur dans le formulaire.

---

## 4. Ce qui ne change pas (hérité de `CHARTE~1.MD`)

Grille asymétrique et espacement (section 3), timings d'animation (section 4), composants standards — en particulier le formulaire de contact/réservation avec validation serveur + honeypot (sections 8 et 9), exigences perf/SEO/a11y/sécurité (section 8).
