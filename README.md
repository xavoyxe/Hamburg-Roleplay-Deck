[![Hamburg Roleplay Deck Banner](https://raw.githubusercontent.com/xavoyxe/Hamburg-Roleplay-Deck/main/assets/banner.png)](https://discord.gg/bBMDRYTwbn)

# 🏙️ Hamburg Roleplay Deck

**Hamburg Roleplay Deck** ist das zentrale Repo für den **Hamburg Roleplay Bot** — ein persönlicher Discord-Bot (Python, v3.10) mit Slash- und Prefix-Befehlen zur Verwaltung von Ausweisen, Reports und Community-Interaktionen.

---

## 🔎 Kurzbeschreibung
Der Bot bietet sowohl Slash-Commands (`/`) als auch klassische Prefix-Commands (`!`). Er ist ein persönlicher Bot für Roleplay-Zwecke und unterstützt Funktionen wie das Erstellen / Löschen / Anzeigen von Ausweisen (inkl. Modal UI für Eingaben) sowie das Senden von Bugreports.

---

## 🧭 Befehlsübersicht

### `/ausweis-erstellen`
**Beschreibung:** Erstelle einen normalen oder gefälschten Ausweis.  
**Verhalten:** Öffnet ein Modal (eingabefeldähnliche UI), in dem Informationen wie Name, Alter, Beruf, Stadt etc. eingetragen werden. Nach Bestätigung wird der Ausweis erstellt und dem Nutzer zugeordnet.  
**Beispiel:** `/ausweis-erstellen` → Modal mit Feldern → Bestätigen → Ausweis gespeichert

### `/ausweis-löschen`
**Beschreibung:** Lösche deinen eigenen Ausweis.  
**Verhalten:** Löscht den im System hinterlegten Ausweis des Nutzers. Optional mit Sicherheitsabfrage/Confirm.  
**Beispiel:** `/ausweis-löschen` → Bestätigungs-Prompt → Ausweis gelöscht

### `/ausweis-ansehen`
**Beschreibung:** Zeige deinen Ausweis oder den Ausweis eines anderen Nutzers an.  
**Verhalten:** Zeigt den formatierten Ausweis an. Optional: Freigabe-/Privacy-System — der angezeigte Ausweis kann nur bei Zustimmung des Besitzers eingesehen werden.  
**Beispiel:** `/ausweis-ansehen @Spieler` → Zeigt Ausweis, falls freigegeben

### `/report`
**Beschreibung:** Sende einen Bug- oder Fehlerreport an das Team.  
**Verhalten:** Öffnet ein kurzes Modal oder nimmt Argumente entgegen. Sendet Report an konfigurierten Report-Channel oder Log.  
**Beispiel:** `/report` → Modal für Titel & Beschreibung → Report erstellt/gesendet

---

## ⚙️ Features & Verhalten
- Unterstützt sowohl **Slash**- als auch **Prefix-Commands** (z. B. `!help` optional).
- **Modal-UI** für /ausweis-erstellen und /report zur komfortablen Eingabe.
- **Freigabe-System**: Nutzer können steuern, wer ihren Ausweis sehen darf.
- **Persistenz:** Speicherung der Ausweise in einer Datenbank (z. B. MongoDB) oder JSON (je nach Konfiguration).
- **Konfigurierbar:** Prefix, Datenbank-URL, Report-Channel, Rollen etc. über `.env` oder config-Datei.

---

## 🛠️ Installation (Python 3.10)

> Voraussetzungen: Python 3.10 installiert
