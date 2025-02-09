# Aufgabe:


Schreiben Sie ein Programm, das die Daten eines Schülers in mehreren
Variablen speichert und hinterher ausgibt.

Zu speichern sind: Nachname, Vorname, Alter, Notendurchschnitt, zweite
Fremdsprache(True/False) und Musik (True/False).

Diese Daten sollen dann im Browser ausgegeben werden.

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
<td>Name</td>
<td>Zeichenkette</td>
<td>nachname</td>
</tr>
<tr class="even">
<td>Vorname</td>
<td>Zeichenkette</td>
<td>vorname</td>
</tr>
<tr class="odd">
<td>Alter</td>
<td>Ganzzahl</td>
<td>alter</td>
</tr>
<tr class="even">
<td>Notendurchschnitt</td>
<td>Dezimalzahl</td>
<td>schnitt</td>
</tr>
<tr class="odd">
<td>zweite Fremdsprache</td>
<td>Wahrheitswert</td>
<td>zweit_fremd</td>
</tr>
<tr class="even">
<td>Musik</td>
<td>Wahrheitswert</td>
<td>musik</td>
</tr>
</tbody>
</table>

``` python
#Hier den Programmcode eingeben und mit STRG+ENTER ausführen
# Deklaration und Initialisierung der Variablen:
nachname = "Mustermann" 
vorname = "Max"
alter = 17
schnitt = 1.8
zweit_fremd = True
musik = False

# Ausgabe:
print("Name:", vorname, nachname)
print("Alter:", alter)
print("Notenschnitt:", schnitt)
print("2. Fremdsprache belegt:", zweit_fremd)
print("Musik belegt:", musik)
```

    Name: Max Mustermann
    Alter: 17
    Notenschnitt: 1.8
    2. Fremdsprache belegt: True
    Musik belegt: False

[Struktogramm](04-Variablen-Aufgabe-LSG_files/figure-html/cell-5-1-fef6123d-ef1e-49ec-9dc6-793eded87502.png)
