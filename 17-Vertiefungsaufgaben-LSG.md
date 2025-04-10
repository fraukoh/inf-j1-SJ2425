# Aufgabe 1


Erstellen Sie ein Programm, das solange nach einem PIN-Code fragt, bis
die PIN richtig eingegeben wird. Nach der richtigen Eingabe erscheint
eine Meldung „Ihnen werden 1000 EUR überwiesen“

``` python
#Hier den Programmcode eingeben und mit STRG+ENTER ausführen
pin_richtig = 1234
pin_benutzer = int(input("Bitte Ihren PIN-Code eingeben"))

while pin_richtig != pin_benutzer:
    print("Ihre PIN ist leider falsch.")
    pin_benutzer = int(input("Bitte Ihren PIN-Code eingeben"))
    
print("Ihnen werden 1000 EUR überwiesen")
```

    Bitte Ihren PIN-Code eingeben 1234

    Ihnen werden 1000 EUR überwiesen

# Aufgabe 2

Erstellen Sie ein Programm mit dem Namen `ratemal`. Dieses Programm
erzeugt eine Zufallszahl im Bereich (1,100). Der Benutzer des Programms
soll diese Zahl mit möglichst wenigen Versuchen raten. Nach jedem
Versuch bekommt der Benutzer die Information, ob die geratene Zahl
größer, kleiner oder gleich der gesuchten Zahl ist.

HINWEIS: Eine Zufallszahl (z) im Bereich (u,o) kann man mit folgendem
Befehl erzeugen:

``` python
import random #aktiviert das random-Modul
z=random.randint(u,o) #erzeugt eine ganzzahlige Zufallszahl zwischen u und o
```

``` python
#Hier den Programmcode eingeben und mit STRG+ENTER ausführen
import random 
z=random.randint(1,100)
z_benutzer = int(input("Bitte eine Zahl eingeben:"))
while z != z_benutzer:
    if z > z_benutzer:
        print("Die Zahl ist kleiner")
    else: 
        print("Die Zahl ist größer")
print("Gewonnen!")
```

### Aufgabe 2.1

Wie viele Versuche hat der Benutzer gebraucht, um die Zahl zu erraten?
Programmieren Sie die Ausgabe von Anzahl der Versuche.

# Aufgabe 3

3n+1 – Problem (Achterbahnzahlen):  
Die 1. Zahl einer Zahlenreihe ist ein gegebener Startwert (=n)  
Die jeweils nächste Zahl wird aus der letzten Zahl gemäß folgender Regel
gebildet:  
Falls die letzte Zahl gerade war, wird sie durch 2 geteilt. Das Ergebnis
ist dann die nächste Zahl.  
Falls die letzte Zahl ungerade war, wird sie mit 3 multipliziert und
anschließend 1 addiert. Das Ergebnis ist dann die nächste Zahl.

> **Beispiel: n=5** 1) 5-ungerade 3*5+1=16  
> 2) 16-gerade 16/2=8  
> 3) 8-gerade 8/2=4  
> 4) 4-gerade 4/2=2  
> 5) 2-gerade 2/2=1  
> 6) 1-ungerade 3*1+1=4  
> usw.

Erstellen Sie eine Funktion achterbahn(n), die diese Zahlenfolge
berechnet.  
Limitieren Sie die Iterationszahl (z.B. iz=100).

``` python
def achterbahn(n):
    zahlen = [n]
    iz = 100
    for i in range(iz):
        if zahlen[len(zahlen)-1] % 2 == 0:
            zahlen.append(zahlen[len(zahlen)-1] / 2)
        else:
            zahlen.append(zahlen[len(zahlen)-1] * 3 + 1)
    return zahlen

achterbahn(200)
```

    [200,
     100.0,
     50.0,
     25.0,
     76.0,
     38.0,
     19.0,
     58.0,
     29.0,
     88.0,
     44.0,
     22.0,
     11.0,
     34.0,
     17.0,
     52.0,
     26.0,
     13.0,
     40.0,
     20.0,
     10.0,
     5.0,
     16.0,
     8.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0,
     1.0,
     4.0,
     2.0]
