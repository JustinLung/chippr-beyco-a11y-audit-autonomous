# Rapportage webtoegankelijkheid-test voor Beyco Coffee Page

![Beyco Visual](https://media.discordapp.net/attachments/871761581590052925/905394941168078888/mockup_beyco.png?width=1428&height=1138)

Dit document is een webtoegankelijkheid-test volgens de Web Content Accessibility Guidelines (WCAG). Een consistente rapportage helpt bij het uitvoeren van een evaluatie en zorgt er voor dat verschillende tests kunnen worden vergeleken.

Datum webtoegankelijkheid-test:
27 oktober 2021
28 oktober 2021
1 november 2021
2 november 2021

Webtoegankelijkheid-test uitgevoerd door: Justin Lung

## Inhoudsopgave

- [Samenvatting](#samenvatting)
- [Achtergrond bij de evaluatie](#achtergrond_evaluatie)
- [Afbakening](#afbakening)
- [Testresultaten en aanbevelingen](#testresultaten_aanbevelingen)
- [Referenties](#referenties)
- [Bijlagen](#bijlagen)
- [Licentie](#licentie)

## Samenvatting

Dit rapport beschrijft in hoeverre de website Beyco (Coffee pagina)overeenstemt met de Web Content Accessibility Guidelines (WCAG) van het W3C. Na de achtergrondinformatie en afbakening van de test worden beoordelaars, beoordelingsproces en testresulltaten beschreven.

Conslusie van deze test luidt dat de Beyco (Coffee pagina) website voldoet de WCAG 2.1, op niveau AA. Gedetailleerde resultaten en aanbevelingen zijn verderop in dit document beschikbaar en in de referenties vindt u bronnen voor eventuele vervolgstudie. Wij stellen feedback op deze evaluatie zeer op prijs.

## Achtergrond bij de evaluatie

De webtoegankelijkheid-test vereist een combinatie van semi-geautomatiseerde en handmatig uitgevoerde evaluatie tools door een ervaren beoordelaar. De beoordelingsresultaten in dit rapport zijn gebaseerd op een beoordeling welke is uitgevoerd op 28 oktober 2021. De website kan ondertussen aangepast zijn.

## Afbakening

**Naam website:** Beyco
**Doel website:**
Beyco “Beyond Coffee” is een wereldwijd koffie handelsplatform dat kopers en producenten met elkaar in contact brengt. Op dit online platform kunnen producenten hun koffie online verkopen en kunnen kopers koffie vinden die ze zoeken. Daarnaast kun je ook ‘trader’ zijn, iemand die zowel koopt als verkoopt.

De website wordt veel gebruikt in landen zoals Peru. Hier is vaak een slechte internetverbinding en ook heel erg veel zonlicht, daarom is het de bedoeling dat de website goed werkt voor deze gebruikers.

**URL Website die wordt getest:**
https://beyco.nl/trade/offers/public

## Beoordelaars

**Naam beoordelaars**: Daan Korver, Justin Lung, Daphne Zwuup, Chaan Soekana, Finn van Bekkum, Armadno Jubitana

## Beoordelingsproces

Het WCAG 2.1 niveau waarop getest is, is niveau AA.

**Tools gebruikt:**

- Screenreader van Apple Macbook
- Visual Studio Code
- Google Chrome
- Lighthouse

**Beoordeling uitgevoerd:**

- A11Y Project-Checklist
- Lighthouse

## Testresultaten en aanbevelingen

De accessibility op desktop, heeft een score van 76. Dit kan echter nog verbeterd worden doormiddel van de volgende punten:

- Buttons hebben geen accesible name. Bij de hamburger menu, is er een button tag aangeroepen, maar zit er geen text in. Om dit op te lossen kan je in die button tekst in zetten. Ook kun je een aria-label gebruiken om dit op te lossen.
- Image elementen hebben geen alt attributes. Dit is dus niet goed voor de toegankelijkheid.
- Links hebben geen geldige benaming. Dit houdt in dat er in de a tag geen content bevat.
- De contrast ratio van de pagina, is niet toegankelijk voor de website.

Dezelfde bevindingen zijn op de mobiele telefoon te zien en heeft ook een accessibility score van 76.

**Internet**
Wij hebben de website ook op langzaam internet getest. Hierbij is het resultaat dat de website volledig geladen is binnen 29.06 seconden. Dit kan waarschijnlijk versneld worden door images verder te compressen en je kan de style verder minifien.

### Sterke punten

### Ontoegankelijke punten

Na het invoeren van een input veld, krijg je een error message te zien. Deze error message wordt alleen met tekst aangeduid. Dit kan worden verbeterd doormiddel van kleur (Een rooie kleur zou goed zijn om aan te duiden dat er geen zoekresultaten zijn). Hierdoor verbeterd de accessibility voor mensen met een beperking ook.

### Checklist

#### Forms

- **All inputs in a form are associated with a corresponding label element.**
  Alle inputs in een form, worden geassocieerd met een label element. Echter kan het nog verbeterd worden om de input types bij een label een for/id te geven zodat de hoogste technologie van een browser het wordt support.
- **Use fieldset and legend elements where appropriate.**
  Er worden goed gebruik gemaakt van fieldsets & legends.
- **Inputs use autocomplete where appropriate.**
  Er wordt gebruikt gemaakt van een autocomplete bij een input waarbij nodig is.
- **Make sure that form input errors are displayed in list above the form after submission.**
  Er wordt gebruikt gemaakt van error handling. Als er geen zoekresultaten zijn, wordt dit duidelijk in tekst aangeduid dat er geen zoekresultaten zijn na het invullen van de input.
- **Associate input error messaging with the input it corresponds to.**
  Er wordt geen gebruik gemaakt van een aria-describedby om de inputs te laten associeren.
- **Make sure that error, warning, and success states are not visually communicated by just color.**
  Bij een error message, wordt het alleen met tekst aangeduid. Dit kan worden verbeterd doormiddel van kleur (Een rooie kleur zou goed zijn om aan te duiden dat er geen zoekresultaten zijn).

#### Media

- n.v.t

#### Video

- n.v.t

#### Audio

- n.v.t

#### Appearance

- **Check your content in specialized browsing modes.**
  Wanneer je tools zoals Window High Contrast/Inverted Colors gebruikt, dan is de website nog steeds goed zichtbaar.
- **Increase text size to 200%.**
  Tekst is goed te lezen na het inzoomen naar 200%
- **Double-check that good proximity between content is maintained.**
  De content kan nog worden gelezen als mensen een screen zoom software gebruiken. Dit werd getest met behulp van de [strawtest](https://www.youtube.com/watch?v=S1j6CYT3kWA)
- **Make sure color isn't the only way information is conveyed.**
  Links kunnen nog steeds gelezen worden na het gebruiken van een grayscale filter.
- **Make sure instructions are not visual or audio-only.**
  Er wordt geen audio gebruikt om instructies aan te duiden.
- **Use a simple, straightforward, and consistent layout.**
  De pagina heeft een logische layout verdeling

#### Animation

- **Ensure animations are subtle and do not flash too much.**
  Animaties zijn niet te "flashy". Ze worden subtiel afgespeeld.
- **Provide a mechanism to pause background video.**
  n.v.t
- **Make sure all animation obeys the prefers-reduced-motion media query.**
  Animaties worden niet in een prefers-reduced-motion media query gebruikt.

#### Color contrast

- **Check the contrast for all normal-sized text.**
  De contrast ratio van een normnal sized text (zwarte #000000 op #FEFFFE ) is 20.9:1.
  
  Het contrast is dus nu enhanced naar een AAA resultaat. Normal-sized text is dus goed leesbaar op de pagina.

- **Check the contrast for all large-sized text.**
  De contrast ratio van large sized text (zwarte #000000 op #FEFFFE ) zijn 20.6.1.
  
  Het contrast is dus nu enhanced naar een AAA resultaat. large-sized text is dus goed leesbaar op de pagina.

- **Check the contrast for all icons.**
  
  Search Icon: grijs (#C6C8CA) op wit (#FEFFFE) heeft een contrast ratio van 1.7:1. Dit is dus niet goed zichtbaar.
  
  Dropdown icon: zwart (#000000) op wit (#FEFFFE) heeft een contrast ratio van 20.9:1. Dit is dus goed zichtbaar. 

  Icon man: zwart (#000000) op grijs (#F5F7F9) heeft een contrast ratio van 19.6:1. Dit is dus goed zichtbaar.

  Page identifier: grijs (#8B8C8B) op wit (#FEFFFE) heeft een contrast ratio van 3.4:1. Dit is dus niet goed zichtbaar.

  Dropdown (port/export) icon: grijs (#CDCECD) op wit (#FEFFFE) heeft een contrast ratio van 1.6:1. Dit is dus niet goed zichtbaar. 

- **Check the contrast of borders for input elements (text input, radio buttons, checkboxes, etc.).**
  Text Input: Contrast ratio voor de inputs is een 1.3:1. Dit betekent dus dat de contrast niet helemaal lekker loopt.
  Radio Button (after click state): De contrast van de UI component is een 4.5:1. De contrast is dus hierbij goed.
  Radio Button (before click state): De contrast van de UI component is een 1.2:1. De contrast is dus niet heel goed.
  Green CTA: De contrast ratio is een 4.5:1. Het voldoet aan de AA resultaat
  White CTA with green text: De contrast ratio is een 4.5:1. Het voldoet aan de AA resultaat
- **Check text that overlaps images or video.**
  n.v.t
- **Check custom ::selection colors.**
  n.v.t

#### Mobile and touch

- **Check that the site can be rotated to any orientation.**
  De website kan goed geroteerd worden. Echter zijn er een aantal dingetjes die ik heb opgemerkt. Bij een koffie product, dit is een design keuze, maar de thumbnail van het product wordt niet laten zien en ziet de layout er niet goed uit.

  ![Beyco Layout](https://cdn.discordapp.com/attachments/871761581590052925/904679116270350336/test.beyco.chippr.dev_trade_offers_publiciPhone_6_7_8_1.png)

- **Remove horizontal scrolling.**
  Er is geen sprake van horizontal scrolling.
- **Ensure that button and link icons can be activated with ease.**
  Buttons en link iconen zijn goed klikbaar.
- **Ensure sufficient space between interactive items in order to provide a scroll area.**
  Er is genoeg ruimte om te scrollen voor mobiel.

## Referenties

Referenties welke gebruikt zijn bij de webtoegankelijkheid-test. Deze referenties zijn allen in het Engels:

- https://www.a11yproject.com/checklist/
- https://www.w3.org/TR/WCAG21/

## Bijlagen

**Lighthouse desktop**

![lighthouse_desktop](https://cdn.discordapp.com/attachments/871761581590052925/904682711380283392/Screenshot_2021-11-01_at_11.46.00.png)

**Lighthouse Mobile**

![lighthouse_mobile](https://media.discordapp.net/attachments/871761581590052925/904683362021679154/Screenshot_2021-11-01_at_11.48.36.png)

**Internet slow 3G**

![network_tab](https://media.discordapp.net/attachments/871761581590052925/905027420841734154/Screenshot_2021-11-02_at_09.39.41.png?width=1420&height=1137)

## Licentie

![GNU GPL V3](https://www.gnu.org/graphics/gplv3-127x51.png)

This work is licensed under [GNU GPLv3](./LICENSE).
