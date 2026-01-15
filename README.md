## Smart energihantering
HACS-paket för Home Assistant som optimerar din Huawei-batteriinstallation och solpaneler.
Styr laddningen automatiskt baserat på elpriser, batteriets status och solprognos för att maximera egenanvändningen.
Paketet gör även följande:

- Begränsar solelexport vid negativa elpriser
- Förhindrar att din elbil laddas från hemmabatteriet
- Säljer batteriöverskott när det är ekonomiskt lönsamt
- Laddar smart för att inte slita på batteriet och med fokus på självförsörning.
<img width="1669" height="881" alt="Skärmbild 2026-01-13 220103" src="https://github.com/user-attachments/assets/1365676f-2878-469f-b8ea-fea4e2c04f27" />


## Installation
### Steg 1
a) Installera och konfigurera [Huawei Solar Integrationen](https://github.com/wlcrs/huawei_solar)

b) Installera och konfigurera [SMHI Integrationen](https://www.home-assistant.io/integrations/smhi/)
Lägg till din plats och namnge din nya sensor med home (vilket ger följande enhetsnamn weather.smhi_home) 

c) Installera och konfiguera [Nordpool Integrationen](https://www.home-assistant.io/integrations/nordpool/). Paketet fungerar även med Nordpool Integrationen från HACS. [Nordpool HACS Integrationen](https://github.com/custom-components/nordpool)

### Steg 2
Installera följande från HACS:

- Apexcharts-card
- Layout-card
- Vertical-stack-in-card
- Energy-flow-card-plus
- Bubble-card

Har du inte HACS?
Följ instruktionerna [här](https://www.hacs.xyz/docs/use/configuration/basic/)

### Steg 3
Lägg till följande rad i din configuration.yaml

```yml
homeassistant:
  packages: !include_dir_named packages
```


> [!IMPORTANT]
> Observera indraget och att det ska vara placerad direkt under Home Assistant som ska ligga högst upp i din fil. 

> [!NOTE]
> Ladda ner file editor (tillägg) för att kunna redigera din configuration.yaml på ett enkelt sätt. Detta gör du via inställningar (kugghjulet till vänster), välj sen tillägg. Klicka på tilläggsbutik och sök (högst upp) efter file editor. Installera och starta sen file editor genom att klicka på öppna webbgränsnitt.
>
> https://www.home-assistant.io/addons/

> [!WARNING]
> Om packges inte ligger direkt under homeassistant och högst upp i din fil kommer du inte kunna ladda ner paketet.

<img width="1028" height="588" alt="Skärmbild 2025-10-27 092254" src="https://github.com/user-attachments/assets/b1f80a61-6d04-44c1-9654-c9106dc91ac0" />
<img width="439" height="86" alt="Skärmbild 2025-10-27 092414" src="https://github.com/user-attachments/assets/d40c3051-d78c-4681-8ec6-17749f93876a" />


### Steg 4
Skapa en mapp på samma plats som din configuration.yaml-fil och namnge den packages.
<img width="874" height="233" alt="Skärmbild 2025-10-27 092730" src="https://github.com/user-attachments/assets/585a1d74-9e17-4c5e-a527-0015f89531fb" />

Klicka på mappen för att komma till dina filer

<img width="333" height="133" alt="Skärmbild 2025-10-27 093712" src="https://github.com/user-attachments/assets/b9b0601c-cbbc-4d23-8273-18efc1e1fa96" />

Klicka på mappen med ett plus och skriv in packages.

### Steg 5
a) Leta upp din nya mapp (packages) i listan och gå in i den. Skapa en ny mapp som du ger namnet sem (samma princip som i steg 5)

b) Ladda ner och packa upp innehållet från github på din dator. Klicka på länken nedan för att ladda ner innehållet.  

https://github.com/Henrik1986/huawei-energy-managment/archive/fb39a1732d69ab12b96c7f657dad6f1d15df60d1.zip

c) Ladda upp innehållet som ligger i mappen sem (från din dator) till mappen sem på din home assistant. 

<img width="335" height="129" alt="Skärmbild 2025-10-27 093414" src="https://github.com/user-attachments/assets/50f36441-a096-4e2b-8d76-980f5de2007e" />

Viktigt att du är inne i mappen sem. 

### Steg 6
Starta om Home Assistant

### Steg 7
Skapa en ny vy i Home Assistant genom att klicka på pennikonen uppe till höger och sedan på plus-tecknet (+).
I dialogrutan som visas, klicka på de tre prickarna uppe till höger och välj Redigera i YAML.
Klistra sedan in innehållet från filen admin_vy.yaml här på Github. 


<img width="609" height="239" alt="Skärmbild 2025-12-21 224942" src="https://github.com/user-attachments/assets/954997c3-f65c-4fa4-a1ed-dce91a6f4095" />
<img width="946" height="106" alt="Skärmbild 2025-12-21 225127" src="https://github.com/user-attachments/assets/2113db8a-2c80-4374-a1c5-4cbde00cb6d4" />
<img width="588" height="343" alt="Skärmbild 2025-12-21 225204" src="https://github.com/user-attachments/assets/5e418d88-b45a-4a5d-9853-e75646df4a3a" />
<img width="603" height="256" alt="Skärmbild 2025-12-21 225248" src="https://github.com/user-attachments/assets/df695c43-6bd4-4a42-afd7-c98dda0d40cc" />

### Steg 8
Nu ska du fått en ny vy där du har en överblick över ditt system. Klickar du på knappen "Mitt system" kan du köpa användarkod, konfiguerar systemet samt uppdatera systemet när ny version släpps. Du ser även vilken version som är den senaste och vilken du har installerad. 


> [!NOTE]
> För att få full funktionallitet behöver du en nyckel. Det finns nycklar som ger dig tillgång till systemet i 30 dagar. Därefter kostar en användarkod 399 kr/år. 

> [!NOTE]
> Om något kort inte fungerar som det ska beror det troligtvis på att fel enhet är inställd. 

## Uppdateringar :loudspeaker:
Via denna sida kommer du kunna läsa om nya funktioner som lagt till vid varje realese. Där kommer det framgå om du behöver tänka på något innan du uppdaterar paketet. 

> [!NOTE]
> För att nya funktioner ska bli tillgängliga hos dig krävs en omstart av Home Assistant. 

## Framtida funktioner :raising_hand:
Har du idéer på nya funktioner? Lämna gärna dina förslag på GitHub under ”Discussions”.

## Problem :bug:
Upptäcker du något problem? Rapportera det gärna på GitHub under ”Issues”.

## Stötta mitt arbete 🚀
Ditt stöd gör det möjligt för mig att fortsätta förbättra paketet, optimera funktioner och lägga till nya smarta funktioner i framtiden. Prova systemet gratis året ut. Därefter kostar systemet 399 kr/år. 

<a href="https://www.buymeacoffee.com/henrikakere" target="https://buymeacoffee.com/henrikakere"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
