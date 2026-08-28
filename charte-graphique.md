# Charte Graphique — Style Tropical / Minimaliste

## 1. Couleurs

| Nom | Hex | Usage |
|---|---|---|
| Cream (Fond principal clair) | `#F3F9D2` | Backgrounds, dégradés légers |
| Tea Green (Vert clair) | `#CBEAA6` à vérifier | Accents secondaires, hovers, badges |
| Willow Green (Vert principal) | `#C0D684` | Boutons primaires, liens, icônes nature |
| Midnight Violet (Violet profond) | `#3D0B37` | Titres forts, footer, contraste élégant |
| Blackberry Cream (Violet moyen) | `#63264A` | CTA secondaires, textes importants, bordures |
| Texte corps alternatif | `#1A1A1A` | Noir doux pour texte corps |

> **Note importante — code Tea Green à vérifier :** le code hexadécimal `#CBEAA6` fourni ne comporte que 5 caractères après le `#`, ce qui le rend invalide en CSS. Il est recommandé de vérifier et de compléter ce code avant intégration. Deux options proches sont à considérer, sans trancher à la place de l'utilisateur : `#C9E4A6` (valeur suggérée, utilisée par défaut dans les exemples CSS ci-dessous) ou `#CBEBA6`. Le code fourni `#CBEAA6` est conservé ici comme référence **à vérifier**.

## 2. Utilisation recommandée

### Backgrounds

- Utiliser **Cream** (`#F3F9D2`) comme fond principal clair.
- Employer des dégradés très légers entre **Cream** et des nuances végétales pour créer de la profondeur sans alourdir l'interface.
- Réserver **Midnight Violet** (`#3D0B37`) aux sections fortes, au footer ou à certains bandeaux de contraste.

### Texte corps

- Privilégier **#1A1A1A** pour le texte courant afin d'obtenir un noir doux, plus confortable à lire qu'un noir pur.
- Maintenir un contraste suffisant avec les fonds clairs et éviter les paragraphes trop longs.

### Titres

- Utiliser **Midnight Violet** pour les titres principaux et les accroches à fort impact.
- Utiliser **Blackberry Cream** pour les sous-titres, textes importants et mises en avant secondaires.

### Boutons primaires

- Utiliser **Willow Green** (`#C0D684`) pour les actions principales : prise de contact, réservation, demande de devis ou découverte d'une offre.
- Associer ce fond à un texte **Midnight Violet** pour conserver une identité naturelle et un contraste élégant.

### Boutons secondaires / WhatsApp

- Utiliser **Blackberry Cream** (`#63264A`) pour les CTA secondaires et les appels à l'action WhatsApp.
- Prévoir des boutons larges, particulièrement visibles sur mobile, avec une zone de clic confortable.

### Accents végétaux / icônes

- Utiliser **Willow Green** pour les icônes nature, éléments décoratifs, séparateurs et accents végétaux.
- Utiliser **Tea Green** pour les hovers, badges et accents secondaires, après validation de son code hexadécimal.

### Mode sombre optionnel

- Utiliser **Midnight Violet** comme fond sombre principal.
- Employer **Cream** pour les textes clairs et **Willow Green** pour les actions et accents.
- Vérifier les contrastes et réduire les grandes surfaces très lumineuses afin de préserver le confort visuel.

## 3. Typographie

- **Titres :** Poppins ou Inter, en graisse Bold / Semi-bold.
- **Corps :** Inter ou System UI, en graisse Regular.
- Prévoir des tailles généreuses pour les titres et les éléments clés.
- Utiliser un `line-height` d'au moins `1.6` pour les paragraphes et une hiérarchie visuelle nette.
- Laisser beaucoup d'espace blanc afin de renforcer l'impression minimaliste et premium.

## 4. Style global

- Direction artistique **clean**, aérée et chaleureuse.
- Utiliser des photos haute qualité représentant notamment :
  - les plages ;
  - la nature réunionnaise ;
  - la nourriture créole ;
  - les coiffures ;
  - les villas.
- Privilégier les coins arrondis sur les cartes, boutons, champs et blocs d'image.
- Ajouter des micro-animations douces : `fade`, léger `scale` au survol et transitions courtes.
- Adopter une conception **mobile-first**.
- Prévoir des boutons larges, notamment pour les actions WhatsApp.
- Utiliser des icônes simples, en styles **line** et **filled**, avec une dominante verte.
- Conserver un ton : **chaleureux, local, professionnel et orienté résultat**.

## 5. Exemples de code CSS (variables)

```css
:root {
  --cream: #F3F9D2;
  /* Valeur suggérée à valider : le code fourni #CBEAA6 est incomplet. */
  --tea-green: #C9E4A6;
  --willow-green: #C0D684;
  --midnight-violet: #3D0B37;
  --blackberry-cream: #63264A;
  --text-dark: #1A1A1A;
}

body {
  background: var(--cream);
  color: var(--text-dark);
  font-family: Inter, system-ui, sans-serif;
  line-height: 1.6;
}

h1,
h2,
h3,
h4 {
  color: var(--midnight-violet);
  font-family: Poppins, Inter, system-ui, sans-serif;
  font-weight: 700;
}
```

## 6. Boutons (exemples)

### Bouton primaire

Fond **Willow Green**, texte **Midnight Violet** :

```css
.button-primary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 3rem;
  padding: 0.875rem 1.5rem;
  border: 0;
  border-radius: 999px;
  background: var(--willow-green);
  color: var(--midnight-violet);
  font: 600 1rem/1.2 Inter, system-ui, sans-serif;
  cursor: pointer;
  transition: transform 180ms ease, filter 180ms ease;
}

.button-primary:hover,
.button-primary:focus-visible {
  filter: brightness(0.96);
  transform: scale(1.02);
}
```

### Bouton secondaire / WhatsApp

Fond **Blackberry Cream**, texte **Cream** :

```css
.button-secondary,
.button-whatsapp {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 3rem;
  padding: 0.875rem 1.5rem;
  border: 0;
  border-radius: 999px;
  background: var(--blackberry-cream);
  color: var(--cream);
  font: 600 1rem/1.2 Inter, system-ui, sans-serif;
  cursor: pointer;
  transition: transform 180ms ease, filter 180ms ease;
}

.button-secondary:hover,
.button-secondary:focus-visible,
.button-whatsapp:hover,
.button-whatsapp:focus-visible {
  filter: brightness(1.08);
  transform: scale(1.02);
}

/* Sur mobile, le bouton WhatsApp peut occuper toute la largeur disponible. */
@media (max-width: 640px) {
  .button-whatsapp {
    width: 100%;
  }
}
```
