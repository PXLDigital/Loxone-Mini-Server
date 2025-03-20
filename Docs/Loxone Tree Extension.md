# Loxone Tree Extension

De Loxone Tree Extension is een uitbreidingsmodule die de Loxone Miniserver in staat stelt om te communiceren via het Tree-bus systeem. Deze technologie maakt het mogelijk om apparaten aan te sluiten die via een gedecentraliseerd netwerk werken, wat ideaal is voor grotere systemen met veel apparaten.

## Inhoudsopgave

- [Installatie](#installatie)
- [Aansluitingen](#aansluitingen)
- [Configuratie in Loxone Config](#configuratie-in-loxone-config)
- [Apparaten koppelen](#apparaten-koppelen)
- [Gebruik en extra functies](#gebruik-en-extra-functies)

## Installatie

1. **Montage**:
   - De Tree Extension moet op een geschikte plaats in de schakelkast worden gemonteerd.
   - Zorg ervoor dat de module niet wordt blootgesteld aan extreme temperaturen of vochtigheid.
2. **Voeding**:
   - De Tree Extension heeft een 24V DC voeding nodig. Gebruik een geschikte stroombron die de benodigde spanning levert.

## Aansluitingen

| Klem | Functie |
|------|---------|
| 24V  | Voeding (24V DC) |
| GND  | Massa |
| Tree | Tree-bus communicatiepoort |

- Verbind de Tree Extension met de Tree-bus van de Miniserver.
- Zorg ervoor dat de bedrading correct is aangesloten om storingen te voorkomen.

## Configuratie in Loxone Config

1. Open **Loxone Config** en selecteer de Miniserver waarop de Tree Extension is aangesloten.
2. Klik op "Tree-apparaat zoeken" en start het koppelproces.
3. De Tree Extension zal automatisch worden gedetecteerd.
4. Wijs een naam en locatie toe aan het apparaat in Loxone Config.
5. Sla de wijzigingen op en stuur de configuratie naar de Miniserver.

## Apparaten koppelen

1. **Koppelmodus activeren**:
   - Bij het aansluiten van de Tree Extension zal de koppelmodus automatisch geactiveerd worden.
   - Voor het toevoegen van een nieuw apparaat: sluit het apparaat aan op de Tree-bus en volg de koppelinstructies.
2. **Koppelen via Loxone Config**:
   - Zoek het apparaat dat je wilt koppelen en voeg het toe aan het systeem.
   - Configureer de parameters van het apparaat, zoals naam, locatie en specifieke instellingen.
3. **Opslaan en testen**:
   - Sla de configuratie op en test de communicatie met de nieuwe apparaten via de Loxone App of Config.

## Gebruik en extra functies

- **Draadloze en bedrade communicatie**: De Tree Extension ondersteunt zowel draadloze als bedrade verbindingen, afhankelijk van het type aangesloten apparaat.
- **Uitbreidingsmogelijkheden**: Met de Tree Extension kunnen meer apparaten aan het Loxone-systeem worden toegevoegd via de Tree-bus, wat ideaal is voor grote installaties.
- **Koppeling met andere Loxone-producten**: De Tree Extension is volledig compatibel met andere Loxone-apparaten en maakt integratie eenvoudiger.

Meer details: [Loxone Tree Extension](https://www.loxone.com/enen/kb/tree-extension/)
