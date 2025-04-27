# Cali-Can Project

**Ein ESPHome-Projekt zur CAN-Bus Integration im VW Grand California**+

basierend auf [VWGC-CanBus](https://github.com/mk4001/VWGC-CanBus.git) habe ich eine Abwandlung für ESP-Home erstellt. 
Großer Dank an [MK4001](https://github.com/mk4001), dank seiner vorarbeit habe ich mir viel Can-Sniffing erspart =)
 

---
## DISCLAIMER
mit diesem Projekt wird in die Fahrzeugelektronik eingegriffen. Ich übernehme keine Haftung für eventuell auftretende Schäden!

---

## 🚶‍♂️ Ziel des Projekts

Dieses Projekt liest ausgewählte CAN-Bus-Daten aus dem VW Grand California aus und ermöglicht folgende Funktionen:

- Anzeige von **Frischwasserstand** und **Grauwasserstand**
- Erkennung, ob das **Fahrzeug verriegelt** ist
- Steuerung:
  - **Innenbeleuchtung** ein-/ausschalten
  - **Außenbeleuchtung** ein-/ausschalten
  - **Trittstufe ein- und ausfahren**
  - **Auto-Modus der Trittstufe toggeln**
  - **Camping-Mode toggeln**

Alles über einen einzigen ESP32 mit CAN-Transceiver und Integration in **Home Assistant**.

---

## 🛠️ Benötigte Hardware

- ESP32 Dev Board (z.B. **ESP32 DevKit v1**)
- CAN-Bus Transceiver Modul (z.B. **SN65HVD230**, **TJA1050**, oder ähnliche)
- Verbindung zum Fahrzeug-CAN (z.B. am Steuergerät / OBD-Stecker oder direkt an passenden Leitungen)

**Achtung:**
- CAN-H (High) und CAN-L (Low) korrekt anschließen
- Abschlusswiderstand (120 Ohm) je nach Einbausituation beachten

---

## 🌐 Software-Setup

- Installiere ESPHome
- Flashe das beiliegende `cali-can.yaml` auf dein ESP32 Board
- Konfiguriere dein WLAN in den `!secret`-Werten oder direkt im YAML
- Füge das Gerät über die ESPHome-Integration in Home Assistant hinzu


---

## 🔄 Erweiterungsmöglichkeiten (Ideen für die Zukunft)

- **Status-Rückmeldungen** für Campingmode und Trittstufe und Licht
- **Feinere Steuerung** der Lichtfunktionen


---

## 📆 Aktueller Stand

Dieses Projekt ist ein **Work in Progress**.
Gemeinsam können wir es stetig verbessern – gerne Pull Requests einreichen oder Issues eröffnen!


---

# Viel Spaß beim Nachbauen! 🌟

