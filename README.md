# SCHWEISSRING Website - GitHub + Netlify + Decap CMS Setup

## 📋 Was ist enthalten?

Diese Website ist **komplett fertig** und bereit für:
- ✅ GitHub Hosting
- ✅ Netlify Deployment
- ✅ Decap CMS (benutzerfreundlicher Editor)
- ✅ Kostenlos & wartungsfrei

---

## 🚀 SETUP-ANLEITUNG (Schritt für Schritt)

### SCHRITT 1: Repository auf GitHub erstellen

1. **Gehe zu GitHub** → https://github.com
2. **Klicke auf das "+" oben rechts** → "New repository"
3. **Repository-Name:** `schweissring-website` (oder einen anderen Namen)
4. **Beschreibung:** "SCHWEISSRING Website mit Decap CMS"
5. **Sichtbarkeit:** Public (oder Private - beides funktioniert)
6. **WICHTIG:** 
   - ❌ **NICHT** "Add a README file" anklicken
   - ❌ **NICHT** ".gitignore" hinzufügen
   - ❌ **NICHT** "Choose a license" auswählen
7. **Klicke auf "Create repository"**

---

### SCHRITT 2: Dateien auf GitHub hochladen

#### Option A: GitHub Desktop (einfacher für Anfänger)

1. **GitHub Desktop herunterladen:** https://desktop.github.com
2. **Installieren und mit GitHub-Account anmelden**
3. **File → Clone Repository** → Dein neues Repository auswählen
4. **Lokalen Ordner wählen** (wo die Dateien gespeichert werden)
5. **Alle Website-Dateien in diesen Ordner kopieren**
6. **In GitHub Desktop:**
   - Summary: "Initial website setup"
   - Klicke auf "Commit to main"
   - Klicke auf "Push origin"
7. **Fertig!** Dateien sind auf GitHub

#### Option B: Web-Interface (noch einfacher!)

1. **In deinem neuen Repository auf GitHub.com**
2. **Klicke auf "uploading an existing file"**
3. **Ziehe ALLE Dateien und Ordner in das Upload-Feld**
   - Alle .html Dateien
   - styles.css
   - admin/ Ordner
   - content/ Ordner
   - images/ Ordner
4. **Commit message:** "Initial website upload"
5. **Klicke auf "Commit changes"**
6. **Fertig!** Dateien sind auf GitHub

#### Option C: Git Command Line (für Fortgeschrittene)

```bash
# In dem Ordner mit den Website-Dateien
git init
git add .
git commit -m "Initial website setup"
git branch -M main
git remote add origin https://github.com/DEIN-USERNAME/schweissring-website.git
git push -u origin main
```

---

### SCHRITT 3: Mit Netlify verbinden

1. **Gehe zu Netlify:** https://app.netlify.com
2. **Klicke auf "Sign up"** (oder "Log in" falls du schon einen Account hast)
3. **Wähle "Sign up with GitHub"** (empfohlen)
4. **Autorisiere Netlify** auf deinem GitHub-Account

#### Site deployen:

5. **Klicke auf "Add new site"** → "Import an existing project"
6. **Wähle "Deploy with GitHub"**
7. **Autorisiere Netlify** (falls noch nicht geschehen)
8. **Wähle dein Repository** `schweissring-website` aus
9. **Build Settings:**
   - Branch to deploy: `main`
   - Build command: *(leer lassen)*
   - Publish directory: `/` (oder leer lassen)
10. **Klicke auf "Deploy site"**

**⏱️ Warte 1-2 Minuten** - Netlify deployt deine Website!

---

### SCHRITT 4: Decap CMS aktivieren

#### 4.1 Identity Service aktivieren:

1. **In Netlify, gehe zu deiner Site**
2. **Klicke auf "Site settings"** (in der Navigation)
3. **Klicke auf "Identity"** im Menü links
4. **Klicke auf "Enable Identity"**

#### 4.2 Git Gateway aktivieren:

5. **Scrolle runter zu "Services"**
6. **Klicke auf "Enable Git Gateway"**

#### 4.3 Registration Einstellungen:

7. **Gehe zu "Identity" → "Settings and usage"**
8. **Registration preferences:**
   - Wähle **"Invite only"** (nur eingeladene Nutzer)
   - Oder **"Open"** wenn mehrere Leute Zugriff haben sollen

#### 4.4 Benutzer einladen:

9. **Klicke auf "Identity"** (im Hauptmenü)
10. **Klicke auf "Invite users"**
11. **Gib deine E-Mail-Adresse ein**
12. **Klicke auf "Send"**

#### 4.5 Einladung annehmen:

13. **Prüfe deine E-Mails** (auch Spam-Ordner!)
14. **Klicke auf den Link** in der Einladungs-E-Mail
15. **Erstelle ein Passwort**
16. **Fertig!** Du bist jetzt angemeldet

---

### SCHRITT 5: Admin-Bereich nutzen

1. **Gehe zu:** `https://deine-seite.netlify.app/admin/`
   - Ersetze `deine-seite` mit deinem Netlify-Subdomain
   - Oder verwende deine eigene Domain wenn eingerichtet

2. **Melde dich an** mit deinem Account

3. **Du siehst jetzt das CMS-Dashboard!** 🎉

---

## 📝 WIE DU INHALTE BEARBEITEST

### Im Admin-Bereich kannst du bearbeiten:

#### 📄 **Seiten:**
- **Startseite:** Hero-Text, Feature-Karten, CTA
- **Kontakt:** Kontaktdaten aktualisieren

#### 👥 **Partner:**
- Partner hinzufügen
- Partner bearbeiten
- Partner löschen
- Logo hochladen

#### 💼 **Stellenangebote:**
- Neue Jobs erstellen
- Bestehende Jobs bearbeiten
- Jobs aktivieren/deaktivieren

#### 📢 **Aktionen & Kataloge:**
- Neue Aktionen erstellen
- Gültigkeitsdatum setzen
- Aktionen aktivieren/deaktivieren

### So funktioniert die Bearbeitung:

1. **Klicke auf die Collection** (z.B. "Partner")
2. **Wähle einen Eintrag** oder klicke auf "New Partner"
3. **Bearbeite die Felder**
4. **Klicke auf "Save"**
5. **Klicke auf "Publish"** (oben rechts)
6. **⏱️ Warte 1-2 Minuten** - Änderungen gehen live!

---

## 🎨 DEINE WEBSITE-URL

### Temporäre Netlify-URL:
Nach dem Deployment bekommst du eine URL wie:
```
https://zufaelliger-name-12345.netlify.app
```

### Eigene Domain verbinden (optional):

1. **In Netlify → Site settings → Domain management**
2. **Klicke auf "Add custom domain"**
3. **Gib deine Domain ein** (z.B. `www.schweissring.de`)
4. **Folge den Anweisungen** für DNS-Setup
5. **Netlify stellt automatisch ein SSL-Zertifikat aus** (HTTPS)

---

## 📂 DATEISTRUKTUR

```
schweissring-website/
│
├── admin/                          # Decap CMS Admin-Bereich
│   ├── index.html                  # Admin-Interface
│   └── config.yml                  # CMS-Konfiguration
│
├── content/                        # Bearbeitbare Inhalte
│   ├── partner/                    # Partner-Daten
│   ├── jobs/                       # Stellenangebote
│   └── promotions/                 # Aktionen/Kataloge
│
├── images/                         # Bilder
│   └── uploads/                    # Hochgeladene Bilder (vom CMS)
│
├── *.html                          # Alle Website-Seiten
├── styles.css                      # Haupt-Stylesheet
└── README.md                       # Diese Anleitung
```

---

## 🔧 WICHTIGE EINSTELLUNGEN

### Branch-Name:
Die Website nutzt den **`main`** Branch. Falls dein Repository **`master`** nutzt:

1. **Öffne:** `admin/config.yml`
2. **Ändere Zeile 3:**
   ```yaml
   branch: master  # statt main
   ```
3. **Commit & Push** die Änderung

### Logo hinzufügen:

1. **Bereite dein Logo vor:**
   - PNG mit transparentem Hintergrund
   - Empfohlene Größe: 300×80px
   - Dateiname: `logo.png`

2. **Hochladen:**
   - Entweder über GitHub direkt in den `images/` Ordner
   - Oder über Netlify CMS (wenn Partner-Logo hochgeladen wird)

3. **In HTML einbinden:**
   - Suche in allen .html Dateien nach: `<img src="logo.png"`
   - Ersetze mit: `<img src="/images/logo.png"`

---

## 🆘 HÄUFIGE PROBLEME & LÖSUNGEN

### Problem: "Admin-Bereich zeigt 404"
**Lösung:** 
- Überprüfe ob der `admin/` Ordner auf GitHub vorhanden ist
- Netlify neu deployen: Site settings → Build & deploy → Trigger deploy

### Problem: "Login funktioniert nicht"
**Lösung:**
- Überprüfe ob Identity aktiviert ist (Site settings → Identity)
- Überprüfe ob Git Gateway aktiviert ist
- Lade dich selbst neu ein

### Problem: "Änderungen gehen nicht live"
**Lösung:**
- Klicke auf "Publish" nicht nur "Save"
- Warte 2-3 Minuten für Deployment
- Prüfe unter Deploys ob ein neuer Build läuft

### Problem: "Logo wird nicht angezeigt"
**Lösung:**
- Überprüfe Dateipfad: sollte `/images/logo.png` sein
- Stelle sicher dass die Datei auf GitHub existiert
- Cache leeren (Strg+F5 im Browser)

---

## 🎯 NÄCHSTE SCHRITTE

Nach dem Setup kannst du:

1. **Logo hinzufügen** (siehe oben)
2. **Alle Partner eingeben** über den Admin-Bereich
3. **Kontaktdaten aktualisieren** in "Seiten → Kontakt"
4. **Stellenangebote erstellen** in "Stellenangebote"
5. **Eigene Domain verbinden** (optional)

---

## 💡 TIPPS & TRICKS

### Lokale Vorschau (optional):
Falls du Änderungen lokal testen willst:

```bash
# Simple HTTP Server starten
npx http-server
# Oder mit Python:
python -m http.server 8000
```

Dann öffne: `http://localhost:8000`

### Backup erstellen:
GitHub IST dein Backup! Alle Versionen sind gespeichert.

**Ältere Version wiederherstellen:**
1. GitHub Repository → "Commits"
2. Finde die gewünschte Version
3. Klicke auf "Browse files" bei diesem Commit
4. Dateien downloaden

### Content-Updates automatisieren:
Decap CMS speichert alle Änderungen direkt in deinem GitHub Repository. Das bedeutet:
- Vollständige Versionskontrolle
- Jede Änderung ist nachvollziehbar
- Rollback jederzeit möglich

---

## 📞 SUPPORT

### Netlify Docs:
https://docs.netlify.com

### Decap CMS Docs:
https://decapcms.org/docs/

### GitHub Docs:
https://docs.github.com

### Community:
- Netlify Discord
- Decap CMS GitHub Discussions

---

## ✅ CHECKLISTE

Hake ab, wenn erledigt:

- [ ] GitHub Repository erstellt
- [ ] Dateien auf GitHub hochgeladen
- [ ] Netlify-Account erstellt
- [ ] Repository mit Netlify verbunden
- [ ] Website deployt (funktioniert!)
- [ ] Netlify Identity aktiviert
- [ ] Git Gateway aktiviert
- [ ] Benutzer eingeladen
- [ ] Einladung angenommen
- [ ] Admin-Bereich erreichbar (`/admin/`)
- [ ] Erfolgreich eingeloggt
- [ ] Logo hochgeladen
- [ ] Kontaktdaten aktualisiert
- [ ] Partner eingepflegt
- [ ] Teständerung gemacht und gepublisht

---

## 🎉 FERTIG!

Du hast jetzt eine:
- ✅ Kostenlose Website
- ✅ Ohne Wartungsaufwand
- ✅ Mit benutzerfreundlichem Editor
- ✅ Auf moderner Technologie
- ✅ Schnell & sicher (JAMstack)

**Viel Erfolg mit deiner SCHWEISSRING-Website!** 🚀

---

## 📧 Fragen?

Bei Problemen kannst du:
1. Diese README nochmal durchlesen
2. Die verlinkten Docs checken
3. In den Community-Foren fragen

Die Website ist **production-ready** und kann sofort live gehen!
