# Aufgabe:


Schreiben Sie ein Programm, das den Umfang und den Flächeninhalt eines
Rechtecks berechnet. Der Benutzer gibt dazu die Länge und die Breite des
Rechtecks ein. Das Programm berechnet die Ergebnisse und gibt diese aus.

#### Welche Eigenschaften haben die Ausgabedaten? (Variablenliste)

<table>
<thead>
<tr class="header">
<th>Bedeutung</th>
<th>Typ</th>
<th>Variable</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Eingabe: Länge in cm</td>
<td>Dezimalzahl</td>
<td>laenge</td>
</tr>
<tr class="even">
<td>Eingabe: Breite in cm</td>
<td>Dezimalzahl</td>
<td>breite</td>
</tr>
<tr class="odd">
<td>Berechnung und Ausgabe: Umfang in cm</td>
<td>Dezimalzahl</td>
<td>umfang</td>
</tr>
<tr class="even">
<td>Berechnung und Ausgabe: Fläche in cm2</td>
<td>Dezimalzahl</td>
<td>flaeche</td>
</tr>
</tbody>
</table>

### Programmcode (Python-Code)

``` python
#Hier den Programmcode eingeben und mit STRG+ENTER ausführen
laenge = float(input("Länge des Rechtecks: "))
breite = float(input("Breite des Rechtecks: "))
umfang = 2 * (laenge + breite)
flaeche = laenge * breite
print("Der Umfang des Rechtecks beträgt: ", umfang, "cm")
print("Die Fläche des Rechtecks beträgt: ", flaeche, "cm^2")
```

[Struktogramm](072-Aufgabe-LSG_files/figure-html/cell-5-1-0065b9a4-c3c3-4a47-b5d6-1e25ff919686.png)
