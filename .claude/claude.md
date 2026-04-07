# LA FUTALERIE - Context Guide pour Claude Code

## 🎯 MISSION & POSITIONNEMENT

**La Futalerie est la PREMIÈRE friperie en ligne 100% grandes tailles hommes en France.**

### Proposition de valeur (StoryBrand Framework)
- **Le héros** : Hommes 30-55 ans, tailles XL à 5XL, qui galèrent à trouver des vêtements à leur taille
- **Leur problème** : Impossible de trouver des pantalons/jeans de qualité à leur taille sans payer une fortune
- **Leur guide** : La Futalerie - expert seconde main grandes tailles
- **Le plan** : Stock dédié 100% grandes tailles + mesures précises + contrôle qualité strict
- **L'appel à l'action** : "Enfin des jeans à ta taille"
- **Ce qu'ils évitent** : Frustration, perte de temps, argent gaspillé, humiliation en magasin
- **Ce qu'ils gagnent** : Confiance, style, économies (3x moins cher que neuf)

### Pain Points Client (PRIORITÉ ABSOLUE)

1. **TAILLES INCORRECTES** ⚠️ 
   - Problème #1 en seconde main : "étiqueté L mais taille M"
   - Impossible de savoir si ça va aller AVANT d'acheter
   - Solution La Futalerie : Mesures détaillées (épaules, longueur manches, tour poitrine) + photos précises

2. **MANQUE DE CHOIX**
   - Offre indigente en grandes tailles
   - Solution : 100% du catalogue grandes tailles

3. **QUALITÉ ALÉATOIRE**
   - Peur d'acheter un vêtement abîmé
   - Solution : Contrôle qualité strict, photos multiples

4. **PRIX EXCESSIFS (NEUF)**
   - Les grandes tailles = premium pricing
   - Solution : Seconde main = 3x moins cher

5. **ABSENCE DE CONSEIL**
   - Solitude dans le parcours d'achat
   - Solution : Guide morpho précis

## 💰 OFFRE PRODUIT

### Catalogue
- **Marques premium** : Levi's, Carhartt, Dickies, Wrangler, Lee
- **Tailles** : XL à 5XL (focus tailles réelles, pas juste étiquettes)
- **Prix moyen** : 30-50€ (vs 90-150€ neuf)
- **État** : Seconde main contrôlé, photos détaillées

### Garanties différenciantes
1. **Mesures précises** (pas juste "XL") : tour de taille, longueur jambe, tour cuisse, hanches
2. **Photos multiples** : face, dos, détails, défauts éventuels
3. **Contrôle qualité** : chaque pièce vérifiée
4. **Retours faciles** : sécurité totale
5. **Guide morpho** : "Si tu fais X tour de taille/Y longueur jambe → ce jean T'IRA"

## 🎨 DESIGN & UX - PRINCIPES OBLIGATOIRES

### Inspirations visuelles
- **Aged Ivy** (agedivy.com) : élégance sobre, masculin premium
- **Mango Outlet** : clarté, filtres efficaces, confiance
- **Jaiio** (jaiio.fr) : modernité française, seconde main haut de gamme

### Règles design STRICTES

#### 1. COULEURS & IDENTITÉ
- **Palette principale** : Tons neutres masculins (gris anthracite, beige, blanc cassé, noir)
- **Accent** : Un seul accent color (à définir) pour CTA
- **Éviter** : Couleurs criardes, trop de contrastes violents
- **Typographie** : Sans-serif moderne, lisible, poids variés (regular/medium/bold)

#### 2. PHOTOS PRODUITS
- **Fond blanc uniforme** obligatoire
- **Multiples angles** : face, dos, détails, défauts
- **Zoom haute qualité**
- **Photos portées** si possible (mannequin grande taille)
- **Badge "Mesures détaillées"** visible

#### 3. PAGE PRODUIT (PRIORITÉ CONVERSION)

**Structure obligatoire** :
```
[Photos carousel - 50% largeur desktop]  |  [Infos produit - 50% largeur]
                                         |  - Titre (Marque + Modèle)
                                         |  - Prix (actuel + "Neuf : XX€" barré)
                                         |  - Taille étiquette + "Voir mesures précises" ↓
                                         |  - État (Excellent/Très bon/Bon + description)
                                         |  - CTA "Ajouter au panier" (gros bouton)
                                         |  - "Retour gratuit si ça ne va pas"
                                         |
[Onglets dessous : Mesures détaillées | Guide taille | Matières & Entretien]
```

**Mesures détaillées (tableau clair)** :
- Tour de taille
- Longueur jambe (entrejambe)
- Tour de cuisse
- Largeur hanches
- Hauteur de taille (montant)

**Guide taille interactif** :
"Tes mesures : [input tour taille] [input longueur jambe] → Ce jean t'ira ✅ / risque d'être serré ⚠️"

#### 4. PAGE COLLECTION/LISTE PRODUITS

**Filtres OBLIGATOIRES (sidebar gauche)** :
- Taille réelle (tour de taille en cm : 90-95, 95-100, 100-105, etc.)
- Longueur jambe (cm)
- Marque
- Coupe (slim, regular, relaxed, wide)
- Prix
- État

**Grille produits** :
- 3-4 colonnes desktop
- Photo + Marque + Modèle + Prix + Taille + Badge état
- Hover : 2e photo ou zoom

**Tri** : Nouveautés / Prix croissant / Prix décroissant / Taille

#### 5. HOMEPAGE

**Hero Section** :
- Message clair : "Enfin des jeans à ta taille. Levi's, Carhartt, Dickies - Seconde main premium."
- Sous-titre : "Mesures détaillées. Contrôle qualité. Retour gratuit."
- CTA : "Voir les jeans" (vers collection)
- Visuel : Photo lifestyle homme grande taille stylé (PAS de stock photo générique)

**Section Réassurance** :
- 4 blocs icônes :
  1. "Mesures précises" (icône règle)
  2. "Contrôle qualité" (icône check)
  3. "Retour gratuit" (icône retour)
  4. "3x moins cher" (icône prix)

**Section Marques** :
- Logos : Levi's, Carhartt, Dickies, Wrangler, Lee

**Section Nouveautés** :
- Carrousel 4-6 derniers produits

**Section Témoignages** :
- 2-3 avis clients (focus sur "enfin trouvé ma taille", "qualité top", "mesures précises")

#### 6. MOBILE-FIRST
- **Priorité absolue** : 70% du trafic e-commerce est mobile
- Boutons CTA gros et tactiles (min 48px hauteur)
- Filtres en drawer/modal
- Photos swipables
- Sticky "Ajouter au panier" en bas

#### 7. PERFORMANCE
- Images optimisées (WebP, lazy loading)
- Score Lighthouse > 90
- Temps de chargement < 2s

## 🔍 SEO - STRATÉGIE OBLIGATOIRE

### Mots-clés principaux
1. **Primaires** : 
   - "jean grande taille homme"
   - "pantalon grande taille homme seconde main"
   - "levi's grande taille occasion"
   - "jean XXL pas cher"

2. **Longue traîne** :
   - "jean levi's 501 taille 46 occasion"
   - "pantalon carhartt grande taille seconde main"
   - "où acheter jean 5XL homme"

### Structure SEO pages

**Homepage** :
- Title : "La Futalerie - Jeans & Pantalons Grande Taille Homme Seconde Main | Levi's, Carhartt"
- Meta description : "Première friperie 100% grandes tailles hommes. Levi's, Carhartt, Dickies d'occasion. Mesures précises, contrôle qualité. 3x moins cher que neuf."
- H1 : "Jeans & Pantalons Grande Taille Homme - Seconde Main Premium"

**Pages produits** :
- Title : "[Marque] [Modèle] Taille [X] - Jean Grande Taille Homme Occasion | La Futalerie"
- Meta description : "[Marque] [Modèle] d'occasion en excellent état. Taille [X], mesures détaillées. [Prix]€ au lieu de [Prix neuf]€."
- H1 : "[Marque] [Modèle] - Jean Grande Taille Homme Taille [X]"

**Page collection** :
- Title : "Jeans Grande Taille Homme Seconde Main - Levi's, Carhartt, Dickies | La Futalerie"
- H1 : "Jeans & Pantalons Grande Taille Homme"

### Contenu SEO obligatoire

**Blocs texte (sous hero homepage)** :
```
## Pourquoi La Futalerie ?

La Futalerie est la première friperie en ligne 100% dédiée aux grandes tailles hommes. 
Fini de fouiller pendant des heures pour trouver UN jean à votre taille. Notre catalogue 
est entièrement composé de pantalons et jeans grandes tailles (XL à 5XL) de marques 
premium comme Levi's, Carhartt, Dickies, Wrangler et Lee.

### Des mesures précises, pas de mauvaises surprises

Nous savons que le problème #1 de la seconde main, c'est les tailles incorrectes. 
C'est pourquoi chaque article est mesuré précisément : tour de taille, longueur de jambe, 
tour de cuisse. Plus de doute avant d'acheter.

### Contrôle qualité strict

Chaque pièce est vérifiée, photographiée sous tous les angles. L'état est décrit avec 
transparence. Si un défaut existe, vous le verrez sur les photos.

### 3 fois moins cher que le neuf

Un Levi's 501 neuf grande taille coûte 90-120€. Chez nous : 30-40€. Même qualité, 
meilleur prix.
```

**Schema.org** (JSON-LD obligatoire) :
- Organization
- Product (chaque fiche produit avec prix, disponibilité, condition)
- BreadcrumbList

## 💳 CONVERSION - TACTIQUES OBLIGATOIRES

### Réassurance permanente
- Badge "Retour gratuit" visible sur toutes les pages produits
- Avis clients (minimum 3-5 témoignages)
- "Plus que X en stock" si pertinent (scarcité)
- "Vu récemment par X personnes" (preuve sociale)

### Urgence (sans abus)
- "Pièce unique" (c'est vrai en seconde main)
- Pas de faux countdown

### Checkout optimisé
- Guest checkout obligatoire (pas forcer création compte)
- Réassurance livraison/retour répétée
- Paypal + CB
- Champs minimum

### Email marketing (post-achat)
- Email confirmation + tracking
- Email "Comment ça te va ?" J+7
- Email réassortiment si nouvelle pièce à sa taille

### Abandons panier
- Email J+1 : "Tu as oublié ton [produit]"
- Code -10% si besoin

## 🛠️ TECH STACK & CONTRAINTES

### Shopify Theme
- **Repo** : https://github.com/lefr4ggerf0u/la-futalerie-shopify-theme-
- **Liquid** obligatoire pour templates
- **Sections** Shopify pour modularité
- **Metafields** pour mesures détaillées produits

### Metafields produits OBLIGATOIRES
```
measurements.waist (nombre) - Tour de taille en cm
measurements.inseam (nombre) - Longueur entrejambe en cm
measurements.thigh (nombre) - Tour de cuisse en cm
measurements.hip (nombre) - Tour de hanches en cm
measurements.rise (nombre) - Hauteur de taille en cm
condition.state (texte) - Excellent / Très bon / Bon
condition.description (texte) - Description détaillée état
original_price (nombre) - Prix neuf de référence
```

### Apps Shopify recommandées
- **Judge.me** : Avis clients
- **Loox** : Photos clients
- **Klaviyo** : Email marketing
- **Searchanise** : Recherche avancée + filtres
- **Bold Product Options** : Guide taille interactif (si besoin)

## 📝 MESSAGES CLÉS (COPYWRITING)

### À DIRE (obligatoire)
- "Enfin des jeans à ta taille"
- "Mesures précises, zéro mauvaise surprise"
- "Contrôle qualité strict"
- "3x moins cher que le neuf"
- "Retour gratuit si ça ne va pas"
- "100% grandes tailles, rien d'autre"

### À NE JAMAIS DIRE
- Mentionner Vinted, Leboncoin ou autres concurrents
- "Pour les hommes forts" (connotation négative)
- "Grandes tailles" seul (toujours préciser l'avantage)
- Jargon technique fashion incompréhensible

### Ton de voix
- **Masculin** sans être macho
- **Direct** et honnête
- **Rassurant** sans être condescendant
- **Accessible** (pas de snobisme fashion)
- Tutoiement

Exemples :
- ❌ "Découvrez notre sélection premium de denim japonais"
- ✅ "Des Levi's 501 à ta taille, enfin."

## 🚫 À ÉVITER ABSOLUMENT

### Design
- Stock photos génériques
- Carrousels illisibles sur mobile
- Pop-ups intrusifs (exit intent ok, pas au chargement)
- Trop d'animations
- Fonts illisibles

### UX
- Navigation complexe (max 2 niveaux)
- Filtres mal organisés
- Photos produits floues
- Descriptions vagues

### SEO
- Keyword stuffing
- Duplicate content
- URLs non optimisées

### Conversion
- Forcer création compte avant achat
- Frais cachés au checkout
- Process d'achat > 3 étapes

## ✅ CHECKLIST AVANT MISE EN PROD

### Design
- [ ] Mobile responsive testé sur iPhone/Android
- [ ] Toutes les images optimisées (WebP < 200KB)
- [ ] Fonts chargées correctement
- [ ] Couleurs cohérentes avec charte

### SEO
- [ ] Titles/meta descriptions tous remplis
- [ ] Schema.org ajouté
- [ ] Sitemap généré
- [ ] Google Analytics + Search Console

### Conversion
- [ ] Checkout fonctionnel
- [ ] Emails transactionnels configurés
- [ ] Avis clients affichés
- [ ] Réassurance visible partout

### Performance
- [ ] Lighthouse > 90
- [ ] Temps chargement < 2s
- [ ] Aucune erreur console

### Légal
- [ ] CGV
- [ ] Mentions légales
- [ ] Politique retours
- [ ] RGPD (cookies, données)

---

## 🎯 PROCHAINES ÉTAPES PRIORITAIRES

1. **V2 Design** : Refonte complète homepage + page produit selon guidelines ci-dessus
2. **Metafields** : Implémenter champs mesures détaillées
3. **Guide taille** : Créer calculateur interactif
4. **SEO** : Optimiser titles/meta + contenu
5. **Photos** : Shooter produits selon guidelines (fond blanc, multi-angles)

---

**Note pour Claude Code** : Ce fichier est le contexte complet du projet. Référence-toi TOUJOURS à ces guidelines avant de proposer du code, des modifications design ou des suggestions. En cas de doute, demande clarification plutôt que de dévier de ces principes.