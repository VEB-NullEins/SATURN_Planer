# Quickguide

## Kurzeinleitung
Im Wesentlichen werden drei Komponenten automatisch kalkuliert: 
- Standort der Anlage
- Kranstellfläche
- eine Reihe von relevanten Abstandskreisen

 Die Kalkulation findet auf Basis von Angaben über das jeweilige Projektgebiet (Hauptwindrichtung, Baulastregel, Abstände…) statt. Mithilfe von einfacher Linienausrichtung oder dem Nachzeichnen eines Weges kann eine oder mehrere Anlagen dann im Projektgebiet platziert werden.

 ## Voraussetzungen
 QGIS 3 muss bereits installiert sein. Für die Nutzung des SATURN Planer sind zudem folgende QGIS Kenntnisse hilfreich:
- Bedienung des Datenquellenmanagers oder des Datenbrowsers
- Layer Anzeige
- Editing Modus für Layer aktivieren und Feature hinzufügen oder bearbeiten
- Attributtabelle aufrufen und bearbeiten

## Schritt-für-Schritt Anleitung
### Öffnen des SATURN Planers aus Geopackage
→ QGIS starten

→ Über Menüleiste: Projekt>Öffnen aus>Geopackage

<p><img width=70% src="./img/QG_Geopackage_oeffnen.png" /></p>

→ Bei Verbindung den Pfad bis zum Geopackage „SATURN_Planer.gpkg“ durchklicken

<p><img width=35% src="./img/QG_Projekt_laden.png"/></p>

→ OK klicken

---
### Erstellen einer Windparkkonfiguration
#### Schritt 1: Basis – Projektgebiet erstellen

→ Layer „Basis – Projektgebiet“ anklicken 

<p><img width=35% src="./img/QG_Layeranzeige_Projektgebiet.png" /></p>

→ Editiermodus aktivieren

<p><img width=35% src="./img/QG_Editiermodus.png" /></p>

→ Polygon Feature hinzufügen

<p><img width=35% src="./img/QG_Polygon_hinzu.png" /></p>

→ Projektgebiet zeichnen und mit Rechtsklick abschließen:

<p><img width=35% src="./img/QG_Projektgebiet_zeichnen.png" /></p>

→ Projektangaben machen:

<p><img width=35% src="./img/QG_Projektgebiet_Angaben.png" /></p>

→ Mit „OK“ bestätigen

→ Wichtig: Speichern des Layer Edits!

<p><img width=35% src="./img/QG_Polygon_speichern.png" /></p>

#### Schritt 2: Windparklayout erstellen

#### - _Option 1: WEA Linienausrichtung_
 
→ Layer „Option 1 – WEA Linienausrichtung“ auswählen

<p><img width=35% src="./img/QG_Linie_1.png" /></p>

→ Editiermodus aktivieren und Linienobjekt hinzufügen

<p><img width=35% src="./img/QG_Linie_2.png" /></p>

→ Linie einzeichnen (1. Punkt Anlagenmittelpunkt/ 2. Punkt Kranausrichtung)

<p><img width=35% src="./img/QG_Linie_3.png" /></p>

→ mit OK bestätigen

→ Vorschau der Anlage erscheint

<p><img width=35% src="./img/QG_Linie_4.png" /></p>

→ Wichtig: Speichern

<p><img width=35% src="./img/QG_Linie_5.png" /></p>

→ Kranstellfläche, Mittelpunkt und Abstände werden kalkuliert

<p><img width=70% src="./img/QG_Linie_6.png" /></p>

#### - _Option 2: WEA Wegausrichtung_

→ Layer „Option 1 – WEA Linienausrichtung“ auswählen

<p><img width=35% src="./img/QG_Weg_1.png" /></p>

→ Editiermodus aktivieren und Linienobjekt hinzufügen

<p><img width=35% src="./img/QG_Weg_2.png" /></p>

→ Linie mit zwei Punkten entlang Weg zeichnen (1. Punkt Höhe Anlagenstandort)

→ Formular ausfüllen: Wegseite Kranausleger bedeutet entlang des Linienverlaufs wird die Anlage rechts oder links platziert

<p><img width=35% src="./img/QG_Weg_3.png" /></p>

→ mit OK bestätigen

→ Wichtig: Speichern

<p><img width=35% src="./img/QG_Weg_4.png" /></p>

→ Kranstellfläche, Mittelpunkt und Abstände werden kalkuliert

<p><img width=70% src="./img/QG_Weg_5.png" /></p>

### Windparkkonfiguration anpassen

→ Layer „Option 1 – …“ oder „Option 2 – ...“ auswählen je nach Ursprung

→ Editiermodus aktivieren und Stützpunktwerkzeug auswählen

<p><img width=35% src="./img/QG_anpassen_1.png" /></p>

→ Stützpunkt/Vertex auswählen und auf neue Position schieben

<p><img width=35% src="./img/QG_anpassen_2.png" /></p>

→ Wichtig: Speichern

<p><img width=35% src="./img/QG_anpassen_3.png" /></p>

→ Kranstellfläche, Mittelpunkt und Abstände werden neu kalkuliert

<p><img width=35% src="./img/QG_anpassen_4.png" /></p>

---
### Anlagen löschen
→ Layer „Standort WEA“ wählen

<p><img width=35% src="./img/QG_loeschen_1.png" /></p>

→ Editiermodus aktivieren

<p><img width=35% src="./img/QG_loeschen_2.png" /></p>

→ Objekt über Rechteck auswählen

<p><img width=35% src="./img/QG_loeschen_3.png" /></p>

→ Anlagenmittelpunkt auswählen (erscheint danach gelb)

<p><img width=35% src="./img/QG_loeschen_4.png" /></p>

→ Auswahl löschen
 
 <p><img width=35% src="./img/QG_loeschen_5.png" /></p>

→ Wichtig: Speichern

→ Anlage wird gelöscht

---
### Versionsplanung
→ Layer „Basis – Projektgebiet“ anklicken 

<p><img width=35% src="./img/QG_Version_1.png" /></p>

→ Rechtsklick und Attributtabelle öffnen

<p><img width=35% src="./img/QG_Version_2.png" /></p>

→ Editiermodus aktivieren

<p><img width=35% src="./img/QG_Version_3.png" /></p>

→ In der Tabelle „Planungsversion“ eine andere Version auswählen

<p><img width=35% src="./img/QG_Version_4.png" /></p>

→ mit Enter bestätigen
→ wichtig: Speichern!

<p><img width=35% src="./img/QG_Version_5.png" /></p>

→ neue Planungsversion wurde ausgewählt und kann beplant werden
→ weitere Vorgaben können für die Version angepasst werden zum Beispiel anderer Anlagentyp oder andere Baulastregeln
→ um zu einer bereits vorhandenen Planungsversion zurückzukehren muss diese einfach wieder in der Attributtabelle ausgewählt werden und die Tabelle gespeichert werden (siehe oben)
