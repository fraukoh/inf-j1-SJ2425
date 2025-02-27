# Aufgabe:


Entwerfen Sie ein Programm, das die Rechenoperationen plus, minus, mal,
geteilt und hoch durchführt.

Definieren Sie dazu zwei Variablen, die Sie für die Berechnungen nutzen
und geben Sie das Ergebnis am Bildschirm aus.

#### Welche Eigenschaften haben die Ausgabedaten? (Variablenliste)

<table>
<thead>
<tr class="header">
<th>Bedeutung</th>
<th>Inhalt</th>
<th>Variablenname</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Erste Zahl</td>
<td>Ganzzahl</td>
<td>zahl1</td>
</tr>
<tr class="even">
<td>Zweite Zahl</td>
<td>Ganzzahl</td>
<td>zahl2</td>
</tr>
<tr class="odd">
<td>Summe</td>
<td>Ganzzahl</td>
<td>addition</td>
</tr>
<tr class="even">
<td>Differenz</td>
<td>Ganzzahl</td>
<td>subtraktion</td>
</tr>
<tr class="odd">
<td>Produkt</td>
<td>Ganzzahl</td>
<td>multiplikation</td>
</tr>
<tr class="even">
<td>Quotient</td>
<td>Kommazahl</td>
<td>division</td>
</tr>
<tr class="odd">
<td>Potenz</td>
<td>Ganzzahl</td>
<td>potenz</td>
</tr>
</tbody>
</table>

``` python
#Hier den Programmcode eingeben und mit STRG+ENTER ausführen
zahl1 = 13
zahl2 = 7

# Durchführen aller Berechnungen:
addition = zahl1 + zahl2
subtraktion = zahl1 - zahl2
multiplikation = zahl1 * zahl2
division = zahl1 / zahl2
potenz = zahl1 ** zahl2

# Ausgabe
# Überschrift
print("Zahl1:", zahl1, "Zahl2:", zahl2) 
print("-------------------")

# Ergebnisse
print("Addition:", addition)
print("Subtraktion:", subtraktion)
print("Multiplikation:", multiplikation)
print("Division:", division)
print("Potenz:", potenz)
```

    Zahl1: 13 Zahl2: 7
    -------------------
    Addition: 20
    Subtraktion: 6
    Multiplikation: 91
    Division: 1.8571428571428572
    Potenz: 62748517

[Struktogramm](05-Rechenoperatoren-Aufgabe-LSG_files/figure-html/cell-5-1-4530a300-3422-4574-ac84-411e12c72975.png)
