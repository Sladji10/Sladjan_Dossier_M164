## Auftrag Bulkimport 

Mysql bietet die Möglichkeit CSV-Files effizient und schnell in eine Tabelle mit gleichen Spalten einzulesen.

Das Kommando dazu heist ***LOAD DATA INFILE "/path/file.csv"***

Mit diesem Kommando, versucht MariaDB Server, die Eingabedatei aus seinem eigenen Dateisystem zu lesen. 
Ohne Pfadangabe sucht der Server die Datei im Data-Verzeichnis der aktuellen Datenbasis: ***C:\...\mySQL\data\db\***

***LOAD DATA LOCAL INFILE "c:\\path\\file.csv***

Wenn Sie dagegen diese Anweisung ausführen, versucht der Client, die Eingabedatei aus seinem Dateisystem zu lesen, und sendet den Inhalt der Eingabedatei an den MariaDB Server. Auf diese Weise können Sie Dateien aus dem lokalen Dateisystem des Clients in die Datenbank laden.
