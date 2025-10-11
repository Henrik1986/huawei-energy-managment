## Smart Energy Managment
HACS package for Home Assistant to optimize your Huawei battery and solar panels. Control charging based on prices, battery state, and solar forecast to maximize self-consumption.

<img width="1850" height="742" alt="Skärmbild 2025-10-11 163741" src="https://github.com/user-attachments/assets/8c306b50-f229-4a00-bfe9-e61b41ed0f2f" />
Bilden ovan visar adminvyn via Home Assistant

> [!IMPORTANT]
> You have du adjust the code to your setup.

## Installation
### Steg 1
Installera och konfigurera [Huawei Solar Integration](https://github.com/wlcrs/huawei_solar)

<a href="https://my.home-assistant.io/redirect/config_flow_start/?domain=https%3A%2F%2Fgithub.com%2Fwlcrs%2Fhuawei_solar" target="_blank" rel="noreferrer noopener"><img src="https://my.home-assistant.io/badges/config_flow_start.svg" alt="Open your Home Assistant instance and start setting up a new integration." /></a>

### Steg 2
Installera och konfigurera [SMHI integrationen]((https://www.home-assistant.io/integrations/smhi/))

### Steg 3
Installera integrationer från HACS
- Apexcharts-card
- Layout-card
- Stack-In-Card

### Steg 4
Lägg till nedanstående rad i din configuration fil. 

Note
Observera indenteringen och att det ligger direkt under Home Assistant 

#### Steg 5
Skapa en mapp som du döper till package.

### Steg 6
Ladda upp innehållet från mappen package till din mapp med samma namn. 

### Steg 7
Skapa en ny vy och klicka på prickarna uppe till höger. Välj redigera i yaml. Klistra in innehållet som finns i filen admin_vy.yaml

### Steg 8
Starta om Home Assistant 

### Steg 9
Klicka in på din nya vy och starta konfigurationen genom att klicka på ....
