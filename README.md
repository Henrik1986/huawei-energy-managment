## Smart energihantering

Ett kraftfullt HACS-paket för Home Assistant som optimerar din energianläggning med solceller och batteri – helt automatiskt. Systemet analyserar elpriser, batteriets status och solprognoser i realtid för att maximera egenanvändning och lönsamhet, utan manuell styrning.

Funktioner:
- Optimerar laddning och urladdning baserat på elpris, solprognos och behov
- Säljer överskottsel när det är som mest lönsamt
- Laddar batteriet när elen är billig – med hänsyn till batteriets livslängd
- Begränsar export vid negativa elpriser
- Förhindrar att elbilen laddas från batteriet
- Stöd för AI-analys som förbättrar styrning och beslut över tid
- Stöd för att styra laddningen av elbilar

Designat för att ge högre självförsörjning, bättre ekonomi och full kontroll över din energianläggning.


<img width="1573" height="877" alt="Skärmbild 2026-06-16 211824" src="https://github.com/user-attachments/assets/3ad851a5-e7d3-47ec-b99c-bde30b7b985d" />
Bilden ovan visar systemets dashboard



## Installation 🛠️

SEM installeras via **HACS (Home Assistant Community Store)** som ett custom repository.

### 1. Lägg till SEM i HACS

Öppna **HACS** i Home Assistant och gå till **Integrations**.

1. Klicka på menyn med **tre punkter (⋮)** uppe till höger.

2. Välj **Custom repositories**.

3. Klistra in följande adress i fältet för repository:

   `https://github.com/Henrik1986/sem-energy-manager`

4. Välj **Integration** som kategori.

5. Klicka på **Add**.

SEM finns nu tillgängligt i HACS och kan installeras därifrån.

### 2. Installera SEM

Sök efter **SEM Energy Manager** i HACS och klicka på **Download**.

När installationen av integrationen är klar behöver du starta om Home Assistant. Därefter visas SEM som en integration i Home Assistant. 

Videoklipp hur du laddar ner SEM från HACS - [Klicka här](https://drive.google.com/file/d/1lD3Xn5wkz_DDYr9zARwxn4JH-MZ9uwGO/view?usp=sharing)

### 3. Följ installationsguiden

SEM är utformad för att göra installationen så enkel som möjligt. När integrationen laddats ner kan du startar en **installationsguide (wizard)** som steg för steg hjälper dig att konfigurera systemet och visar vilka komponenter och inställningar som behöver finnas på plats.

Installationen görs bäst på en **dator**. Genom att ha Home Assistant och installationsguiden öppna i två fönster bredvid varandra blir det enklare att följa instruktionerna och samtidigt göra de inställningar som krävs.

Videoklipp som visar hur du startar installationsguiden - [Klicka här](https://drive.google.com/file/d/1Pn8AXn_xB9325W0WqvzVwqpP2utj2Kdc/view?usp=sharing)

### 4. Konfigurera och uppdatera SEM

När installationen är klar behöver du normalt inte arbeta direkt med konfigurationsfiler. **Inställningar, justeringar och framtida uppdateringar av systemet hanteras direkt från SEM:s egen sida i Home Assistants sidofält.**

Det gör att SEM kan konfigureras och anpassas direkt från Home Assistants gränssnitt utan att du behöver redigera YAML-filer manuellt.


## Saknar du stöd för ditt system? 💬
Vill du göra din anläggning kompatibel är du välkommen att öppna en diskussion på GitHub eller kontakta mig, så tittar vi på möjligheterna att lägga till stöd.

## Uppdateringar :loudspeaker:
Via denna sida kommer du kunna läsa om nya funktioner som lagt till vid varje realese. Där kommer det framgå om du behöver tänka på något innan du uppdaterar paketet. 

> [!NOTE]
> För att nya funktioner ska bli tillgängliga hos dig krävs en omstart av Home Assistant.



## Framtida funktioner :raising_hand:
Har du idéer på nya funktioner? Lämna gärna dina förslag på GitHub under ”Discussions”.

## Problem :bug:
Upptäcker du något problem? Rapportera det gärna på GitHub under ”Issues”.

## Stötta mitt arbete 🚀
Ditt stöd gör det möjligt för mig att fortsätta förbättra paketet, optimera funktioner och lägga till nya smarta funktioner i framtiden. 

<a href="https://www.buymeacoffee.com/henrikakere" target="https://buymeacoffee.com/henrikakere"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
