# Aufgabe: Fischbestand


Der Fischbestand eines Teichs beträgt zu Beginn eines Jahres drei
Fische. Jedes Jahr verdoppelt sich der Fischbestand. Erstellen Sie ein
Programm, das die Dauer in Jahren ermittelt, bis ein bestimmter, vom
Anwender einzugebender Fischbestand erreicht bzw. überschritten wird.

``` python
jahr = 1
fischzahl = 3
ziel_fischzahl = int(input("Gewünschter Mindest-Fischbestand: "))
while fischzahl < ziel_fischzahl:
    jahr = jahr + 1
    fischzahl = fischzahl * 2
print("Der gewünschte Fischbestand wird im Jahr", jahr, "erreicht.")
```

    Gewünschter Mindest-Fischbestand:  50

    Der gewünschte Fischbestand wird im Jahr 6 erreicht.

[Struktogramm](16-Aufgaben-WHILE_files/figure-html/cell-3-1-42f11b2f-fbe0-460a-a03c-5766dd6be05b.png)

# Aufgabe: Sparbuch

Auf einem Sparbuch wird ein Geldbetrag angelegt. Für diesen Betrag gibt
es einen bestimmten Zinssatz. In diesem Projekt soll überprüft werden,
wie viele Jahre es dauert, bis dieser Betrag einen bestimmten Zielwert
erreicht ober überschreitet. Dabei sollen die Jahresendwerte der
Finanzanlage jeweils ausgegeben werden. (Zinseszinsen nicht vergessen!)

### Programmcode (Python-Code)

``` python
#Hier den Programmcode eingeben und mit STRG+ENTER ausführen
anlagebetrag = float(input("Welcher Betrag soll angelegt werden? "))
zinssatz = float(input("Zu welchem prozentualen Zinssatz wird verzinst? "))
zielwert = float(input("Welcher Zielwert soll erreicht werden? "))
jahr = 0
while anlagebetrag < zielwert:
    anlagebetrag = anlagebetrag * (1 + (zinssatz / 100))
    jahr = jahr + 1
    print("Jahr", jahr, ":", anlagebetrag)
```

    Welcher Betrag soll angelegt werden?  1000
    Zu welchem prozentualen Zinssatz wird verzinst?  2
    Welcher Zielwert soll erreicht werden?  1200

    Jahr 1 : 1020.0
    Jahr 2 : 1040.4
    Jahr 3 : 1061.208
    Jahr 4 : 1082.43216
    Jahr 5 : 1104.0808032
    Jahr 6 : 1126.162419264
    Jahr 7 : 1148.68566764928
    Jahr 8 : 1171.6593810022657
    Jahr 9 : 1195.092568622311
    Jahr 10 : 1218.9944199947574

[Struktogramm](16-Aufgaben-WHILE_files/figure-html/cell-7-1-d5fe2293-6848-4755-a46d-5721d2986012.png)
