# La Futalerie — Thème Shopify

Thème Shopify personnalisé pour **La Futalerie**, boutique de jeans et pantalons de marque (Levi's, Carhartt, Dickies, Wrangler, Lee) de seconde main.

Basé sur **Dawn 15.4.1** (thème officiel gratuit Shopify), customisé pour une expérience de conversion optimisée.

---

## Installation dans Shopify

### Méthode 1 — Via GitHub (recommandée)

1. Aller dans **Shopify Admin → Boutique en ligne → Thèmes**
2. Cliquer **Ajouter un thème → Se connecter à GitHub**
3. Autoriser Shopify à accéder à votre GitHub
4. Sélectionner le repo `la-futalerie-shopify-theme`
5. Cliquer **Importer du GitHub**
6. Prévisualiser → **Publier**

### Méthode 2 — Upload ZIP

1. Télécharger ce repo en ZIP (bouton Code → Download ZIP)
2. **Shopify Admin → Boutique en ligne → Thèmes → Ajouter un thème → Télécharger un fichier ZIP**
3. Prévisualiser → Publier

---

## Après l'installation — Configuration Shopify

### 1. Navigation (menus)

Dans **Admin → Boutique en ligne → Navigation** :

**Menu principal** (handle : `main-menu`) :
- Accueil → `/`
- Pantalons → `/collections/all`
- À propos → `/pages/a-propos`
- FAQ → `/pages/faq`
- Contact → `/pages/contact`

### 2. Pages à créer

Dans **Admin → Boutique en ligne → Pages** :

| Titre | Handle | Template |
|-------|--------|----------|
| À propos | `a-propos` | `page.about` |
| FAQ | `faq` | `page.faq` |
| Contact | `contact` | `page.contact` |

Pour chaque page :
1. Créer la page avec le bon titre
2. Dans la section "Modèle de thème", sélectionner le bon template

### 3. Collections

Dans **Admin → Produits → Collections** :

Créer une collection principale :
- Nom : `Pantalons`
- Handle : `all` (ou utiliser la collection automatique Shopify)
- Description : "Jeans et pantalons Levi's, Carhartt, Dickies, Wrangler, Lee — sélection experte de seconde main."

Pour les filtres (Marque, Taille), aller dans **Admin → Boutique en ligne → Navigation → Menus de filtres** et créer des filtres basés sur les tags produit.

### 4. Ajouter vos produits

Format recommandé pour le titre :
```
Levi's 501 - Taille 32/34 - Excellent état
```

**Tags recommandés** (pour les filtres) :
- Marque : `marque-levis`, `marque-carhartt`, `marque-dickies`, `marque-wrangler`, `marque-lee`
- Taille : `taille-28`, `taille-30`, `taille-32`, `taille-34`, etc.
- État : `etat-excellent`, `etat-tres-bon`, `etat-bon`

**Description produit** — Structure recommandée :
```
Marque : Levi's
Modèle : 501
Taille étiquette : 32W / 34L
État : Excellent

Mesures réelles (à plat) :
- Tour de taille : 42 cm (x2 = 84 cm)
- Longueur totale : 108 cm
- Entrejambe : 82 cm
- Largeur cuisse : 30 cm
- Ouverture bas : 19 cm

[Description de la pièce, particularités, défauts éventuels]
```

### 5. Photo hero homepage

Dans l'éditeur de thème (Admin → Boutique en ligne → Thèmes → Personnaliser) :
- Cliquer sur la section **Hero La Futalerie**
- Uploader une photo de jeans/workwear (idéalement 1800px de large)

### 6. Paramètres importants

Dans **Admin → Paramètres** :
- **Paiements** : Activer PayPal, Apple Pay, Google Pay
- **Expédition** : Configurer Colissimo (4,90€ + gratuit dès 80€)
- **Emails** : Personnaliser les emails transactionnels
- **Checkout** : Activer le paiement sans compte

---

## Customisations effectuées

### Design
- Palette de couleurs vintage/workwear (blanc cassé, charcoal, vert forêt, camel)
- Typographie : DM Serif Display (titres) + Inter (corps)
- Cards produit avec bordure et ombre légère

### Sections custom
| Fichier | Description |
|---------|-------------|
| `sections/futalerie-hero.liquid` | Hero plein écran avec overlay, double CTA, trust bar |
| `sections/futalerie-reviews.liquid` | Avis clients (cards avec étoiles) |
| `sections/futalerie-usps.liquid` | 3 colonnes avantages |
| `sections/futalerie-process.liquid` | Comment ça marche (3 étapes) |
| `sections/futalerie-comparison.liquid` | Tableau comparatif vs Vinted |
| `sections/futalerie-trust-bar.liquid` | Barre de réassurance (paiement, livraison…) |
| `sections/futalerie-newsletter.liquid` | Inscription newsletter |
| `sections/futalerie-about.liquid` | Contenu page À propos |
| `sections/futalerie-faq.liquid` | FAQ avec accordéons |

### Templates
- `templates/index.json` — Homepage avec 9 sections
- `templates/product.json` — Fiche produit en français avec badges de confiance
- `templates/collection.json` — Collection avec filtres et barre de réassurance
- `templates/page.about.json` — Page À propos
- `templates/page.faq.json` — Page FAQ complète

---

## Apps recommandées (post-lancement)

- **Avis** : Judge.me (gratuit) ou Loox
- **Emails** : Klaviyo (panier abandonné, séquences)
- **Chat** : Tidio (gratuit) ou Gorgias
- **Analytics** : Google Analytics 4 (via Shopify)

---

[Getting started](#getting-started) |
[Staying up to date with Dawn changes](#staying-up-to-date-with-dawn-changes) |
[Developer tools](#developer-tools) |
[Contributing](#contributing) |
[Code of conduct](#code-of-conduct) |
[Theme Store submission](#theme-store-submission) |
[License](#license)

Dawn represents a HTML-first, JavaScript-only-as-needed approach to theme development. It's Shopify's first source available theme with performance, flexibility, and [Online Store 2.0 features](https://www.shopify.com/partners/blog/shopify-online-store) built-in and acts as a reference for building Shopify themes.

* **Web-native in its purest form:** Themes run on the [evergreen web](https://www.w3.org/2001/tag/doc/evergreen-web/). We leverage the latest web browsers to their fullest, while maintaining support for the older ones through progressive enhancement—not polyfills.
* **Lean, fast, and reliable:** Functionality and design defaults to “no” until it meets this requirement. Code ships on quality. Themes must be built with purpose. They shouldn’t support each and every feature in Shopify.
* **Server-rendered:** HTML must be rendered by Shopify servers using Liquid. Business logic and platform primitives such as translations and money formatting don’t belong on the client. Async and on-demand rendering of parts of the page is OK, but we do it sparingly as a progressive enhancement.
* **Functional, not pixel-perfect:** The Web doesn’t require each page to be rendered pixel-perfect by each browser engine. Using semantic markup, progressive enhancement, and clever design, we ensure that themes remain functional regardless of the browser.

You can find a more detailed version of our theme code principles in the [contribution guide](https://github.com/Shopify/dawn/blob/main/.github/CONTRIBUTING.md#theme-code-principles).

## Getting started
We recommend using Dawn as a starting point for theme development. [Learn more on Shopify.dev](https://shopify.dev/themes/getting-started/create).

> If you're building a theme for the Shopify Theme Store, then you can use Dawn as a starting point. However, the theme that you submit needs to be [substantively different from Dawn](https://shopify.dev/themes/store/requirements#uniqueness) so that it provides added value for merchants. Learn about the [ways that you can use Dawn](https://shopify.dev/themes/tools/dawn#ways-to-use-dawn).

Please note that the main branch may include code for features not yet released. The "stable" version of Dawn is available in the theme store.

## Staying up to date with Dawn changes

Say you're building a new theme off Dawn but you still want to be able to pull in the latest changes, you can add a remote `upstream` pointing to this Dawn repository.

1. Navigate to your local theme folder.
2. Verify the list of remotes and validate that you have both an `origin` and `upstream`:
```sh
git remote -v
```
3. If you don't see an `upstream`, you can add one that points to Shopify's Dawn repository:
```sh
git remote add upstream https://github.com/Shopify/dawn.git
```
4. Pull in the latest Dawn changes into your repository:
```sh
git fetch upstream
git pull upstream main
```

## Developer tools

There are a number of really useful tools that the Shopify Themes team uses during development. Dawn is already set up to work with these tools.

### Shopify CLI

[Shopify CLI](https://github.com/Shopify/shopify-cli) helps you build Shopify themes faster and is used to automate and enhance your local development workflow. It comes bundled with a suite of commands for developing Shopify themes—everything from working with themes on a Shopify store (e.g. creating, publishing, deleting themes) or launching a development server for local theme development.

You can follow this [quick start guide for theme developers](https://shopify.dev/docs/themes/tools/cli) to get started.

### Theme Check

We recommend using [Theme Check](https://github.com/shopify/theme-check) as a way to validate and lint your Shopify themes.

We've added Theme Check to Dawn's [list of VS Code extensions](/.vscode/extensions.json) so if you're using Visual Studio Code as your code editor of choice, you'll be prompted to install the [Theme Check VS Code](https://marketplace.visualstudio.com/items?itemName=Shopify.theme-check-vscode) extension upon opening VS Code after you've forked and cloned Dawn.

You can also run it from a terminal with the following Shopify CLI command:

```bash
shopify theme check
```

### Continuous Integration

Dawn uses [GitHub Actions](https://github.com/features/actions) to maintain the quality of the theme. [This is a starting point](https://github.com/Shopify/dawn/blob/main/.github/workflows/ci.yml) and what we suggest to use in order to ensure you're building better themes. Feel free to build off of it!

#### Shopify/lighthouse-ci-action

We love fast websites! Which is why we created [Shopify/lighthouse-ci-action](https://github.com/Shopify/lighthouse-ci-action). This runs a series of [Google Lighthouse](https://developers.google.com/web/tools/lighthouse) audits for the home, product and collections pages on a store to ensure code that gets added doesn't degrade storefront performance over time.

#### Shopify/theme-check-action

Dawn runs [Theme Check](#Theme-Check) on every commit via [Shopify/theme-check-action](https://github.com/Shopify/theme-check-action).

## Contributing

Want to make commerce better for everyone by contributing to Dawn? We'd love your help! Please read our [contributing guide](https://github.com/Shopify/dawn/blob/main/.github/CONTRIBUTING.md) to learn about our development process, how to propose bug fixes and improvements, and how to build for Dawn.

## Code of conduct

All developers who wish to contribute through code or issues, please first read our [Code of Conduct](https://github.com/Shopify/dawn/blob/main/.github/CODE_OF_CONDUCT.md).

## Theme Store submission

The [Shopify Theme Store](https://themes.shopify.com/) is the place where Shopify merchants find the themes that they'll use to showcase and support their business. As a theme partner, you can create themes for the Shopify Theme Store and reach an international audience of an ever-growing number of entrepreneurs.

Ensure that you follow the list of [theme store requirements](https://shopify.dev/themes/store/requirements) if you're interested in becoming a [Shopify Theme Partner](https://themes.shopify.com/services/themes/guidelines) and building themes for the Shopify platform.

## License

Copyright (c) 2021-present Shopify Inc. See [LICENSE](/LICENSE.md) for further details.
