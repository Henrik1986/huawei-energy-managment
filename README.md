## Smart energihantering
HACS-paket för Home Assistant som optimerar din Huawei-batteriinstallation och solpaneler.
Styr laddningen automatiskt baserat på elpriser, batteriets status och solprognos för att maximera egenanvändningen.
Paketet gör även följande:

- Begränsar solelexport vid negativa elpriser
- Förhindrar att din elbil laddas från hemmabatteriet
- Säljer batteriöverskott när det är ekonomiskt lönsamt

<img width="1850" height="742" alt="Skärmbild 2025-10-11 163741" src="https://github.com/user-attachments/assets/8c306b50-f229-4a00-bfe9-e61b41ed0f2f" />

## Installation
### Steg 1
Installera och konfigurera [Huawei Solar Integrationen](https://github.com/wlcrs/huawei_solar)

<a href="https://my.home-assistant.io/redirect/config_flow_start/?domain=huawei_solar" target="_blank" rel="noreferrer noopener"><img src="https://my.home-assistant.io/badges/config_flow_start.svg" alt="Open your Home Assistant instance and start setting up a new integration." /></a>

### Steg 2
Installera och konfigurera [SMHI Integrationen](https://www.home-assistant.io/integrations/smhi/)

<a href="https://my.home-assistant.io/redirect/config_flow_start/?domain=smhi" target="_blank" rel="noreferrer noopener"><img src="https://my.home-assistant.io/badges/config_flow_start.svg" alt="Open your Home Assistant instance and start setting up a new integration." /></a>

### Steg 3
Installera följande integrationer från HACS (för att aktivera konfigurationsvyn):

- Apexcharts-card
- Layout-card
- Vertical-stack-in-card

Har du inte HACS?
Följ instruktionerna [här](https://www.hacs.xyz/docs/use/configuration/basic/)

### Steg 4
Lägg till följande rad i din configuration.yaml

```yml
homeassistant:
  packages: !include_dir_named packages
```
> [!IMPORTANT]
> Observera indraget — det ska placeras direkt under Home Assistant.

### Steg 5
Skapa en mapp på samma plats som din configuration.yaml-fil och namnge den packages.

### Steg 6
Ladda upp innehållet från package-mappen på GitHub till mappen du just skapade.

### Steg 7
Skapa en ny vy i Home Assistant genom att klicka på pennikonen uppe till höger och sedan på plus-tecknet (+).
I dialogrutan som visas, klicka på de tre prickarna uppe till höger och välj Redigera i YAML.
Klistra sedan in innehållet från filen admin_vy.yaml.

### Steg 8
Starta om Home Assistant

### Steg 9
Klicka in på din nya vy och starta konfigurationen genom att klicka på Inställningar

> [!NOTE]
> Om ett kort inte fungerar beror det troligtvis på att fel enhet/enheter används. Justera korten vid behov. Du behöver konfiguerar energivyn i Home Assistant för att få kortet som visar energiflödet. https://www.home-assistant.io/dashboards/energy/ 

## Uppdateringar :loudspeaker:
Detta är ingen officiell integration, vilket innebär att uppdateringar inte kommer automatiskt till Home Assistant. För att hålla dig uppdaterad om nya versioner är det enklast att ”följa” mitt repository. I varje ny realse kommer det framgå vilka filer du behöver uppdatera eller lägga till. 

Varje release innehåller information om:
- Nya funktioner
- Hur du uppdaterar paketet

## Framtida funktioner :raising_hand:
Har du idéer på nya funktioner? Lämna gärna dina förslag på GitHub under ”Discussions”.

## Problem :bug:
Upptäcker du något problem? Rapportera det gärna på GitHub under ”Issues”.

## Stötta mitt arbete 🚀
Gillar du paketet? Du får gärna stötta det!
Ditt stöd gör det möjligt för mig att fortsätta förbättra paketet, optimera funktioner och lägga till nya smarta funktioner i framtiden.

<a href="https://www.buymeacoffee.com/henrikakere" target="https://buymeacoffee.com/henrikakere"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
