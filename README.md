# SLZB-xxxx Advanced Dashboard Card 🚀

An advanced, dynamic, and all-in-one Home Assistant dashboard card for the **SMLIGHT SLZB-MRxx** (and other SLZB series) Zigbee/Multi-protocol coordinators.
Mine is a SLZB-MR4U [link](https://smlight.tech/global/slzbmr4)
|[README en Français🇫🇷](https://github.com/eTim/homeassistant-smlight-slzb-card/blob/cef5cd243a8bf94d183da0317b324c10046a7a07/README-FR.md)|[README in Italiano🇮🇹](https://github.com/eTim/homeassistant-smlight-slzb-card/blob/main/README-IT.md)|


## ✨ Features

- **Dynamic Header:** Real-time connection mode (Ethernet/Wi-Fi) and internet connectivity status.
- **Protocol Monitoring:** Live display of active protocols for both chips (EFR32 & CC2652).
- **Thermal Management:** Historical 24h graphs and live temperature for Core (ESP32) and both radio chips.
- **Resource Tracking:** Flash FileSystem and RAM usage monitoring with trend graphs.
- **Smart Maintenance:** - Conditional Update notifications (only shows when a firmware update is available).
    - Hardware controls: Hard Reset, Radio Reset, and Flash Mode.
- **Quick Settings:** LED Night Mode, Total LED toggle, and Auto-update settings.

## 🛠 Prerequisites

This card relies on several community-made frontend integrations. You must install these via **HACS** first:

1. [SMLIGHT SLZB intégration](https://www.home-assistant.io/integrations/smlight)
2. [Mushroom Cards](https://github.com/piitaya/lovelace-mushroom)
3. [Mini Graph Card](https://github.com/kalkih/mini-graph-card)
4. [Stack In Card](https://github.com/custom-cards/stack-in-card)
5. [Config Template Card](https://github.com/iantrich/config-template-card) (Crucial for dynamic naming)
6. [Card Mod](https://github.com/thomasloven/lovelace-card-mod) (Recommended)

## 🚀 Installation

1. Ensure your SLZB-MR4U is integrated into Home Assistant (via the official integration or MQTT).
2. Open your Home Assistant Dashboard.
3. Add a new **Manual Card**.
4. Copy the content of [slzb-card.yaml](./dashboards/slzb-card.yaml) and paste it into the editor.
5. **Note:** If your device entity prefix is not `sensor.slzb_mr4u_`, use the "Find and Replace" function to match your entity names.

## 📸 Screenshots

| Monitoring View | Maintenance View |
|-----------------|------------------|
| ![monitoring view](https://github.com/eTim/homeassistant-smlight-slzb-card/blob/c1c396fef67991bae9b9d54fb66a4c0060d0fdf7/Screenshot.png) | ![update pending view](https://github.com/eTim/homeassistant-smlight-slzb-card/blob/c989714db1aad393312720a1bae7b95a17d064f8/assets/Screenshot-update-pending.png)  |

## 🤝 Contributing

This is my first dashboard project! Feel free to open an **Issue** for bugs or a **Pull Request** if you have ideas for improvements (e.g., adding Power over Ethernet monitoring or more specific Zigbee stats).

Find more about this topics on https://community.home-assistant.io/t/share-advanced-dashboard-card-for-smlight-slzb/975278

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
