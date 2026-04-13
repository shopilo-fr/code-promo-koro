# Code promo KoRo, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo KoRo** depuis [shopilo.fr](https://shopilo.fr/reductions/koro.fr). Renvoie les **coupons KoRo** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-koro](https://shopilo-fr.github.io/code-promo-koro/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-koro
cd code-promo-koro
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "KoRo",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les snacks et superaliments en vrac",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/koro.fr"
  }
]
```

## Coupons KoRo disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les snacks et superaliments en vrac | [shopilo.fr](https://shopilo.fr/reductions/koro.fr) |

Codes actifs : **[shopilo.fr/reductions/koro.fr](https://shopilo.fr/reductions/koro.fr)**

## Questions frequentes

### Comment utiliser un code promo KoRo ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/koro.fr), ajoutez les produits a votre panier sur KoRo et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons KoRo ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction KoRo les plus recents ?
La page [shopilo.fr/reductions/koro.fr](https://shopilo.fr/reductions/koro.fr) est mise a jour quotidiennement avec les codes promo KoRo, bons de reduction KoRo et coupons promotionnels KoRo les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de KoRo

KoRo est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/koro.fr), retrouvez les meilleurs codes promo KoRo, coupons KoRo verifies et bons de reduction KoRo actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-koro
```

```javascript
const { fetchCoupons } = require('code-promo-koro');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
