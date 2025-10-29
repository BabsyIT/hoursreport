# 🎹 Babsy Stundenrapport - Tastatur-Optimierte & Zweisprachige Version

## ✨ Was ist neu?

### 🌍 Zweisprachige E-Mails (DE/EN)
Alle Felder werden jetzt mit **zweisprachigen Namen** versendet, sodass die E-Mail sowohl auf Deutsch als auch auf Englisch lesbar ist:

**Beispiel E-Mail:**
```
Vorname / First Name: Max
Nachname / Last Name: Mustermann
E-Mail-Adresse / Email Address: max@email.ch
Telefon / Phone: +41 79 123 45 67
Monat / Month: Januar/January
Jahr / Year: 2025

=== Einsatz 1 / Entry 1 ===
Datum von / Date from: 2025-01-15
Datum bis / Date to: 2025-01-20

Tag 2025-01-15 / Day 2025-01-15: 8 h
Tag 2025-01-16 / Day 2025-01-16: 7.5 h
Tag 2025-01-17 / Day 2025-01-17: 8 h
Tag 2025-01-18 / Day 2025-01-18: 4 h
Tag 2025-01-19 / Day 2025-01-19: 8 h

Gesamtstunden / Total Hours: 35.5 h
Stundenansatz CHF / Hourly Rate CHF: 25.00
Familie Kundenname / Family Client Name: Familie Müller
Ort Einsatz / Location: Zürich
Tätigkeit / Activity: Babysitting
Bemerkungen / Notes: Sehr nette Familie
```

### 🎯 Keine Pfeile bei Stunden-Feldern (Desktop)
Die störenden Pfeile (Spinner) bei Number-Inputs wurden entfernt - perfekt für Tastatur-Eingabe!

## 🚀 Tastatur-Features (Desktop)

### **1. Super-schnelle Stunden-Eingabe**
- **Enter** = nächster Tag
- **Zahlen 1-8** = Direkte Schnelleingabe (einfach die Zahl tippen!)
- **Schnellwahl-Buttons** unter jedem Feld (1h, 2h, 3h, 4h, 5h, 8h)
- **Keine Pfeile** = Kein versehentliches Klicken mehr

### **2. Intelligente Navigation**
- **Enter** = nächstes Feld
- **Shift+Enter** = nur Pflichtfelder (überspringt optionale Felder!)
- Automatisches Öffnen von Dropdowns
- Auto-Select von Text für schnelles Überschreiben

### **3. Globale Shortcuts**
- **Ctrl/Cmd + E** = Neuer Einsatz
- **Ctrl/Cmd + S** = Absenden
- **Esc** = Hilfe schließen

### **4. Visuelles Feedback**
- ✨ Leuchtende Focus-Highlights
- 💡 Popup-Hints bei Aktionen
- 🎯 Smooth Scrolling zum aktiven Feld
- 📊 Felder werden beim Focus leicht vergrößert

### **5. Hilfe-Panel**
- Button **"⌨️ Tastatur-Hilfe"** (unten links)
- Zeigt alle Shortcuts
- Immer verfügbar

## 📧 E-Mail Format

### Vorteile der zweisprachigen E-Mails:
1. ✅ **International verständlich** - Englische Sitter können E-Mails lesen
2. ✅ **Buchhaltung friendly** - Beide Sprachen auf einen Blick
3. ✅ **Keine Verwirrung** - Klare Zuordnung aller Felder
4. ✅ **Professionell** - Zeigt Internationalisierung

### Struktur:
```
=== Persönliche Angaben / Personal Information ===
[Zweisprachige Felder]

=== Berichtszeitraum / Reporting Period ===
[Zweisprachige Felder]

=== Einsatz 1 / Entry 1 ===
[Datum-Bereich]
[Tagesweise Stunden mit Datum]
[Gesamtstunden]
[Weitere Details]

=== Einsatz 2 / Entry 2 ===
[...]
```

## 🎯 Beispiel-Workflow (nur Tastatur):

```
Max [Enter] 
Mustermann [Enter] 
max@email.ch [Enter]
+41 79... [Shift+Enter zum Überspringen]

[Monat wählen] [Enter] 
2025 [Enter]

2025-01-15 [Enter]  → Tabelle erscheint
2025-01-20 [Enter]

8 [Enter]  (oder nur "8" tippen bei leerem Feld)
7 [Enter]
8 [Enter]
4 [Enter]
8 [Enter]

25 [Enter]
Familie Müller [Enter]
Zürich [Enter]

[Ctrl+E für neuen Einsatz]
[Ctrl+S zum Absenden]
```

## 🔧 Tastatur-Shortcuts Übersicht

| Aktion | Shortcut | Kontext |
|--------|----------|---------|
| Nächstes Feld | `Enter` | Überall |
| Nur Pflichtfelder | `Shift + Enter` | Überall |
| Neuer Einsatz | `Ctrl/Cmd + E` | Global |
| Absenden | `Ctrl/Cmd + S` | Global |
| Hilfe schließen | `Esc` | Hilfe-Panel |
| Nächster Tag | `Enter` | Stunden-Eingabe |
| Schnelleingabe | `1-8` | Stunden-Eingabe (leeres Feld) |

## 💡 Besondere Features

### Stunden-Felder ohne Pfeile
- Desktop: Keine störenden Spinner-Pfeile
- Cleaner Look
- Bessere Tastatur-Erfahrung
- Fokus bleibt auf dem Feld

### Intelligente Feld-Navigation
Das Formular erkennt automatisch:
- Pflichtfelder (⭐ mit rotem Stern)
- Optionale Felder (können übersprungen werden)
- Datum-Felder (generieren automatisch Tabellen)
- Stunden-Felder (spezielle Shortcuts aktiv)

### Visuelle Hinweise
- **Grüne Felder** = Automatisch übernommen (Copy-to-All aktiv)
- **Leuchtender Rahmen** = Aktuell fokussiertes Feld
- **Popup-Hints** = Bestätigung bei wichtigen Aktionen

## ⚙️ Setup & Installation

1. **Lade die Dateien hoch:**
   - `index.html` (Hauptformular)
   - `danke.html` (Bestätigungsseite)

2. **Füge deinen Web3Forms Access Key ein:**
   ```html
   <input type="hidden" name="access_key" value="DEIN-KEY-HIER">
   ```

3. **Passe die Redirect-URL an:**
   ```html
   <input type="hidden" name="redirect" value="https://DEINE-URL/danke.html">
   ```

4. **Fertig! 🎉**

## 📊 Technische Details

### Feldnamen-Konvention:
Alle Felder nutzen das Format:
```
"Deutscher_Name / English_Name"
```

Beispiele:
- `Vorname / First Name`
- `Einsatz_1__Datum_von / Date_from`
- `Einsatz_1__Tag_2025-01-15 / Day_2025-01-15`
- `Gesamtstunden / Total_Hours`

### CSS für Number-Inputs ohne Pfeile:
```css
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
    -webkit-appearance: none;
    margin: 0;
}
input[type="number"] {
    -moz-appearance: textfield;
    appearance: textfield;
}
```

## 📱 Mobile vs Desktop

**Desktop (diese Version):**
- ✅ Alle Tastatur-Shortcuts aktiv
- ✅ Hilfe-Panel verfügbar
- ✅ Auto-Focus und Auto-Select
- ✅ Keine Number-Input Pfeile
- ✅ Optimiert für schnelle Eingabe

**Mobile:**
- ✅ Touch-optimiert
- ✅ Zweisprachige E-Mails
- ❌ Keine Keyboard-Shortcuts
- ✅ Vereinfachte Navigation
- ✅ Alle Features bleiben funktional

## 🎓 Tipps für Benutzer

### Für deutsche Benutzer:
- Alle Felder sind auf Deutsch beschriftet
- E-Mail enthält beide Sprachen
- Navigation bleibt intuitiv

### Für englische Benutzer:
- Alle Beschriftungen zeigen englische Übersetzung
- E-Mail ist vollständig verständlich
- Workflow identisch

### Für die Buchhaltung:
- Beide Sprachen in einer E-Mail
- Klare Struktur
- Einfaches Copy-Paste in Excel
- Automatische Gesamtsummen

## 🐛 Bekannte Einschränkungen

- Tastatur-Shortcuts funktionieren nur auf Desktop
- Mobile Geräte nutzen Touch-Navigation
- Browser-Autofill kann Shortcuts überlagern (Tab drücken)
- E-Mail-Feldnamen können etwas länger aussehen (aber besser lesbar!)

## 💬 Support

Bei Fragen oder Problemen:
- 📧 Email: sitter@babsy.ch
- 📱 WhatsApp: +41 78 861 60 25

---

## 📋 Changelog

### Version 2.0 (Aktuell)
- ✅ Zweisprachige E-Mails (DE/EN)
- ✅ Number-Input Pfeile entfernt (Desktop)
- ✅ Verbesserte Tastatur-Navigation
- ✅ Schnelleingabe für Stunden (1-8)
- ✅ Globale Shortcuts (Ctrl+E, Ctrl+S)
- ✅ Visuelles Feedback System
- ✅ Hilfe-Panel integriert

### Version 1.0
- Basis-Formular mit tagesweiser Stundenerfassung
- Mehrere Einsätze möglich
- Web3Forms Integration

---

**Viel Spaß mit der tastatur-optimierten & zweisprachigen Version! 🎹🌍✨**

*Tipp: Zeige neuen Team-Mitgliedern die Tastatur-Hilfe (⌨️ unten links) für einen schnellen Start!*
