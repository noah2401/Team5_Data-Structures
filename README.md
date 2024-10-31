**Hier findest du eine kurze Übersicht über die vorgestellten Data Structures:**
---
**List:**


**1.	Merkmale**
  -	Veränderbarkeit (Mutable): Listen können nach ihrer Erstellung verändert werden.
  -	Ordnung:
    -	feste Reihenfolge
    -	auf Element über seinen Index zugreifen (Index beginnt bei 0)
  -	Duplikate erlaubt: 
    -	identische Elemente -> ideal, wenn Sammlung von Werten, die sich wiederholen können
  -	Vielseitige Datentypen: 
    -	z. B. Zahlen, Strings, andere Listen flexibel

**2. Wann solltest du Listen verwenden?**
  -	Dynamische Sammlungen: 
    -	Ideal bei häufigen Änderungen (z. B. Hinzufügen, Entfernen oder Modifizieren von Elementen)
    -	eine einfache Möglichkeit, mit variablen Datenmengen zu arbeiten
  -	Zugriff auf Elemente (Index): 
    -	Schneller Zugriff über den Index der Werte
  -	Feste Reihenfolge
  -	Häufige Iterationen (Durchlaufen): 
    -	Häufige Iterationen einer Sammlung von Elementen (z. B. um sie anzuzeigen oder zu verarbeiten)-> aufgrund ihrer einfachen Syntax und Flexibilität besonders geeignet
  
**3. Besonderheiten der Modellierung**
  -	Erstellung: eckige Klammern
  -	Zugriff auf Elemente: Index
  -	Hinzufügen von Elementen: 
    -	append(), um ein Element am Ende der Liste hinzuzufügen
    -	insert(i,x), um ein Element an einer bestimmten Stelle hinzuzufügen
  -	Entfernen von Elementen:
    -	remove(), um ein spezifisches Element zu entfernen
    -	pop(), um das letzte Element zu entfernen
  -	min(), max(), sum()
  -	Das erste Element x finden: index(x) ->Es gibt eine Fehlermeldung, wenn solch ein Element nicht existiert.
  -	Anzahl von x: count(x)
  -	Sortieren und Umkehren: 
    -	sort(), um die Elemente der Liste im selben Exemplar zu sortieren
    -	reverse(), um die Reihenfolge der Listenelemente im selben Exemplar umzukehren
  -	Slicing: [start:end] ; [start:end:step] ->start inklusive, end exklusive

**4. Anwendungsbeispiele**
  -	To-Do-Listen
  -	Speichern von Benutzereingaben
  -	Kollektionsverwaltung
    -	Liste von Produkten im Einkaufswagen

**5. Benutzung von Listen…**
  -	Als Stack (Stapel):
  -	Als Queue (Schlange):

**6. List Comprehension**
  -	Funktion
  -	Helfen, Listen auf eine elegante und effiziente Weise zu erstellen und zu transformieren
  -	Vorteile von List Comprehensions
    -	Kompaktheit:
      - reduzieren den Codeaufwand 
      -	machen den Code lesbarer
    -	Effizienz: 
      -	List Comprehensions oft schneller als herkömmliche Schleifen -> eine einzige Zeile
      -	Einfache und übersichtliche Codes

**7. Fazit**
  -	Mit Dynamischen, geordnete und veränderbare Daten arbeiten
  -	Flexibilität und einfache Handhabung
  -	Bei großen Datenmengen oder häufige Änderungen an den Anfangs- oder Mittelpositionen der Liste nimmt die Effizienz ab

---

**tuple:**


Auch Tupel stellen eine geordnete Sammlung von Elementen da. Ein Tupel besteht aus mehreren Werten, die durch Kommas voneinander getrennt sind.

**1. Merkmale**
  -	Unveränderlichkeit (Immutable)
  -	Ordnung: 
    -	Die Elemente in einem Tupel sind geordnet-> Reihenfolge der Elemente beim Zugriff wichtig 
  -	Typenvielfalt: 
    -	Elemente unterschiedlicher Datentypen enthalten
    -	Beispielsweise Integer, Float, Strings als auch andere Tupel 
  -	Länge: Die Anzahl der Elemente in einem Tupel ist fest und kann nicht geändert werden.

**2. Wann solltest du Tupel verwenden?**
  Tupel werden in Python häufig verwendet, wenn eine Sammlung von Werten benötigt wird, die nicht verändert werden soll. Sie finden Anwendung in:
  -	Datenstrukturierung: Zum Beispiel können Koordinaten oder RGB-Farbwerte als Tupel dargestellt werden.
  -	Rückgabewerte von Funktionen: Funktionen können mehrere Werte als Tupel zurückgeben, was die Handhabung mehrerer Rückgabewerte vereinfacht.
  -	Datenspeicherung: Tupel können als Schlüssel in Dictionaries verwendet werden, da sie unveränderlich sind.

**3. Anwendungsbeispiele**
  -	Mathematische Tupel: z.B. (x, y, z) für einen Punkt im Raum.
  -	Datenbankmodelle: häufig in Verbindung mit Dictionaries verwendet, um Datensätze zu repräsentieren
  -	Funktionale Programmierung: Gruppierung von Werten
  -	Tuple Comprehension

**4. Allgemein**
  -	ausgegebenen Tupel sind immer von Klammern umgeben, sodass verschachtelte Tupel richtig interpretiert werden
  -	Sie können mit oder ohne Klammern eingegeben werden
  -	Ein spezielles Problem ergibt sich in der Darstellung von Tupeln, die 0 oder 1 Elemente haben: Die Syntax hat ein paar Eigenheiten um das Problem zu lösen
    -	Leere Tupel lassen sich mit einem leeren Klammerpaar darstellen
    -	ein Tupel mit einem Element wird erstellt, indem dem Wert ein Komma nachgestellt wird, es reicht jedoch nicht, das Element nur in Klammern zu schreiben

**5. Fazit**
  -	Unveränderlichkeit und Kombination verschiedener Datentypen -> ideal für viele Anwendungen
  -	Einfache Möglichkeit, Daten zu gruppieren und sicherzustellen, dass diese Daten nicht versehentlich verändert werden
  	
---

**set:**


Eine Menge ist eine ungeordnete Sammlung ohne doppelte Elemente.

**1. Merkmale von Mengen:**
  -	Veränderbarkeit (Mutable)
  -	Eindeutigkeit: Jedes Element in einer Menge ist einzigartig. Duplikate werden automatisch entfernt.
  -	Unordnung: Die Elemente in einer Menge haben keine feste Reihenfolge. Das bedeutet, dass die Elemente nicht durch einen Index angesprochen werden können.

**2. Methoden und Operationen:**
  -	Erstellen einer Menge: 
    -	geschweiften Klammern 
    -	 set()-Funktion
  - Elemente hinzufügen: add() 
  -	Elemente entfernen:
    -	remove() wirft einen Fehler, wenn das Element nicht vorhanden ist
    -	discard() tut dies nicht
  -	Mengenoperationen:
    -	Vereinigung (|)
    -	Schnittmenge (&)
    -	Differenz (-)
    -	symmetrischer Differenz (^)

**3. Wann man Mengen verwenden sollte:**
  -	Eindeutige Werte: 
    -	Duplikate nicht relevant -> z.B. eine Liste von Teilnehmern, um sicherzustellen, dass jeder nur einmal gezählt wird
  -	Schnelle Mitgliedschaftsabfragen: sehr schnelle Möglichkeit, zu überprüfen, ob ein Element vorhanden ist
  -	Mengenoperationen: s.o.

---

**dictionary:**


Dictionaries durch Schlüssel (keys), als die jeder unveränderbare Typ dienen kann, indizierbar
  -	Tupel können als Schlüssel verwendet werden 
  -	Listen können nicht als Schlüssel benutzt werden

**1. Merkmale von Dictionaries:**
  -	Veränderbarkeit (Mutable)
  -	Schlüssel-Wert-Paare: 
    -	besteht aus Schlüsseln und den zugehörigen Werten
    -	Jeder Schlüssel ist eindeutig und wird verwendet, um auf den entsprechenden Wert zuzugreifen
  -	Unordnung:
    -	Keine bestimmte Reihenfolge
    -	Ab Python 3.7 wird jedoch die Einfügereihenfolge beibehalten

**2. Wann man Dictionaries verwenden sollte:**
  -	Assoziative Arrays: Wenn du Daten in Form von Schlüssel-Wert-Paaren speichern möchtest
  -	Schneller Zugriff auf Daten: Dictionaries bieten eine sehr schnelle Möglichkeit, auf Werte zuzugreifen
  -	Strukturierte Daten: Wenn du Daten strukturieren möchtest, z.B. um Objekte mit Eigenschaften darzustellen

**3. Anwendungsbeispiele:**
  -	Der dict()-Konstruktor:  erstellt Dictionaries direkt von Sequenzen von Schlüssel-Wert-Paare
  -	Parre als Schlüsselwort-Argumente 
  -	Benutzerdaten speichern: Informationen über einen Benutzer speichern
  -	Zählungen durchführen: Häufigkeiten zählen, z.B. wie oft jedes Wort in einem Text vorkommt
  -	Konfigurationen speichern: Konfigurationseinstellungen speichern, z.B. in einem Programm oder einer Anwendung
  -	Dict Comprehension
