# 7Lagg

**7Lagg** est un plugin Minecraft développé pour **Paper 1.20.2+** qui permet de **nettoyer automatiquement les items au sol** pour réduire le lag sur votre serveur.

Développé avec amour par [7ka1], ce plugin est simple, efficace et personnalisable.

---

## ⚙️ Fonctionnalités

- Nettoyage automatique des items au sol toutes les X minutes (configurable)
- Annonce dans le chat avant chaque nettoyage
- Commandes admin pour :
  - Forcer un nettoyage (`/clean`)
  - Recharger la configuration (`/clean reload`)
  - Activer/désactiver le nettoyage auto (`/clean toggle`)
- Système de permissions pour sécuriser les commandes

---

## ⌨️ Commandes

| Commande             | Description                                    | Permission         |
|----------------------|------------------------------------------------|---------------------|
| `/clean`             | Supprime immédiatement tous les items au sol   | `7lagg.clean`       |
| `/clean reload`      | Recharge la configuration                     | `7lagg.reload`      |
| `/clean toggle`      | Active/Désactive le nettoyage automatique     | `7lagg.toggle`      |

---

## ⚙️ Configuration (`config.yml`)

```yaml
cleanup-interval-minutes: 5
cleanup-warning-delay-seconds: 10
pre-cleanup-message: "Les items au sol seront supprimés dans {delay} secondes."
post-cleanup-message: "{count} items supprimés."
