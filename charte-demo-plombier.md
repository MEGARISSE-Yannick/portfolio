# Charte graphique — Démo "Site Vitrine Essentiel" (artisan / plombier)
### Confiance technique × Réactivité × Sérieux sans fioritures

Projet démo pour l'offre **Site Vitrine Essentiel**. Palette définie par l'utilisateur (Dark Raspberry / Tea Green / Dusty Taupe / Steel Azure / Dark Khaki) — remplace l'ancienne piste bleu-marine/orange héritée de `YM/projets/essentiel.html`. Hérite de la charte mère (`CHARTE~1.MD`) pour la grille, l'espacement, les animations, l'accessibilité et le SEO (sections 3/4/6/8) — seules la palette et la typographie changent ci-dessous.

---

## 1. Palette

| Rôle | Nom | HEX | Usage |
|---|---|---|---|
| Dominante | Steel Azure | `#004385` | Header, footer, titres, CTA secondaire (texte blanc dessus) — bleu = confiance/technique, cohérent avec le métier (eau, tuyauterie) |
| Accent CTA principal | Dark Raspberry | `#82204A` | Bouton d'action principal ("Devis gratuit", "Appeler maintenant"), urgence — texte blanc dessus |
| Fond de section | Tea Green | `#CADBC0` | Sections alternées, cartes — respiration douce entre les blocs bleu/raspberry |
| Accent décoratif restreint | Dusty Taupe | `#A27E6F` | Icônes, bordures, badges, grands titres uniquement — **jamais en petit texte** (voir contrastes) |
| Texte corps | Dark Khaki | `#30321C` | Texte courant, remplace le slate générique |
| Fond principal | Blanc | `#FFFFFF` | Fond par défaut |

### Contrastes vérifiés (WCAG, formule officielle)

| Combinaison | Ratio | Verdict |
|---|---|---|
| Dark Khaki sur Blanc | 13.13:1 | ✅ AAA — texte courant |
| Steel Azure sur Blanc (titres) | 9.81:1 | ✅ AAA |
| **Blanc sur Steel Azure** (bouton/header) | 9.81:1 | ✅ AAA |
| **Blanc sur Dark Raspberry** (CTA principal) | 9.31:1 | ✅ AAA |
| Dark Khaki sur Tea Green | 9.01:1 | ✅ AAA — texte sur section claire |
| Dusty Taupe sur Blanc | 3.65:1 | ⚠️ Large/UI uniquement (titres ≥ 24px, icônes, bordures) — **jamais en texte courant** |
| Dark Khaki sur Dusty Taupe | 3.60:1 | ⚠️ Large/UI uniquement, même limite |

**Bonne nouvelle par rapport à l'ancienne palette orange** : Steel Azure et Dark Raspberry supportent tous les deux un texte blanc sans restriction (9.3–9.8:1) — plus besoin de la règle "texte foncé obligatoire sur les CTA" qui s'appliquait à l'orange. Seul le Dusty Taupe reste à usage restreint (comme le Sage dans la charte mère) : jamais en texte de lecture, uniquement en accent large ou décoratif.

---

## 2. Typographie

- **Titres (H1–H3)** : Oswald ou Barlow Semi Condensed, Bold/700 — condensé, droit, évoque le métier et la solidité plutôt que la mode.
- **Corps / UI** : Inter, 400–600 — lisible, neutre, cohérent avec la charte mère.
- Pas de troisième famille : la démo doit rester "un artisan sérieux qui répond vite", pas un exercice de style typographique.

---

## 3. Personnalité & ton

Direct, rassurant, orienté urgence/disponibilité ("intervention rapide", "devis gratuit"). Peu de texte, beaucoup d'action visible (téléphone, WhatsApp, formulaire court). C'est la démo la plus "commerciale" des trois — elle doit convertir en un coup d'œil, pas raconter une histoire. Le bleu Steel Azure porte la confiance technique, le Dark Raspberry porte l'urgence d'agir — deux signaux forts et distincts, sans troisième couleur qui viendrait diluer le message.

---

## 4. Ce qui ne change pas (hérité de `CHARTE~1.MD`)

Grille asymétrique et espacement (section 3), timings d'animation et `prefers-reduced-motion` (section 4), composants standards Header/Footer/formulaire (section 9), et l'intégralité des exigences perf/SEO/a11y/sécurité (section 8) — y compris le Schema.org `LocalBusiness` avec adresse et zone La Réunion.
