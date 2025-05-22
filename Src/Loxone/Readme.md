# LoxoneBoys House - Smart Home Project

Dit project beschrijft een geautomatiseerde woningconfiguratie ontwikkeld in **Loxone Config**. Het doel van dit project is om een reeks domoticafuncties te implementeren zoals beveiliging, handmatige ventielbediening, en datavisualisatie via een netwerkverbinding.

## 🔧 Functies

### 1. Alarmsysteem

Een alarmsysteem dat wordt geactiveerd op basis van:

- **Raambreuksensor**  
- **Aanwezigheidssensor**

Bij detectie van een indringer of breuk wordt het alarm geactiveerd en kunnen bijkomende acties worden ondernomen, zoals het versturen van meldingen of het activeren van lichten/sirenes.

### 2. Handmatige Ventielregeling

- Er zijn **drie afzonderlijke ventielen** geïnstalleerd.
- Elk ventiel kan handmatig geopend of gesloten worden met behulp van een **potentiometer**.
- Deze functie is nuttig voor HVAC-demonstraties of irrigatiesystemen.

### 3. UDP Connectie en Datavisualisatie

- Er is een **UDP-netwerkverbinding** opgezet.
- De Miniserver ontvangt externe data via het netwerk, zoals:
  - Temperatuur (landbouwtoepassingen)
  - Luchtvochtigheid
  - Bodemvochtigheid
- Deze waarden worden weergegeven in de **Loxone App** via virtuele ingangen en kunnen worden gelogd of geanalyseerd.

## 📦 Gebruikte Hardware

- **Loxone Miniserver**
- **Potentiometers** (voor ventielregeling)
- **Aanwezigheidssensoren** (bewegingsdetectie)
- **Raambreuksensor**
- **Drukventielen**
- **Netwerkmodule** voor UDP-communicatie

## 🖥️ Visualisatie in de Loxone App

- Overzicht van actuele sensordata (temperatuur, vochtigheid)
- Status van ventielen en handmatige regeling
- Alarmmeldingen en visuele statusweergave

## 🚀 Installatie

1. Open het `.Loxone` bestand in **Loxone Config**.
2. Verbind de Miniserver via het lokale netwerk.
3. Stel de UDP-ontvangst correct in (IP & poort).
4. Upload de configuratie naar de Miniserver.
5. Verbind de Loxone App en test alle modules.

## 📈 Mogelijke uitbreidingen

- Logging van sensordata naar externe databases (InfluxDB, CSV)
- Integratie met weerstations of cloud-API’s
- Extra sensoren voor CO₂, lichtintensiteit, enz.
- Automatische ventilatie of irrigatie op basis van de ontvangen data

## 📚 Bronnen

- [Loxone Config documentatie](https://www.loxone.com/enen/kb/loxone-config/)
- [Virtuele ingangen & UDP communicatie](https://www.loxone.com/enen/kb/virtual-input-udp/)

---

Voor technische ondersteuning of vragen, gelieve contact op te nemen met het projectteam of via de officiële Loxone community.

