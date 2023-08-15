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
- Verknüpfung miteinander
- Bspw.:

SELECT ... FROM Land L INNER JOIN Kontinent K ON

L.KontinentID = K.KontinentID

### LEFT JOIN
- Angabe verknüpfter Werte aus linker und rechter Tabelle
- Verknüpfung mit linker Tabelle
- Bspw.:

SELECT ... FROM Land L LEFT JOIN Kontinent K ON

L.KontinentID = K.KontinentID

### RIGHT JOIN
- Angabe verknüpfter Werte aus linker und rechter Tabelle
- Verknüpfung mit rechter Tabelle
- Bspw.:

SELECT ... FROM Land L RIGHT JOIN Kontinent K ON

L.KontinentID = K.KontinentID

### FULL JOIN
- Angabe aller Werte aus beiden Tabellen
- Keine Abhängigkeit von Verknüpfungen
- Bspw.:

SELECT ... FROM Land L FULL JOIN Kontinent K ON

L.KontinentID = K.KontinentID

## Kombinieren von Abfragemengen

### Syntax
SELECT Spaltenname FROM TabellennameA

UNION

SELECT Spaltenname FROM TabellennameB;

### Erläuterung
- Spaltenname = Name der Spalte in Tabelle A/Tabelle B
- TabellennameA/B = Name der Tabelle

### Beispiel
SELECT O.Name FROM Ort O

UNION

SELECT L.Name FROM Land L;

## Unterabfragen
- Sub-Selects
- Einbindung von SQL-Anweisungen in andere SQL-Anweisungen
- 2. Select in runden Klammern
- Vergleichsoperatoren verwendbar für einzelne Rückgabewerte
- Mengenoperatoren verwendbar für mehrere Rückgabewerte
- ORDER BY und UNION nicht zulässig
 
### Mengenoperatoren
- IN = Prüfung nach Wert innerhalb eines Subselects
- ALL = Prüfung nach erfüllter Bedingung für alle Ergebnisse eines Subselects
- ANY = Prüfung nach erfüllter Bedingung für beliebiges Ergebnis eines Subselects
- EXISTS = Prüfung ob Subselect überhaupt ein Ergebnis hat
