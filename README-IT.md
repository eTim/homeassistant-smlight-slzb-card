# Dashboard Card Avanzata per SLZB-xxxx 🚀

Una card per Home Assistant avanzata, dinamica e "tutto-en-uno" per i coordinatori Zigbee/Multi-protocollo **SMLIGHT SLZB-MRxx** (e altre serie SLZB).  
Il modello utilizzato qui è un SLZB-MR4U [link al prodotto](https://smlight.tech/global/slzbmr4).

## ✨ Funzionalità

- **Intestazione Dinamica:** Visualizzazione in tempo reale della modalità di connessione (Ethernet/Wi-Fi) e dello stato della connettività Internet.
- **Monitoraggio Protocolli:** Visualizzazione live dei protocolli attivi per entrambi i chip (EFR32 & CC2652).
- **Gestione Termica:** Grafici storici delle ultime 24 ore e temperature in diretta per la CPU (ESP32) e i due chip radio.
- **Monitoraggio Risorse:** Occupazione del FileSystem (Flash) e utilizzo della RAM con grafici di tendenza.
- **Manutenzione Intelligente:** - Notifiche di aggiornamento condizionali (appaiono solo quando è disponibile un nuovo firmware).
    - Controlli hardware: Riavvio (Hard Reset), Reset Radio e Modalità Flash.
- **Impostazioni Rapide:** Gestione modalità notte dei LED, spegnimento totale dei LED e impostazioni per l'aggiornamento automatico.

## 🛠 Prerequisiti

Questa card si basa su diverse integrazioni della community. È necessario installarle prima tramite **HACS**:

1. [Integrazione ufficiale SMLIGHT SLZB](https://www.home-assistant.io/integrations/smlight)
2. [Mushroom Cards](https://github.com/piitaya/lovelace-mushroom)
3. [Mini Graph Card](https://github.com/kalkih/mini-graph-card)
4. [Stack In Card](https://github.com/custom-cards/stack-in-card)
5. [Config Template Card](https://github.com/iantrich/config-template-card) (**Indispensabile** per la visualizzazione dinamica dei nomi dei chip)
6. [Card Mod](https://github.com/thomasloven/lovelace-card-mod) (Raccomandato)

## 🚀 Installazione

1. Assicurati che il tuo SLZB sia correttamente integrato in Home Assistant (tramite integrazione ufficiale o MQTT).
2. Apri la tua Dashboard di Home Assistant.
3. Aggiungi una nuova card di tipo **Manuale** (pulsante "Manuale" in fondo alla lista).
4. Copia il contenuto del file [slzb-card.yaml](./dashboards/slzb-card.yaml) e incollalo nell'editor.
5. **Nota:** Se il prefisso delle tue entità non è `sensor.slzb_mr4u_`, usa la funzione "Trova e Sostituisci" (Ctrl+H) del tuo editor per far corrispondere il codice ai nomi delle tue entità.

## 📸 Screenshot

| Vista Monitoraggio | Vista Manutenzione |
|-----------------|------------------|
| ![vista monitoraggio](https://github.com/eTim/homeassistant-smlight-slzb-card/blob/c1c396fef67991bae9b9d54fb66a4c0060d0fdf7/Screenshot.png)  | *Prossimamente disponibile* |

## 🤝 Contributo

Questo è il mio primo progetto dashboard! Non esitare ad aprire una **Issue** per segnalare un bug o una **Pull Request** se hai idee per miglioramenti (es: aggiunta del monitoraggio PoE o statistiche Zigbee specifiche).

## 📄 Licenza

Questo progetto è rilasciato sotto licenza MIT - vedi il file [LICENSE](LICENSE) per ulteriori dettagli.
