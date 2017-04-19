Das Spreadsheets Plugin ist ein Plugin zum Exportieren und Importieren von
Omeka-Objekten nach bzw. aus MS Excel Spreadsheets.

Es besteht aus zwei Teilen:

- Objekte als Excel Datei exportieren
- Objekte aus Excel Datei importieren

!![Spreadsheets Plugin Übersicht][g1]

## Objekte als Excel Datei exportieren

Der Export erfolgt ins XLSX (Excel 2007) Format.

Um Objekte als Excel Datei zu exportieren legen Sie zunächt ein Schema an.
Gehen Sie dazu in der Übersicht auf "Schema hinzufügen".

### Schema hinzufügen

#### Name

Geben Sie hier einen beliebigen Namen ein, um das Schema später identifizieren zu können.
Der Name dient dabei nur der internen Erkennung.

#### Objekttyp

Wählen Sie hier den zu exportierenden Objekttyp aus.
Pro Schema kann immer nur ein Objekttyp festgelegt werden.
Wenn Sie Objekte eines anderen Typs exportieren möchten,
müssen Sie dafür ein separates Schema angeben.

#### Dateien

Wählen Sie aus wie Dateien bzw. Dateinamen oder Datei-URLs exportiert werden sollen.
Sie haben drei Optionen:

- Dateinamen nicht exportieren
- Dateinamen exportieren
- Dateinamen mit kompletter URL exportieren

Bei der dritten Option wird jeweils die Datei mit der kompletten URL der aktuellen
Domain und dem Pfad zur Original-Datei exportiert.

### Schema bearbeiten

Hier können Sie die Einstellungen, die Sie beim anlegen des Schemas getätigt haben,
bearbeiten.

### Schema löschen

Hier können Sie das Schema löschen

### Spreadsheet erzeugen

Beim Klick auf die jeweilige Schaltfläche wird die Datei erzeugt und zum Speichern
angeboten.
Es werden immer alle Objekte des jeweiligen Typs exportiert.

## Objekte aus Excel Datei importieren

Der Import erfolgt aus dem XLSX (Excel 2007) Format.

Um Objekte aus einer Excel Datei zu importieren fügen Sie ein Schema hinzu und
erzeugen Sie einen Import für die Datei.
Gehen Sie dazu in der Übersicht auf "Schema hinzufügen & Import erzeugen".

### Schema hinzufügen & Import erzeugen

In diesem ersten Schritt wählen die den zu importierenden Objekttyp aus und laden
eine Excel Datei im XLSX (Excel 2007) Format hoch.

!!! note "Beachten Sie"
    Die erste Zeile Ihrer Datei sollte immer die Spaltennamen enthalten.
    Diese wird bei der Zuordnung der Felder (Field-Matching) ausgelesen und verwendet.
    Die erste Zeile wird niemals als Objekt-Datensatz importiert.

### Feldzuordnung - Field-Matching

In diesem zweiten Schritt setzen Sie die Einstellungen für das Importschema und
ordnen die Spalten der Excel Datei den Metadaten Feldern des Objekttyps zu.

!![Importschema erzeugen - Einstellungen und Feldzuordnung][g2]

#### Einstellungen

##### Name des Importschemas

Geben Sie hier einen beliebigen Namen ein, um das Schema später identifizieren zu können.
Der Name dient dabei nur der internen Erkennung.

##### Import Einstellungen

Hier können Sie aus drei Optionen wählen:

-   Nur Objekte importieren

    Es werden nur die Datensätze aus der hochgeladenen Datei importiert. Das
    Schema wird _nicht_ zur weiteren Verwendung gespeichert.

-   Importschema speichern und Objekte importieren

    Das Schema wird für die weitere Verwendung gespeichert und die Datensätze
    aus der hochgeladenen Datei werden importiert.

-   Nur Importschema speichern
    Das Schema wird für die weitere Verwendung gespeichert. Es werden _keine_
    Daten aus der aktuell hochgeladenen Excel Datei gespeichert.

### Objektfelder und Dublin Core

#### hervorgehoben

Wenn Ihre Excel-Datei eine Spalte für die Objekteigenschaft "hervorgehoben"
enthält, können Sie diese hier angeben.

!!! note "Beachten Sie"
    Die Werte für diese Spalte sollten nur 0 (für nicht hervorgehoben) und
    1 (für hervorgehoben) sein.

#### Dublin Core Titel

Geben Sie hier die Excel-Spalte an, die dem Titel des Objekts entspricht.

!!! warning "Achtung"
    Dieses Feld _muss zugeordnet werden_. Wenn Sie hier keine Zuordnung treffen,
    können Objekte nicht sinnvoll importiert werden, da die Objekte in den
    Übersichten keinen Titel haben.

### Objekttyp - Metadaten

Hier findet die Zuordnung der Excelspalten zu den Metadatenfeldern des Objekttyps
statt. Sie müssen hier nicht alle Felder zuordnen.

#### Inhaltstyp

Zu jedem Feld können Sie den Inhaltstyp auswählen. Dieser bezieht sich auf den
Inhaltstyp in Omeka. Sie können zwischen "text" und "html" wählen. Wählen Sie
"html" wird das Metadatenfeld anschließen in Omeka im WYSIWYG-Editor geladen.



[g1]: img/spreadsheets-001.png  "Spreadsheets Plugin Übersicht"
[g2]: img/spreadsheets-002.png  "Importschema erzeugen - Einstellungen und Feldzuordnung"