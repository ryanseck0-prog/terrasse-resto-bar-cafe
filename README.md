# Terrasse Resto Bar Café — Site vitrine

Site vitrine animé, une page, pour **Terrasse Resto Bar Café** (Dakar, Sénégal).
HTML / CSS / JavaScript natifs, sans build ni dépendance : le dossier se dépose tel quel sur n'importe quel hébergement statique.

**Site en ligne :** https://static.teamily.ai/sites/6a079efa-f204-4bb9-aa98-455a9f3cee6f/webpages/terrasse-dakar/index.html

---

## Le restaurant

| | |
|---|---|
| **Nom** | Terrasse Resto Bar Café |
| **Adresse** | Abdou Karim Bourgi angle 15, 10 Rue Dr. Theze, Dakar 10000 |
| **Téléphone / WhatsApp** | +221 71 119 87 87 |
| **Réservations** | +221 71 119 78 78 |
| **Horaires** | 8h00 – 00h00, 7j/7 |
| **Note Google** | 4,8 / 5 |
| **Cuisine** | Libanaise / méditerranéenne, bar à cocktails |
| **Instagram** | [@terrasserestobarcafe](https://www.instagram.com/terrasserestobarcafe/) |

---

## Fonctionnalités

- **Commande WhatsApp** — bouton flottant, boutons dans l'en-tête, la carte, le pied de page et le bandeau final. Chaque plat de la carte possède un bouton « + » qui ouvre WhatsApp avec le message pré-rempli (`Je souhaite commander : <plat>`).
- **Téléphone cliquable** — `tel:` dans la section « Nous trouver » et le pied de page.
- **Carte complète** — 91 plats et boissons avec prix en FCFA, répartis en 8 onglets (petit-déjeuner, mezzés, salades, sandwichs & burgers, grillades, pizzas & pâtes, desserts, boissons & bar), plus les liens vers les cartes PDF officielles.
- **Galerie** — lightbox avec navigation clavier (← → Échap) et boutons.
- **Carte Google Maps** intégrée + itinéraire.
- **Animations** — écran de chargement, hero en diaporama Ken Burns, titres révélés ligne par ligne, bandeau défilant, apparitions au scroll, onglets animés, barre de progression de lecture, menu mobile plein écran, bouton WhatsApp pulsant.
- **Responsive** — mobile, tablette, desktop ; respect de `prefers-reduced-motion`.

---

## Structure

```
.
├── index.html          # page unique (HTML + CSS + JS inline)
├── images/             # 18 visuels (photos de l'établissement + logo)
├── .nojekyll           # nécessaire pour GitHub Pages (sert les dossiers commençant par _)
└── README.md
```

---

## Lancer en local

Aucune installation. Ouvrir `index.html` dans un navigateur, ou servir le dossier :

```bash
python3 -m http.server 8000
# puis http://localhost:8000
```

---

## Déploiement

### GitHub Pages

1. **Settings → Pages**
2. *Source* : `Deploy from a branch`
3. *Branch* : `main` · *Folder* : `/ (root)`
4. Enregistrer — le site sort sur `https://<utilisateur>.github.io/terrasse-resto-bar-cafe/`

### Autre hébergement

Le dossier est statique : glisser-déposer sur Netlify, Vercel, Cloudflare Pages, un serveur Nginx/Apache, etc.

---

## Personnalisation

| Quoi | Où |
|---|---|
| Numéro WhatsApp | constante `WA_NUMBER` dans le `<script>` de `index.html` |
| Numéro de téléphone affiché | attributs `href="tel:..."` et textes de la section `#infos` |
| Plats et prix | tableaux de données dans le `<script>` (section carte) |
| Photos | remplacer les fichiers de `images/` en conservant les noms |
| Couleurs | variables CSS `:root` en haut du `<style>` |

---

## Sources des informations

- Fiche Google Maps de l'établissement (nom, adresse, téléphone, note, pluscode)
- Cartes PDF officielles (sur place, livraison, boissons) pour les plats et les prix
- Publications officielles Instagram / Facebook pour les horaires et les visuels

> Les prix et la carte évoluent : à revérifier périodiquement avec le restaurant.

---

## Licence

Contenu (textes, photos, marque) © Terrasse Resto Bar Café. Code du site fourni pour l'usage de l'établissement.
