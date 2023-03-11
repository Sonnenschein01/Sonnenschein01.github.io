# Sonnenschein01.github.io

# Header1
## H2
### H3
#### H4
##### H5
###### H6

Alternatively, for H1 and H2, an underline-ish style:

Alt-H1
======

Alt-H2
------

Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~

1. First ordered list item
2. Another item
⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses

[I'm an inline-style link](https://www.google.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes 
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

Here's our logo (hover to see the title text):

Inline-style: 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Reference-style: 
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"

Inline `code` has `back-ticks around` it.

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
 
```python
s = "Python syntax highlighting"
print s
```
 
```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].  

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.  
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    This footnote also has been made with a different syntax using 4 spaces for new lines.
    
    Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 

<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

Three or more...

---

Hyphens

***

Asterisks

___

Underscores

Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

This line is also a separate paragraph, but...
This line is only separated by a single newline, so it's a separate line in the *same paragraph*.

Youtube Videos können so verlinkt werden, aber abspielen geht auf der Website nicht

<a href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
" target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

...oder mit Markdown Text verlinken

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](http://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)



# Datenbanken: 

### Was ist das überhaupt? 

#### Ein Leihe würde sagen: Etwas worin Daten gespeichert werden. 

 

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

##### Wozu braucht man diese Datenhierarchie denn?

* Wir versuchen Informationen, Beziehungen und Personen aus der echten Welt in Form von Daten festzuhalten und dadurch eine Struktur zu erstellen und die Beziehungen zueinander darzustellen.

____

# ER-Modell 

##### Wie kann man die erwähnten Entitäten und Relationen, die in der realen Welt vorhanden sind verständlich veranschaulichen?  

* ER-Modellierung wurde dafür geschaffen. ER heißt Entity Relationship.
* Damit erstellen wir ER-Diagramme. 

## ER-Modellierung (ERM) Begriffe 

Entity heißt **Entität** und bedeutet so viel wie „Ein existierendes Ding“. Eine Entität definiert sich und unterscheidet sich von anderen Entitäten durch die Eigenschaften, die sie besitzt.  

Beispiel: Maren und Dennis sind Schüler, die unterschiedliche Namen und somit unterschiedliche Eigenschaften besitzen. Sie können also nicht dieselbe Entität sein und können somit identifiziert/unterschieden werden. 




Die Eigenschaften der Entitäten nennt man in diesem Fall **Attribute** und sie werden durch Werte angegeben. Sie können eine Entität oder auch eine Relation beschreiben. 

Beispiel: Anzahl, Name, Klasse, Alter 


Die **Werte** sind primitive Datenelemente, die direkt darstellbar sind. Alle Attribute der Entitäten werden mit Werten angegeben. 

Beispiel: int (Zahl) für das Alter, String (Zeichenkette) für den Namen 

 

**Entitätstypen** fassen alle gleichartigen Entitäten zusammen. Sie funktionieren als Blaupause oder Schablone um alle Entitäten einer Art zusammen abzuspeichern und zu strukturieren. 

Beispiel: Schüler und Lehrer sind zwei Entitätstypen, mit denen wir jetzt jede Entität aus einer Schulklasse einem Entitätstypen zuordnen können. 1 = Schüler 2 = Lehrer 

 

Relationship aus dem Begriff Entity-Relationship steht für die **Relation**, also Beziehung. Die Entitäten können also einen Bezug zueinander haben und hängen somit zusammen. 

Beispiel: Es gibt den Lehrer Herr Volk und dieser unterrichtet die Schüler Paul und Jan, was auch ihre Beziehung zu ihm beschreibt.  

 

**Primärschlüssel** sind Attribute, die es kein zweites Mal geben darf und somit eindeutig eine Entität Identifizieren. Oft kommen IDs mit dieser Rolle zum Einsatz, welche selbst erstellte Primärschlüssel sind. (Auch mehrere Attribute zusammen können einen Primärschlüssel bilden, sofern sie die Bedingung erfüllen, dass es sie in dieser Kombination nur einmal gibt.) 

Beispiel: Zwei Schüler heißen Alex, aber einer hat die ID 69 und der andere 420. 

 

Die **Kardinalität** ist die Anzahl an Entitäten die an einer Relation Teilnehmen, da sich diese Zahl je nach Relation unterscheiden kann. Es gibt 1:1, 1:n, m:n Beziehungen. Bei 0…n muss eine Entität nicht zu einer Relation gehören. Das nennt sich auch Optionalität. 

Beispiel: In einer Klasse sind 20 Schüler, sodass eine Relation von Klasse zu Schülern mit der Kardinalität von 1:20 besteht. Jeder Schüler ist einer Klasse zugeordnet aber mehrere Klassen sind nicht einem Schüler zugeordnet. 
