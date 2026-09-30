# Jonny P Magic – neue Website

Neues Design für www.jonny-p-magic.de: dunkel und elegant, mit Gold-Akzenten, für Smartphones optimiert.

## Inhalt

| Datei | Zweck |
|---|---|
| `index.html` | Startseite: Hero, Über mich, Programme, Galerie, FAQ, Ablauf, Kontaktformular |
| `impressum.html`, `datenschutz.html` | Rechtstexte (**müssen noch ergänzt werden**) |
| `danke.html` | Seite, die nach dem Absenden des Formulars erscheint |
| `assets/style.css` | Das komplette Design (Farben oben in `:root`) |
| `assets/img/` | Platzhalter-Bilder, durch echte Fotos ersetzen |
| `jimdo/` | Layout-Code, falls die Seite bei Jimdo bleiben soll |

## Noch zu erledigen

1. **Fotos:** Eigene Fotos unter `assets/img/` ablegen (z. B. `portrait.jpg`, `galerie-1.jpg` …) und die Dateinamen in `index.html` anpassen.
   Für das Hero-Hintergrundbild in `assets/style.css` den Pfad `img/hero.svg` durch dein Bild ersetzen.
2. **Impressum:** Den Text aus dem aktuellen Jimdo-Impressum übernehmen (Adresse, E-Mail).
3. **Datenschutz:** Mit einem Generator passend zum Hoster erstellen (z. B. e-recht24.de oder datenschutz-generator.de).
4. **Texte prüfen:** Die Inhalte stammen aus öffentlich zugänglichen Infos zu Jonny P Magic (Website-Auszüge, MZvD-Profil). Bitte mit der aktuellen Seite abgleichen.
5. Optional: Showreel-Video (YouTube) einbinden, siehe Kommentar in der Galerie in `index.html`.

## Option A: Bei Jimdo bleiben

Das hängt vom Jimdo-Produkt ab:

- **Jimdo Creator mit JimdoPro/Business:** Unter *Design → Layout* kann man ein eigenes Layout mit HTML/CSS hinterlegen.
  Dafür sind `jimdo/layout.html` und `jimdo/layout.css` gedacht. Die Texte aus `index.html` fügst du dann wie gewohnt als
  Jimdo-Elemente ein; für das Kontaktformular nimmst du das Jimdo-Formular-Element.
  *Vorher den bestehenden Layout-Code sichern.*
- **Jimdo Dolphin / „Jimdo“ (neuer Baukasten) oder kostenloser Tarif:** Eigenes HTML/CSS für das Layout ist nicht möglich.
  Man kann nur Vorlage, Farben und Schriften wählen. Das neue Design lässt sich dort nur ungefähr nachbauen
  (dunkles Farbschema, Gold als Akzentfarbe, Serifen-Schrift für Überschriften).

## Option B (empfohlen): Eigenes Hosting

Die Seite besteht nur aus einfachen HTML-Dateien und kann kostenlos oder sehr günstig gehostet werden:

- **Hosting: [Netlify](https://www.netlify.com)** (kostenloser Tarif). Den Ordner per Drag-and-drop hochladen oder dieses GitHub-Repo verbinden.
  Das Kontaktformular funktioniert dort ohne Einrichtung (`data-netlify`); Anfragen kommen per E-Mail an.
- **Domain: [INWX](https://www.inwx.de)** (deutscher Anbieter, .de-Domain ca. 5 €/Jahr). Die bestehende Domain `jonny-p-magic.de` wird mit dem
  AuthCode von Jimdo umgezogen, es ist also kein Neukauf nötig. Danach die DNS-Einträge bei INWX auf Netlify zeigen lassen.
- Alternative mit allem bei einem deutschen Anbieter: **All-Inkl.com** (Tarif „Privat“, Domain inklusive).
  Das Formular braucht dort allerdings ein kleines PHP-Skript oder einen Dienst wie Formspree.

**Reihenfolge beim Umzug:** Zuerst die neue Seite bei Netlify online stellen und unter der Netlify-Adresse testen.
Dann den Domain-Umzug starten und erst danach den Jimdo-Tarif kündigen, damit die Seite nicht offline geht.
