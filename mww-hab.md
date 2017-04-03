# Objekttyp MWW-HAB - besondere Metadaten-Felder

Bei der Befüllung der Metadatenfelder des Objekttyps für Exponate (MWW-HAB) zu beachten:

## Verknüpfung mit Normdaten

Personennamen und Orte werden mit den Normdatensätzen der GND verküpft. Dazu wird der Name/Ortsname eingegeben und mit dem GND-Normdatensatz verlinkt.
Beispiel: [Wittenberg](http://d-nb.info/gnd/4066640-2)

Dies betrifft die Felder:
- Verfasser / Künstler / Schaffende 
- Person Erscheinungsort / Entstehungsort
- Drucker
- Erscheinungsort / Entstehungsort

## Kontrollierte Vokabulare

Die bei einigen Feldern eingebundenen Dropdown-Listen können über den Menüpunkt "Einfache Vokabeln" editiert werden. Vorsicht: Änderungen an den Auswahllisten - z.B. Umbenennungen - wirken sich nicht auf bereits über die Auswahllisten Einträge in das betreffende Metadatenfeld aus. Der Listeneintrag steht bei diesen zuvor bearbeiteten Objekten in seiner alten Form in der Datenbank und muss ggf. nachträglich geändert werden. 


### Signatur

Bei Werken, die in einem Online-Katalog verzeichnet sind, wird die Signaturangabe mit dem OPAC-Eintrag verlinkt.
Beispiel: [A: 151.31 Theol. (5)](https://opac.lbs-braunschweig.gbv.de/DB=2/SET=4/TTL=1/CMD?ACT=SRCHA&IKT=1016&SRT=YOP&TRM=ppn+151603960)

Entsprechendes gilt für die Felder
- Bibliografischer Nachweis
- Katalogeintrag
- Link

### Ausstellungssektion

Das System befüllt dieses Feld programmatisch.

//relevant??

Der Eintrag identifiziert die Sektion, in der das betreffende Objekt eingebunden ist. Der Link muss als relativer Link (ohne Domain) eingegeben werden, und zwar als einfacher Texte **ohne Verlinkung**. Beispiel: /exhibits/show/luther-die-marke#page19

Um den Link zu erhalten 




