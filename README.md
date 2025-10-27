# Babsy Stundenrapport Formular - Setup Anleitung

## 🚀 Web3Forms Setup (3 einfache Schritte)

### Schritt 1: Access Key erstellen
1. Gehe zu: https://web3forms.com/
2. Klicke auf "Get Started for Free"
3. Gib deine Email-Adresse ein: **company@babsy.ch**
4. Du erhältst einen **Access Key** (z.B. `a1b2c3d4-e5f6-7890-abcd-ef1234567890`)

### Schritt 2: Access Key im Formular eintragen
1. Öffne die Datei `babsy-stundenrapport.html`
2. Suche die Zeile (ca. Zeile 449):
   ```html
   <input type="hidden" name="access_key" value="DEIN-WEB3FORMS-ACCESS-KEY">
   ```
3. Ersetze `DEIN-WEB3FORMS-ACCESS-KEY` mit deinem echten Access Key
4. Speichern!

### Schritt 3: Hochladen und testen
1. Lade beide Dateien auf GitHub hoch:
   - `babsy-stundenrapport.html` (das Formular)
   - `danke.html` (die Danke-Seite)
2. Passe in `babsy-stundenrapport.html` die Redirect-URL an (Zeile 452):
   ```html
   <input type="hidden" name="redirect" value="https://DEINE-GITHUB-PAGES-URL/danke.html">
   ```
3. Teste das Formular!

## ✨ Features

### Tagesweise Stundenerfassung
- Wähle einen Datumsbereich (von - bis)
- Das System zeigt automatisch alle Tage an
- Trage für jeden Tag die Stunden ein
- Gesamtsumme wird automatisch berechnet

### Mehrere Einsätze
- Beliebig viele Einsätze hinzufügen möglich
- Jeder Einsatz mit eigener Stundenerfassung
- Übersichtliche Darstellung

### E-Mail-Versand
- Alle Daten werden an **company@babsy.ch** gesendet
- Absender erhält automatisch eine Kopie (Reply-To)
- Übersichtliche Formatierung in der E-Mail

## 📊 Kosten

**Komplett KOSTENLOS!**
- Web3Forms: Unbegrenzte Submissions
- Kein Account erforderlich
- Keine Rate Limits
- Perfekt für deine 300+ Submissions pro Monat

## 🔧 Anpassungen

### E-Mail-Empfänger ändern
Zeile 450 in `babsy-stundenrapport.html`:
```html
<input type="hidden" name="email" value="company@babsy.ch">
```

### Betreff ändern
Zeile 451:
```html
<input type="hidden" name="subject" value="Neuer Babsy-Sitter Stundenrapport">
```

### Redirect-URL ändern
Zeile 452:
```html
<input type="hidden" name="redirect" value="https://babsy.ch/danke.html">
```

## 🐛 Troubleshooting

### Formular sendet nicht
- Access Key korrekt eingefügt?
- Formular von der richtigen Domain abgeschickt? (nicht file:///)
- Browser-Konsole auf Fehler prüfen

### E-Mail kommt nicht an
- Spam-Ordner prüfen
- Access Key nochmal verifizieren auf web3forms.com
- Email-Adresse in Web3Forms Dashboard prüfen

### 500 Server Error
- Web3Forms hat keine Rate Limits → sollte nicht passieren
- Access Key überprüfen
- Formular-Struktur überprüfen

## 📧 Support

Bei Fragen oder Problemen:
- Web3Forms Docs: https://docs.web3forms.com/
- Web3Forms Support: support@web3forms.com

## 📝 Dateien

- `babsy-stundenrapport.html` - Das Hauptformular
- `danke.html` - Bestätigungsseite nach dem Absenden

## 🎯 Was in den E-Mails enthalten ist

Jede Submission enthält:
- Persönliche Daten (Name, Email, Telefon)
- Berichtszeitraum (Monat/Jahr)
- Alle Einsätze mit:
  - Datumsbereich
  - Detaillierte Stunden pro Tag
  - Gesamtstunden
  - Stundenansatz
  - Familie/Kunde
  - Ort
  - Tätigkeit
  - Bemerkungen

---

**Viel Erfolg! 🍼💜**
