# Gebührenrechner PWA

Eine Progressive Web App für Gebührenberechnung mit Plattform-Vergleich und Versandberechnung.

## Features

- 📊 **Plattformvergleich**: Vergleiche Gebühren zwischen eBay, Check24, Kaufland, Amazon, Metro, Hood und OTTO
- 📦 **Versandberechnung**: Automatische Auswahl des günstigsten Versandtarifs
- 💰 **Gewinnoptimierung**: VK-Vorschlag basierend auf Zielgewinn
- 📱 **PWA**: Installierbar auf Desktop und Mobilgeräten
- 🔄 **Offline-Funktionalität**: Funktioniert auch ohne Internetverbindung
- 💾 **Datenpersistenz**: Alle Einstellungen werden lokal gespeichert

## Installation als PWA

### Desktop (Chrome/Edge)
1. Öffne die App im Browser
2. Klicke auf das Install-Icon in der Adressleiste
3. Bestätige die Installation

### Mobile (Android)
1. Öffne die App in Chrome
2. Tippe auf das Menü (⋮)
3. Wähle "Zum Startbildschirm hinzufügen"

### Mobile (iOS)
1. Öffne die App in Safari
2. Tippe auf das Teilen-Icon
3. Wähle "Zum Home-Bildschirm"

## GitHub Pages Deployment

### Erstmaliges Setup

1. **Repository erstellen**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: PWA Gebührenrechner"
   ```

2. **Zu GitHub pushen**
   ```bash
   git remote add origin https://github.com/DEIN-USERNAME/DEIN-REPO-NAME.git
   git branch -M main
   git push -u origin main
   ```

3. **GitHub Pages aktivieren**
   - Gehe zu deinem Repository auf GitHub
   - Klicke auf "Settings"
   - Scrolle zu "Pages" im linken Menü
   - Unter "Source" wähle "main" Branch
   - Klicke auf "Save"
   - Deine App wird verfügbar sein unter: `https://DEIN-USERNAME.github.io/DEIN-REPO-NAME/`

### Updates deployen

```bash
git add .
git commit -m "Beschreibung der Änderungen"
git push
```

Die Änderungen werden automatisch auf GitHub Pages aktualisiert (kann 1-2 Minuten dauern).

## Lokale Entwicklung

Öffne einfach die `index.html` in einem modernen Browser. Für die volle PWA-Funktionalität (Service Worker) wird ein lokaler Server empfohlen:

```bash
# Mit Python 3
python -m http.server 8000

# Mit Node.js (npx)
npx serve

# Mit PHP
php -S localhost:8000
```

Dann öffne `http://localhost:8000` im Browser.

## Datenverwaltung

### Export
Die App bietet Export-Funktionen für:
- Marktplätze
- Kategorien
- Versandtarife
- Alle Daten zusammen

### Import
Importiere zuvor exportierte Daten über den Admin-Tab.

## Technologie

- **Frontend**: Vanilla HTML, CSS, JavaScript
- **PWA**: Service Worker, Web App Manifest
- **Speicher**: LocalStorage für Datenpersistenz
- **Hosting**: GitHub Pages (statisches Hosting)

## Browser-Unterstützung

- Chrome/Edge (Desktop & Mobile) ✅
- Firefox (Desktop & Mobile) ✅
- Safari (Desktop & Mobile) ✅

## Lizenz

Dieses Projekt ist für den persönlichen Gebrauch bestimmt.
