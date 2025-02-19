# Aufgabe:


Bei den bisherigen Programmen waren alle Werte fest vom Programmcode
vorgegeben. Es bestand keine Möglichkeit für die Programmbenutzer,
selber Werte in das Programm einzugeben. Diese Option wird jetzt
gezeigt. Schreiben Sie dazu ein Programm, das den Inhalt einer
Kreisfläche berechnet. Der Benutzer soll den Radius im Programm auf
Aufforderung eingeben. Das Programm errechnet die passende Kreisfläche
und gibt das Ergebnis aus.

Formel: *F* = *r*<sup>2</sup>*π*

*F*-Fläche, *r*-Radius.

#### Welche Eigenschaften haben die Ausgabedaten? (Variablenliste)

<table>
<thead>
<tr class="header">
<th>Bedeutung</th>
<th>Datentyp</th>
<th>Variable</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Eingabe: Radius in cm</td>
<td>Dezimalzahl</td>
<td>radius</td>
</tr>
<tr class="even">
<td>Verarbeitung: Kreiszahl Pi</td>
<td>Dezimalzahl</td>
<td>pi</td>
</tr>
<tr class="odd">
<td>Berechnung und Ausgabe: Fläche in cm2</td>
<td>Dezimalzahl</td>
<td>flaeche</td>
</tr>
</tbody>
</table>

### Programmcode (Python-Code)

``` python
#Hier den Programmcode eingeben und mit STRG+ENTER ausführen
radius = float(input("Bitte Radius eingeben: "))
pi = 3.14
flaeche = radius * radius * pi
print("Der Inhalt der Kreisfläche beträgt:", flaeche)
```

    Bitte Radius eingeben:  10
    Der Inhalt der Kreisfläche beträgt: 314.0

[Struktogramm](071-Aufgabe-LSG_files/figure-html/cell-5-1-14852b0b-3637-4bd1-987c-2e4af82390a5.png)
