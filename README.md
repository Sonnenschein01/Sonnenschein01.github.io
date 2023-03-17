
# Datenbanken: 

## Was ist das überhaupt? 
### Ein Leihe würde sagen: Etwas worin Daten gespeichert werden. 


#### Die Definition zeigt, dass es etwas genauer ist: 

Eine Datenbank ist ein System zur elektronischen Datenverwaltung. Die wesentliche Aufgabe einer Datenbank ist es, große Datenmengen effizient, widerspruchsfrei und dauerhaft zu speichern und benötigte Teilmengen in unterschiedlichen, bedarfsgerechten Darstellungsformen für Benutzer und Anwendungsprogramme bereitzustellen. 
Das heißt, es geht grob gesagt nicht nur um das Speichern von Datensätzen in Datenbanken an sich, sondern auch um andere Kriterien, wie zum Beispiel Konsistenz und Darstellung. 

#### Datensatz? Datenbank? Was sind die Unterschiede? 

| Name           |     Beschreibung
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------- 
| Bit            | Kleinste im Computer verarbeitbare Dateneinheit                                                                                    
| Byte           | Bildung festgelegter Bitfolgen                                                                                                     
| Datenelement   | Gruppierung von einem oder mehreren Zeichen in einem Wort, einer Gruppe von Wörtern oder einer Zahl, z.B. Artikelname oder -nummer.
| Datensatz      | Gruppe von inhaltlich zusammenhängenden Datenelementen, die verschiedene Eigenschaften desselben Phänomens beschreiben             
| Datei          | Zusammenfassung logisch zusammengehörender, gleichartiger Datensätze                                                               
| Datenbank      | Gruppen von Dateien, zwischen denen logische Abhängigkeiten bestehen                                                               

#### Wozu braucht man diese Datenhierarchie denn?

* Wir versuchen Informationen, Beziehungen und Personen aus der echten Welt in Form von Daten festzuhalten und dadurch eine Struktur zu erstellen und die Beziehungen zueinander darzustellen.

---

# ER-Modell 

#### Wie kann man die erwähnten Entitäten und Relationen, die in der realen Welt vorhanden sind verständlich veranschaulichen?  

* ER-Modellierung (ERM) wurde dafür geschaffen. ER heißt Entity Relationship.
* Damit erstellen wir ER-Diagramme (ERD). 

## ER-Modellierung (ERM) Begriffe 

* Entity heißt **Entität** und bedeutet so viel wie „Ein existierendes Ding“. Eine Entität definiert sich und unterscheidet sich von anderen Entitäten durch die Eigenschaften, die sie besitzt.                                                     
***Beispiel:** Maren und Dennis sind Schüler, die unterschiedliche Namen und somit unterschiedliche Eigenschaften besitzen. Sie können also nicht dieselbe Entität sein und können somit identifiziert/unterschieden werden.*




* Die Eigenschaften der Entitäten nennt man in diesem Fall **Attribute** und sie werden durch Werte angegeben. Sie können eine Entität oder auch eine Relation beschreiben.                                           
***Beispiel:** Anzahl, Name, Klasse, Alter.*                                                                                                     


* Die **Werte** sind primitive Datenelemente, die direkt darstellbar sind. Alle Attribute der Entitäten werden mit Werten angegeben.       
***Beispiel:** int (Zahl) für das Alter, String (Zeichenkette) für den Namen*                                                                            


* **Entitätstypen** fassen alle gleichartigen Entitäten zusammen. Sie funktionieren als Blaupause oder Schablone um alle Entitäten einer Art zusammen abzuspeichern und zu strukturieren.                                                          
***Beispiel:** Schüler und Lehrer sind zwei Entitätstypen, mit denen wir jetzt jede Entität aus einer Schulklasse einem Entitätstypen zuordnen können. 1 = Schüler 2 = Lehrer*                                                                        

 

* Relationship aus dem Begriff Entity-Relationship steht für die **Relation**, also Beziehung. Die Entitäten können also einen Bezug zueinander haben und hängen somit zusammen.                                                                               
***Beispiel:** Es gibt den Lehrer Herr Volk und dieser unterrichtet die Schüler Paul und Jan, was auch ihre Beziehung zu ihm beschreibt.* 

 

* **Primärschlüssel** sind Attribute, die es kein zweites Mal geben darf und somit eindeutig eine Entität Identifizieren. Oft kommen IDs mit dieser Rolle zum Einsatz, welche selbst erstellte Primärschlüssel sind. (Auch mehrere Attribute zusammen können einen Primärschlüssel bilden, sofern sie die Bedingung erfüllen, dass es sie in dieser Kombination nur einmal gibt.)                                             
***Beispiel:** Zwei Schüler heißen Alex, aber einer hat die ID 69 und der andere 420.*                                        

 

* Die **Kardinalität** ist die Anzahl an Entitäten die an einer Relation Teilnehmen, da sich diese Zahl je nach Relation unterscheiden kann. Es gibt 1:1, 1:n, m:n Beziehungen. Bei 0…n muss eine Entität nicht zu einer Relation gehören. Das nennt sich auch Optionalität.        
***Beispiel:** In einer Klasse sind 20 Schüler, sodass eine Relation von Klasse zu Schülern mit der Kardinalität von 1:20 besteht. Jeder Schüler ist einer Klasse zugeordnet aber mehrere Klassen sind nicht einem Schüler zugeordnet.*                            

#### Jetzt da diese Begriffe der ER-Modellierung bekannt sind können wir mit diesen ER-Diagramme erstellen



## ER-Diagramme (ERD)  

1. Entitätstypen werden als Rechtecke dargestellt. Im Rechteck steht der Name des Entitätstyps.  

2. Attribute werden als Ovale dargestellt, die mit einer Linie mit dem Entitätstyp verbunden sind, zu dem sie gehören. Im Oval steht der Name des Attributs.  

3. Die Namen von Primärschlüsseln werden unterstrichen.  

4. Relationen werden als Rauten dargestellt, die jeweils mit einer Linie mit den beteiligten Entitätstypen verbunden sind. In der Raute steht der Name der Relation.  

5. An den Verbindungslinien von Relationen werden die Kardinalitäten notiert.  

6. Entitäten werden nicht dargestellt. 

____

### Beispiele für ER-Diagramme: 

!['Image1'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/erstesbsp.png "Beispiel 1")

* *Beispiel 1:* 

Jedes Album besitzt eine AlbumNr, einen Titel und einen Preis.  
AlbumNr ist der Primärschlüssel mit dem jedes Album eindeutig identifiziert werden kann. 

!['Image2'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/zweitesbsp.png "Beispiel 2")

* *Beispiel 2:* 

Jeder Mensch hat eine eindeutige Steuernummer (Primärschlüssel), einen Vornamen, einen Nachnamen und ein Geburtsdatum.  

Jeder Finger hat einen eindeutigen Abdruck und eine Länge.  

Zudem hat jeder einzelne Mensch zwischen 0 und n Finger (Kardinalität 0..n).  

Jeder einzelne Finger hat aber nur genau einen Menschen (Kardinalität 1) 

Hat ist die Beziehung, die die Entitäten zueinander haben. In diesem Fall hat sie keine Attribute.


---


# Relationenmodell

Das Stichwort Relational findet sich auch hier wieder. Nicht nur in der realen Welt und in der abstrahierten Abbildung der ER-Diagramme, sondern auch in Form von Tabellen ist es relevant. In dieser Tabellenform werden nämlich die Relationen abgespeichert, die wir mithilfe eines ER-Diagramms darstellen. 

Laut Definition ist eine **relationale Datenbank** eine digitale Datenbank, die zur elektronischen Datenverwaltung dient und auf einem tabellenbasierten relationalen Datenbankmodell beruht. Grundlage des Konzeptes relationaler Datenbanken ist die Relation. Sie stellt eine mathematische Beschreibung einer Tabelle dar.

Operationen auf diesen Relationen werden durch die relationale Algebra bestimmt. 

## Grundlegendes Konzept: 

Eine relationale Datenbank kann man sich als eine Sammlung von Tabellen *(den Relationen)* vorstellen, in welchen Datensätze abgespeichert sind. Jede Zeile in einer Tabelle ist ein Datensatz und stellt in unserem Fall eine Entität dar. Jede Zeile besteht aus einer Reihe von Attributwerten *(Attribute = Eigenschaften)*, den Spalten der Tabelle. Die Anzahl und der Typ der Attribute für eine Relation nennt man Relationenschema. Das Bild illustriert die Relation **R** mit Attributen ***A**1* bis ***A**n* in den Spalten. 

!['Image3'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/drittesbsp.png "Beispiel 3")

*Beispiel:*

**Schüler**

**Schüler-ID** | Name           | Klasse
 ---           | ---            | ---
 69            | Maxi Malost    | 10
 420           | Mario Ahner    | 11
 42            | Max Mustermann | 12

In diesem Beispiel heißt die Relation Schüler und stellt somit den Entitätstypen dar.                                                
Das Relationenschema besteht aus drei Attributen, die verschiedene Werttypen haben.                                                    
Schüler-ID ist der Primärschlüssel und daher als Attribut hier dick geschrieben. In der korrekten Syntax wird es aber unterstrichen.     
Jede Zeile stellt somit einen Schüler mit seinen Eigenschaften dar. Alle sind in der Relation ‘Schüler’.                              

Jetzt wissen wir in welcher Form eine relationale Datenbank die Relationen abspeichert. Diesen tabellarischen Zustand wollen wir nun erreichen. Das erstellte ER-Diagramm kann man nun in diese Tabellen umwandeln. 

---

# Transformation 

Für das Umwandeln von ER-Diagrammen in eine Relation in Form einer Tabelle gibt es bestimmte Regeln:  

1. Jeder Entitätstyp wird als Tabelle dargestellt. Jede Tabelle benötigt einen Primärschlüssel.  

2. Jede n:m-Beziehung wird durch eine eigene Tabelle dargestellt.  

3. Jede 1:n- und 1:1-Beziehung mit eigenen Attributen wird wie bei Regel 2 durch eine eigene Tabelle dargestellt.  

4. Jede 1:n-Beziehung ohne eigene Attribute wird so dargestellt, dass der Primärschlüssel des 1-Entitätstyps Fremdschlüssel des n-Entitätstyps wird.  

5. Jede 1:1-Beziehung ohne eigene Attribute wird so dargestellt, dass der Primärschlüssel des ersten Entitätstyps beim zweiten Entitätstyp Primär- und Fremdschlüssel zugleich wird.  

6. Sind Regel 4 oder 5 nicht anwendbar, dann wird für die Beziehung eine gesonderte Tabelle angelegt. 

---

* Auf den ersten Blick ist das viel, aber nun gehen wir anhand dieses Beispiels zusammen durch:

1. Jeder Entitätstyp ist eine eigene Tabelle mit einem Primärschlüssel. Optimalerweise ist der Primärschlüssel ein einzelnes Attribut. Im Zweifel wird ein künstlicher Primärschlüssel zugewiesen, wie z.B eine ID. Jede Zeile einer Tabelle ist eine Entität des Entitätstyps.

!['Image4'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/viertesbsp.png "Beispiel 4")

* Aufteilen wie in 1. beschrieben:

!['Image4.2'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/viertesbsp2.png "Beispiel 4 Teil 2")

!['Pfeil'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/pfeil.png "Pfeil")

**Mensch**

Steuernummer | Vorname | Nachname | Geburtsdatum
----         | ---     | ---      | ----
17           | Petra   | Silie    | 28.2.2005
42           | Angela  | Merkel   | 17.7.1954

### &

!['Image4.3'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/viertesbsp3.png)

!['Pfeil'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/pfeil.png "Pfeil")

**Kurs**

Nummer | Fach
---    | ----
1      | Mathematik
2      | Informatik

* Die Relationen werden also aufgeteilt. Das macht man je nach Kardinalität unterschiedlich:

2. m:n-Kardinalitäten erfordern eine zusätzliche Tabelle für die Relation. (Das erstellen der Tabelle für die Entitätstypen (Hier: Schüler und Kurs) wurden schon in Regel 1 erklärt.) In der zusätzlichen Tabelle gibt es eine Spalte für jeden Primärschlüssel der beteiligten Entitätstypen. Primärschlüssel, die in einer „fremden“ Tabelle auftauchen, nennt man dort Fremdschlüssel. 

!['Image5'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/fuenftesbsp.png)

In diesem Beispiel besucht Schüler Nr. 23 in realität zwei Kurse. 

!['Image5'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/fuenftesbsp2.png)

!['Image5'](https://raw.githubusercontent.com/Sonnenschein01/Sonnenschein01.github.io/main/pfeil.png)

**Besucht**

Schüler-Nr. | Kurs-Nr. 
---         | ---
17          | 1
23          | 1
23          | 2
