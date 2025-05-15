# Loxone Demo Koffer

Deze `README.md` beschrijft het Loxone Demo Koffer project waarin data van verschillende Loxone-sensoren wordt ontvangen via UDP en gevisualiseerd in de Loxone App. Dit project maakt gebruik van zowel Air- als Tree-technologie van Loxone. Het biedt een praktische demonstratie van de mogelijkheden van het Loxone systeem binnen een portable koffer.

## Inhoudsopgave

- [Overzicht](#overzicht)
- [Hardwarecomponenten](#hardwarecomponenten)
- [Gebruikte Loxone-componenten](#gebruikte-loxone-componenten)
- [Netwerkcommunicatie (UDP)](#netwerkcommunicatie-udp)
- [Integratie met Loxone Config & App](#integratie-met-loxone-config--app)
- [Opbouw van de GitHub-repo](#opbouw-van-de-github-repo)
- [Installatie en Setup](#installatie-en-setup)
- [Toekomstige uitbreidingen](#toekomstige-uitbreidingen)
- [Bronnen](#bronnen)

---

## Overzicht

De Loxone Demo Koffer is ontworpen als een educatieve en demonstratieve tool waarmee gebruikers kunnen leren werken met de Loxone Miniserver, Air & Tree Extension, en verschillende sensoren. De sensordata wordt via UDP ontvangen en live verwerkt om weergegeven te worden in de Loxone App. Dit biedt inzicht in automatiseringsprocessen en data-integratie met het Loxone-systeem.

## Hardwarecomponenten

- Loxone Miniserver (Gen 1 of 2)
- Loxone Air Base Extension
- Loxone Tree Extension
- Loxone Weather Station
- Loxone Comfort Sensor (binnenklimaat)
- Loxone Drukventielen
- Power supply module
- UDP-sensor controller (extern of ingebouwd)
- Netwerkrouter of -switch
- Behuizing: robuuste koffer met interne bedrading

## Gebruikte Loxone-componenten

### Weather Station

- Biedt real-time gegevens over wind, regen, temperatuur, helderheid en luchtvochtigheid.
- Wordt gekoppeld via Air-technologie en stuurt regelmatig data door naar de Miniserver.

### Comfort Sensor Air

- Meet temperatuur, luchtvochtigheid en CO2-niveaus binnen.
- Kan ook als bewegingssensor fungeren.
- Maakt gebruik van de Air Base Extension.

### Drukventielen

- Worden gebruikt voor demonstraties met lucht- of waterdruk.
- Worden via digitale uitgangen van de Miniserver aangestuurd.

## Netwerkcommunicatie (UDP)

In dit project worden externe sensoren of microcontrollers gebruikt die data verzenden via het UDP-protocol naar het netwerk waarop de Miniserver zich bevindt.

### UDP Ontvangen in Loxone:

- In Loxone Config wordt een virtuele UDP-ingang aangemaakt.
- Het formaat van het bericht moet overeenkomen met de geconfigureerde parser.
- Voorbeeld van een UDP-pakket: `T=21.5;H=45.2;CO2=380`
- Met virtuele ingangen en String-parsing worden waarden automatisch geüpdatet in de visualisatie.

## Integratie met Loxone Config & App

- In Loxone Config worden alle apparaten toegevoegd via de Air of Tree Extensions.
- De ontvangen UDP-data wordt via virtuele ingangen in blokken (zoals de statusdisplay, analog monitor, etc.) gekoppeld.
- Deze informatie wordt dan zichtbaar in de Loxone App onder het tabblad "Sensoren" of in aangepaste dashboards.

## Opbouw van de GitHub-repo

GitHub-repo: [PXLDigital/Loxone-Mini-Server](https://github.com/PXLDigital/Loxone-Mini-Server)

### Belangrijke folders:

- `/docs`: bevat documentatie over het project en demonstraties.
- `/udp_receiver`: voorbeeldcode voor een UDP-server in Python of C++.
- `/loxone_config_exports`: voorbeelden van .LoxConfig bestanden of exports van Loxone Config.
- `/images`: foto's of schema’s van de opstelling en de interne bedrading van de koffer.

## Installatie en Setup

1. Voeding aansluiten op Miniserver en Extensions.
2. Apparaten koppelen:
   - Start de koppelmodus in Loxone Config.
   - Voeg het weerstation, comfort sensor en drukventielen toe.
3. UDP-configuratie:
   - Zet een virtueel UDP-apparaat op met de juiste poort en parsing regels.
4. App layout bouwen:
   - Voeg visualisatieblokken toe in Loxone Config.
   - Synchroniseer met de Miniserver.

## Toekomstige uitbreidingen

- Logging en opslag van sensordata in een extern systeem (bijv. InfluxDB + Grafana).
- Toevoegen van MQTT naast UDP voor bredere integratie.
- Integratie met Home Assistant voor uitgebreide automatisering.
- Live grafieken van temperatuur en CO2 in de app.
- Toevoegen van geluidssignalen (buzzers) of verlichting (LED-strips) voor visuele/auditieve feedback.
- Maken van een instructievideo voor gebruikers van de demo koffer.

## Bronnen

- [Loxone Air Base Extension](https://www.loxone.com/enen/kb/air-base-extension/)
- [Loxone Tree Extension](https://www.loxone.com/enen/kb/tree-extension/)
- [Loxone Weather Station](https://www.loxone.com/enen/kb/weather-station/)
- [Loxone Comfort Sensor](https://www.loxone.com/enen/kb/comfort-sensor-air/)
- [Officiële Loxone Config handleiding](https://www.loxone.com/enen/kb/loxone-config/)

---

Voor vragen of feedback, maak een issue aan op de GitHub-repo of contacteer het team van [PXL Digital](https://pxl.be/digital).
