# Aufgabe 1:


Die Funktion **print_cow()** soll eine Kuh auf der Konsole ausgeben. Die
Kuh besteht aus mehreren Zeilen, die jeweils ein Teil der Kuh
darstellen.  
Die Funktion soll keine Parameter entgegennehmen. Sie soll die Kuh auf
der Konsole ausgeben.

``` python
def print_cow():
    print("^__^")
    print("(oo)\_______")
    print("(__)\       )\/\/")
    print("    ||----w |")
    print("    ||     ||")

print_cow()
```

    ^__^
    (oo)\_______
    (__)\       )\/\/
        ||----w |
        ||     ||

# Aufgabe 2:

Schreiben Sie ein Unterprogramm **dreiecksFlaeche**, welches die Länge
der Grundseite g und die zugehörige Höhe h übergeben bekommt.  
Das Unterprogramm zeigt in der Konsole die Fläche A=0.5*g*h.  
Testen Sie Ihr Unterprogramm indem Sie es aufrufen.

``` python
def dreiecksFlaeche(g,h):
    flaeche = 0.5*g*h
    print("Die Fläche beträgt: ", flaeche)

dreiecksFlaeche(3,4)
```

    Die Fläche beträgt:  6.0

# Aufgabe 3:

Erstellen Sie eine Funktion, die den jährlichen Zinsbetrag berechnet.
Die Funktion soll die Parameter Kapital und Zinssatz in Prozent haben.

``` python
def zinsbetrag(kapital, zinssatz):
    zins = kapital * zinssatz/100
    print("Der Zinsbetrag beträgt: ", zins, "Euro")

zinsbetrag(1000, 5)
```

    Der Zinsbetrag beträgt:  50.0 Euro
