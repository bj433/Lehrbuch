# Aufbau von Programmiersprachen

## Programmiersprache und Quelltext
- Formale Sprache zum Abfassen (Formulieren) von Verarbeitungsanweisungen für Rechnersysteme
- Lesbare Beschreibungen = Quelltext/Quellcode/Programmcode

## Bestandteile einer Programmiersprache

### Syntax
- Grammatik einer Programmiersprache
- Beschreibung von Sprachelementen

### Schlüsselwörter
- Bezeichner für Syntaxausdrücke
- Keine Variablen/Funktionen

### Zeichensatz
- Festgelegte alphabetische/numerische Zeichen/Sonderzeichen

### Typische/r Befehlssatz/Grundfunktionen
- Befehle zur Ein-/Ausgabe von Daten
- Befehle zur Deklaration von Variablen und Datenstrukturen
- Funktionen zur Verarbeitung von Zeichenketten
- Mathematische Grundfunktionen
- Kontrollstrukturen für bedingte Ausführung oder wiederholte Ausführung

## Einteilung von Programmiersprachen
- Mögliche Abgrenzungen:
  - Anwendungsgebiete
  - Generationen
  - Programmierparadigmen
 
### Anwendungsgebiete
- Wissenschaftlich-technisch: Fortran, C++, Java
- Kommerziell: COBOL, Java, C#
- Systemsoftware: C, C++
- Spieleprogrammierung: C, C++, C#
- Mobile Apps: Java, Swift, Objective-C
- Webentwicklung: HTML, CSS, JavaScript, PHP
- Anwendungssoftware für PC: C#, Java, Python, C++

### Generationen

#### 1. Generation
- Maschinensprache
- Binärer Code, maschinennahe Programmierung
- Direkte Lauffähigkeit
- Schwer verständlich
- Bspw.: 0001 1010 0011 0100 0001 0000 1101

#### 2. Generation
- Assemblersprache
- Leichter verständliche Symbole (Mnemonics)
- Keine direkte Lauffähigkeit
- Bspw.: mov ds, ax, mov ax, 09h int 21h

#### 3. Generation
- Höhere prozedurale Sprache
- Nähe zu menschlicher Sprache
- Unabhängigkeit von Computersystemen
- Bspw.:

  z1 = 1,5
  
  z2 = 6,3

  summe = float (z1) + float (z2)

  print (summe)

#### 4. Generation
- Sprachen für Datenbanken
- Einsatz für DB-Abfragen, Tabellenkalkulationen
- Bspw.: SELECT * FROM Artikel

#### 5. Generation
- Sprachen der künstlichen Intelligenz
- Nachahmung menschlichen Denkens
- Bspw.:
  f(x) (/
    (+ (* x x ) 3)
    (- a x)))

### Programmierparadigmen
- Grundlegende Konzept einer Programmiersprache
- Grundauffassungen, Methoden und Prinzipien
- Imperative maschinennahe Sprachen: Bspw.: Assembler
- Höhere imperative Sprachen: Bspw.: C, Fortran, COBOL, Pascal
- Objektorientierte Sprachen: Bspw.: C#, Java, Smalltalk
- Deklarative logische Sprachen: Bspw.: Prolog
- Deklarative funktionale Sprachen: Bspw. Lisp, Haskell
