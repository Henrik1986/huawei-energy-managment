## Smart Energy Managment
HACS package for Home Assistant to optimize your Huawei battery and solar panels. Control charging based on prices, battery state, and solar forecast to maximize self-consumption.

<img width="1850" height="742" alt="Skärmbild 2025-10-11 163741" src="https://github.com/user-attachments/assets/8c306b50-f229-4a00-bfe9-e61b41ed0f2f" />
Bilden ovan visar adminvyn via Home Assistant

## Installation
### Steg 1
Installera och konfigurera [Huawei Solar Integration](https://github.com/wlcrs/huawei_solar)

<a href="https://my.home-assistant.io/redirect/config_flow_start/?domain=huawei_solar" target="_blank" rel="noreferrer noopener"><img src="https://my.home-assistant.io/badges/config_flow_start.svg" alt="Open your Home Assistant instance and start setting up a new integration." /></a>

### Steg 2
Installera och konfigurera [SMHI Integrationen](https://www.home-assistant.io/integrations/smhi/)

<a href="https://my.home-assistant.io/redirect/config_flow_start/?domain=smhi" target="_blank" rel="noreferrer noopener"><img src="https://my.home-assistant.io/badges/config_flow_start.svg" alt="Open your Home Assistant instance and start setting up a new integration." /></a>

### Steg 3
Installera följande integrationer från HACS för att kunna visa energivyn
- Apexcharts-card 
- Layout-card
- Vertical-stack-in-card

Har du inte HACS? 
Följ instruktionerna [här](https://www.hacs.xyz/docs/use/configuration/basic/)

### Steg 4
Lägg till nedanstående rad i configuration.yaml. 

```yml
homeassistant:
  packages: !include_dir_named packages
```
> [!IMPORTANT]
> Observera indenteringen och direkt under Home Assistant. 

### Steg 5
Skapa en mapp på samma ställe som du hittar din configuration.yaml. Döp mappen till packages. 

### Steg 6
Ladda upp innehållet från mappen package på Github till mappen du precis skapade. 

### Steg 7
Skapa en ny vy i Home Assistant genom att klicka på penna upp till höger och klicka sen på pluset. I rutan du fick upp ska du nu klicka på de tre prickarna upp till höger och välja redigera i yaml. Klistra in innehållet som finns i filen admin_vy.yaml

### Steg 8
Starta om Home Assistant 

### Steg 9
Klicka in på din nya vy och starta konfigurationen genom att klicka på Inställningar

> [!NOTE]
> Om ett kort inte fungerar beror det troligtvis på att fel enhet/enheter används. Justera korten vid behov. 

## Uppdateringar :loudspeaker:
Detta är ingen integration och därför kommer inga uppdateringar automatiskt till Home Assitant. För att få information om en ny realse är det lättast att "följa" min repo. För att uppdatera din kod gör du om steg 6 och startar om Home Assistant. I varje realse står det vilka nya funktioner som finns, men även vilka uppdateringar som gjort och om några ändringar behövs göras. 

## Framtida funktioner :raising_hand:
Önska gärna nya funktioner här på Github under discussion. 

## Problem :bangbang:
Upptäcker du något problem är jag tacksam om du rapporterar det här på Github under issues.
