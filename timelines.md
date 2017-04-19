Das Timelines Plugin erlaubt in Omeka aus Objekten Zeitstrahlen für [TimelineJS][1] zu erstellen.

## Timelines Plugin konfigurieren

Sie können initial den verwendeten Objekt-Typ für die Zeitstrahlen festlegen.
Gehen Sie dazu in der Omeka-Administrations-Schnittstelle auf Plgins->Timeline->konfigurieren

!![Timeline Plugin konfigurieren][g1]

!!! warning "Achtung"
    Beachten Sie, dass der Objekttyp bei bereits angelegten Zeitstrahlen nicht mehr verändert werden kann.
    Sie sollten also diese Einstellung einmalig, bevor Sie Zeitstrahlen anlegen, vornehmen.

## Anlegen von Zeitstrahlen

Klicken Sie in der Omeka-Administrations-Schnittstelle auf den Menüpunkt "Timelines" und dort auf den Knopf "Timeline hinzufügen".
Das Formular ist in drei Teile geteilt:

- Timeline Einstellungen
- Timeline Cover / Startseite
- Metadaten Zuordnungen

### Timeline Einstellungen

Hier können Sie globale Einstellungen für den gesamten Zeitstrahl angeben.

#### Name der Timeline

Geben Sie hier einen beliebigen Namen ein, um den Zeitstrahl später identifizieren zu können.
Der Name dient dabei nur der internen Erkennung und wird nicht im Frontend ausgegeben.

#### Hintergrundfarbe

Geben Sie hier die Hintergrundfarbe als Hexadezimalwert an, Bsp.: #66ccff.
Diese Hintergrundfarbe ist die Standardfarbe für den Zeitstrahl (alle Slices), kann aber bei den einzelnen Objekten überschrieben werden.

### Timeline Cover / Startseite

#### Startseite ignorieren

Ist diese Option gewählt, werden Einstellungen der Startseite hier ignoriert. Stattdessen kann optional ein Objekt in der Objektauswahl als Startseite festgelegt werden.

#### URL zum Bild

Geben Sie hier eine URL zum Coverbild an.
Die URL muss vollständig mit Protokoll angegeben werden z.B.: http(s)://domainname.tld/unterverzeichnis/bild.jpg

#### Bildunterschrift

Geben Sie hier die Bildunterschrift an.

#### Credit / Copyright

Geben Sie hier die Copyrighthinweise an.

#### Überschrift

Geben Sie hier die Überschrift an.

!!! note "Beachten Sie"
    Alle HTML-Auszeichnungen außer Umbrüchen (&lt;br&gt; bzw. &lt;br/&gt;) werden bei der Ausgabe ignoriert.


#### Text

Geben Sie hier den Beschreibungstext ein.


### Metadaten Zuordnungen

Ordnen Sie hier die jeweiligen Felder des Objekttyps dem Feldern des Zeitstrahls zu.
Sie müssen dabei nicht alle Felder zuordnen.

!!! note "Beachten Sie"
    Die Felder für Stunde, Minute und Sekunde werden derzeit im Plugin ignoriert, Sie können also die Zuordnungen leer lassen.


## Bearbeiten von Zeitstrahlen

Wenn Sie einen Zeitstrahl erfolgreich angelegt haben können Sie diesen bearbeiten und insbesondere Objekte auswählen und bearbeiten.

!![Zeitstrahl Bearbeitungsmöglichkeiten in der Übersicht][g2]

### Bearbeiten

Hier können Sie die Einstellungen, die Sie beim Erzeugen des Zeitstrahls gesetzt haben. bearbeiten

### Löschen

Hier können Sie den gesamten Zeitstrahl löschen

### Objekte auswählen

Hier können Sie die Objekte für den Zeitstrahl auswählen und ggf. ein Objekt für die Startseite angeben.

!![Auswahl von Objekten und einem Startseiten-Objekt für einem Zeitstrahl][g5]

### Objekte bearbeiten

Hier könne Sie die Objekte, die Sie zuvor für den Zeitstrahl ausgewählt haben (siehe "Objekte auswählen"), bearbeiten und so Eigenschaften von Objekten für die Anzeige überschreiben.
Für jedes Objekt werden oben das erste Bild des Objekts und die relevaten Felder angezeigt. Darunter können Sie die Felder für das jeweilige Objekt überschreiben.

!![Zeitstrahl Bearbeitungsmöglichkeiten in der Übersicht][g3]

!!! note "Beachten Sie"
    Das Überschreiben von Feldern überschreibt nicht die Eigenschaften des Objekts, es gilt nur für die Ausgabe im Zeitstrahl.



### Shortcode

Hier sehen Sie den Shortcode, den Sie bei einer SimplePage verwenden können, um den jeweiligen Zeitstrahl anzuzeigen.
Sie können den Shortcode per Copy & Paste in den WYSIWYG-Editor der SimplePage kopieren:

!![Einbinden eines Shortcodes für Zeitstrahlen bei einer SimplePage][g4]

!!! note "Beachten Sie"
    Geben Sie bei der SimplePage, auf der Sie einen Zeitrahl anzeigen lassen möchten, im Bereich "Layout" die Auswahl "Volle Seitenbreite" an!


[1]: http://timeline.knightlab.com/  "TimelineJS"
[g1]: img/timelines-001.png  "Timeline Plugin konfigurieren"
[g2]: img/timelines-002.png  "Zeitstrahl Bearbeitungsmöglichkeiten in der Übersicht"
[g3]: img/timelines-003.png  "Zeitstrahl Bearbeitungsmöglichkeiten in der Übersicht"
[g4]: img/timelines-004.png  "Einbinden eines Shortcodes für Zeitstrahlen bei einer SimplePage"
[g5]: img/timelines-005.png  "Auswahl von Objekten und einem Startseiten-Objekt für einem Zeitstrahl"