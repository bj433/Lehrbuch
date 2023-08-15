# Anweisungen in SQL

### Anlegen und Löschen einer Datenbank
- CREATE DATABASE ...
- DROP DATABASE ...

### Anlegen, Ändern und Löschen von Tabellen
- CREATE TABLE ...
- ALTER TABLE ... (ADD, MODIFY, DROP)
- DROP TABLE ...

### Einfügen, Ändern und Löschen von Datensätzen
- INSERT INTO ...
- UPDATE ...
- DELETE ...

### Abfragen von Daten, Aggregatfunktionen, Vergleichs-, Rechen- und Logische Operatoren
- SELECT ... FROM ... WHERE ...
- LIKE ...
- ORDER BY ...
- GROUP BY ...
- MIN
- MAX
- SUM
- COUNT
- AVG
- NULL

## Joins/Anfragen über mehrere Tabellen

### INNER JOIN
- Angabe verknüpfter Werte aus linker und rechter Tabelle
- Bspw.:
SELECT ... FROM Land L INNER JOIN Kontinent K ON

L.KontinentID = K.KontinentID

### LEFT JOIN
