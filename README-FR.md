# Carte de Dashboard Avancée pour SLZB-xxxx 🚀

Une carte Home Assistant avancée, dynamique et tout-en-un pour les coordinateurs Zigbee/Multi-protocoles **SMLIGHT SLZB-MRxx** (et autres séries SLZB).  
Le modèle utilisé ici est un SLZB-MR4U [lien vers le produit](https://smlight.tech/global/slzbmr4).

## ✨ Fonctionnalités

- **En-tête Dynamique :** Affichage du mode de connexion en temps réel (Ethernet/Wi-Fi) et statut de la connectivité Internet.
- **Monitoring des Protocoles :** Affichage en direct des protocoles actifs pour les deux puces (EFR32 & CC2652).
- **Gestion Thermique :** Graphiques historiques sur 24h et températures en direct pour le CPU (ESP32) et les deux puces radio.
- **Suivi des Ressources :** Occupation du système de fichiers (Flash) et utilisation de la RAM avec graphiques de tendance.
- **Maintenance Intelligente :** - Notifications de mise à jour conditionnelles (apparaissent uniquement lorsqu'un nouveau firmware est disponible).
    - Contrôles matériels : Redémarrage (Hard Reset), Reset Radio et Mode Flash.
- **Réglages Rapides :** Gestion du mode nuit des LEDs, extinction totale des LEDs et paramètres de mise à jour automatique.

## 🛠 Prérequis

Cette carte repose sur plusieurs intégrations de la communauté. Vous devez d'abord les installer via **HACS** :

1. [Intégration SMLIGHT SLZB officielle](https://www.home-assistant.io/integrations/smlight)
2. [Mushroom Cards](https://github.com/piitaya/lovelace-mushroom)
3. [Mini Graph Card](https://github.com/kalkih/mini-graph-card)
4. [Stack In Card](https://github.com/custom-cards/stack-in-card)
5. [Config Template Card](https://github.com/iantrich/config-template-card) (**Indispensable** pour l'affichage dynamique des noms de puces)
6. [Card Mod](https://github.com/thomasloven/lovelace-card-mod) (Recommandé)

## 🚀 Installation

1. Assurez-vous que votre SLZB est bien intégré à Home Assistant (via l'intégration officielle ou MQTT).
2. Ouvrez votre tableau de bord Home Assistant.
3. Ajoutez une nouvelle carte de type **Manuel** (bouton "Manuel" tout en bas de la liste).
4. Copiez le contenu du fichier [slzb-card.yaml](./dashboards/slzb-card.yaml) et collez-le dans l'éditeur.
5. **Note :** Si le préfixe de vos entités n'est pas `sensor.slzb_mr4u_`, utilisez la fonction "Rechercher et Remplacer" (Ctrl+H) de votre éditeur pour faire correspondre le code à vos propres noms d'entités.

## 📸 Captures d'écran

| Vue Monitoring | Vue Maintenance |
|-----------------|------------------|
| ![vue monitoring](https://raw.githubusercontent.com/eTim/homeassistant-smlight-slzb-card/main/Screenshot.png) | *Bientôt disponible* |

## 🤝 Contribution

C'est mon tout premier projet de dashboard ! N'hésitez pas à ouvrir une **Issue** pour signaler un bug ou une **Pull Request** si vous avez des idées d'amélioration (ex: ajout du monitoring PoE ou statistiques Zigbee spécifiques).

## 📄 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.
