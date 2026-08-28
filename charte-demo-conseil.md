# Charte graphique — Démo "Page de Conversion" (cabinet de conseil / coach)
### Sobriété corporate × Expertise × Épure

Projet démo pour l'offre **One-Page Conversion**. Palette définie par l'utilisateur (Ink Black / Deep Space Blue / Cerulean / Pale Slate / Alice Blue) — remplace l'ancienne piste Anthracite/Ivoire/Or. Hérite de la charte mère (`CHARTE~1.MD`) pour la grille, l'espacement, les animations, l'accessibilité et le SEO (sections 3/4/6/8) — seules la palette et la typographie changent ci-dessous. Toujours volontairement distincte des deux autres démos et de la charte mère (sauge/mauve/terracotta) : ici, un dégradé mono-teinte bleu marine du plus sombre au plus clair, avec un seul accent vif.

---

## 1. Palette

| Rôle | Nom | HEX | Usage |
|---|---|---|---|
| Texte corps | Ink Black | `#00171F` | Texte courant — le plus foncé de la gamme |
| Dominante | Deep Space Blue | `#003459` | Titres, header/footer, CTA secondaire (texte blanc dessus) |
| Accent unique | Cerulean | `#007EA7` | CTA principal — **toujours en fond de bouton avec texte blanc, jamais en texte de lecture** |
| Fond secondaire | Pale Slate | `#C7CCDB` | Sections alternées, cartes, bordures |
| Fond principal | Alice Blue | `#E1E5EE` | Fond clair par défaut (remplace l'Ivoire) |

Toujours un seul accent vif (Cerulean) sur une base mono-teinte bleu marine : la sobriété reste l'argument de vente de cette démo.

### Contrastes vérifiés (WCAG, formule officielle)

| Combinaison | Ratio | Verdict |
|---|---|---|
| Ink Black sur Alice Blue | 14.57:1 | ✅ AAA — texte courant |
| Ink Black sur Pale Slate | 11.46:1 | ✅ AAA |
| Deep Space Blue sur Alice Blue (titres) | 10.17:1 | ✅ AAA |
| **Blanc sur Deep Space Blue** (header/CTA secondaire) | 12.84:1 | ✅ AAA |
| **Blanc sur Cerulean** (CTA principal) | 4.62:1 | ✅ AA normal — tout juste au-dessus du seuil, à ne pas assombrir davantage |
| Ink Black sur Cerulean (texte) | 3.98:1 | ⚠️ Échoue en texte courant, large/UI seulement |
| **Cerulean sur Alice Blue** (texte/lien) | 3.67:1 | ⚠️ Échoue en texte courant (< 4.5), large/UI seulement |
| Cerulean sur Pale Slate (texte/lien) | 2.88:1 | ❌ Échoue même en large — à éviter |

**Règle d'or de cette démo** : Cerulean ne fonctionne comme texte de lecture nulle part dans cette palette — c'est exclusivement une couleur de **fond de bouton** (avec texte blanc, 4.62:1, marge faible donc ne pas y ajouter d'opacité ou de dégradé qui l'assombrirait). Pour un lien ou un texte d'accent, utiliser Deep Space Blue à la place.

---

## 2. Typographie

- **Titres (H1–H3)** : Fraunces ou Source Serif 4, 600–700 — une serif éditoriale pour signaler l'expertise et le recul, à l'opposé du monospace "dev" de la charte mère. Avec cette palette plus froide (bleu marine/cerulean) que l'ancienne version ivoire/or, le rendu penche légèrement plus "corporate moderne" que "boutique chaleureuse" — toujours premium, avec un peu plus d'arête.
- **Corps / UI** : Inter, 400–500 — sobre, laisse la serif porter la personnalité.

---

## 3. Personnalité & ton

Confiant, posé, peu de mots mais chacun pèse. Une seule page, une seule promesse par section (accroche → expertise → preuve sociale → FAQ → contact), aucune surcharge visuelle. Le dégradé mono-teinte (du Ink Black au Alice Blue) structure la profondeur des sections sans jamais introduire de couleur parasite ; le Cerulean, unique et réservé au bouton principal, concentre toute l'attention sur l'action de conversion.

---

## 4. Ce qui ne change pas (hérité de `CHARTE~1.MD`)

Grille asymétrique et espacement (section 3), timings d'animation — ici particulièrement le scroll reveal soigné en Framer Motion, cœur de l'expérience one-page (section 4), composants standards (section 9), exigences perf/SEO/a11y/sécurité (section 8).
