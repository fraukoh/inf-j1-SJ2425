# Funktionen in Python


Funktionen sind grundlegende Bausteine in Python, die es ermöglichen,
Code zu strukturieren und wiederzuverwenden. Sie können Parameter
entgegennehmen, Berechnungen durchführen und Werte zurückgeben. Es gibt
verschiedene Arten von Funktionen, abhängig davon, ob sie Parameter
haben und ob sie einen Wert zurückgeben.

## 1. Funktionen mit Parametern und Rückgabewert

Diese Art von Funktion nimmt Parameter entgegen, führt eine Operation
aus und gibt einen Wert zurück.

**Beispiel:**

``` python
def summe(a, b):
    """Gibt die Summe von a und b zurück."""
    erg = a + b
    return erg

# Aufruf der Funktion
ergebnis = summe(5, 3) 
print("Ergebnis:", ergebnis)  # Ausgabe: Ergebnis: 8
```

In diesem Beispiel nimmt die Funktion `summe` zwei Parameter `a` und `b`
entgegen, addiert sie und gibt das Ergebnis zurück.

## 2. Funktionen ohne Parameter, aber mit Rückgabewert

Diese Funktionen nehmen keine Parameter entgegen, führen aber dennoch
eine Operation aus und geben einen Wert zurück.

**Beispiel:**

``` python
def get_pi():
    """Gibt den Wert von Pi zurück."""
    return 3.14159

# Aufruf der Funktion
pi_wert = get_pi()
print("Pi:", pi_wert)  # Ausgabe: Pi: 3.14159
```

Die Funktion `get_pi` nimmt keine Parameter entgegen, gibt aber den Wert
von Pi zurück.

## 3. Funktionen mit Parametern, aber ohne Rückgabewert

Diese Funktionen nehmen Parameter entgegen, führen eine Operation aus,
geben aber keinen expliziten Wert zurück. Sie werden oft verwendet, um
Seiteneffekte zu erzeugen, z.B. Ausgaben auf der Konsole.

**Beispiel:**

``` python
def differenz(a, b):
    """Berechnet die Differenz von a und b und gibt das Ergebnis aus."""
    erg = a - b
    print("Ergebnis:", erg)

# Aufruf der Funktion
differenz(10, 4)  # Ausgabe: Ergebnis: 6
```

Die Funktion `differenz` nimmt zwei Parameter entgegen, berechnet die
Differenz, gibt das Ergebnis aber nicht mit `return` zurück, sondern
gibt es direkt aus.

## 4. Funktionen ohne Parameter und ohne Rückgabewert

Diese Funktionen nehmen keine Parameter entgegen und geben auch keinen
Wert zurück. Sie werden oft verwendet, um eine bestimmte Aktion
auszuführen.

**Beispiel:**

``` python
def gruesse():
    """Gibt eine Begrüßung aus."""
    print("Hey Du!")

# Aufruf der Funktion
gruesse()  # Ausgabe: Hey Du!
```

Die Funktion `gruesse` nimmt keine Parameter entgegen und gibt keinen
Wert zurück, sondern gibt einfach eine Begrüßung aus.

Diese Beispiele verdeutlichen die verschiedenen Arten von Funktionen in
Python und wie sie je nach Bedarf eingesetzt werden können.

# Übung:

Bestimmen Sie für jede der folgenden Funktionen: \* Ob sie Parameter hat
(ja/nein) \* Ob sie einen Rückgabewert hat (ja/nein)

## Aufgabe 1

``` python
def begruessung():
    print("Willkommen zum Python-Kurs!")
```

## Aufgabe 2

``` python

def würfel():
    import random
    return random.randint(1, 6)
```

## Aufgabe 3

``` python

def addiere(a, b):
    summe = a + b
    print(f"Die Summe ist: {summe}")
```

## Aufgabe 4

``` python

def berechne_flaeche(länge, breite):
    return länge * breite
```

## Aufgabe 5

``` python

def zeige_uhrzeit():
    from datetime import datetime
    print(datetime.now().strftime("%H:%M:%S"))
```

## Aufgabe 6

``` python

def generiere_zufallsname():
    namen = ["Anna", "Max", "Lisa", "Tom"]
    import random
    return random.choice(namen)
```

## Aufgabe 7

``` python

def drucke_info(name, alter, stadt):
    print(f"{name} ist {alter} Jahre alt und wohnt in {stadt}.")
```

## Aufgabe 8

``` python

def ist_volljährig(alter):
    return alter >= 18
```

## Aufgabe 9

``` python

def alarm():
    for i in range(3):
        print("ALARM!")
```

## Aufgabe 10

``` python

def berechne_note(punkte, maximalpunkte):
    prozent = (punkte / maximalpunkte) * 100
    return f"Note: {prozent:.1f}%"
```

## Lösungen

<details>
<summary>
Klicke hier um die Lösungen anzuzeigen
</summary>

    > Begruessung:   
        Parameter: nein   
        Rückgabewert: nein   
        

    > Würfel:   
        Parameter: nein   
        Rückgabewert: ja   


    > Addiere:   
        Parameter: ja   
        Rückgabewert: nein   
        

    > Berechne_flaeche:
        Parameter: ja
        Rückgabewert: ja


    > Zeige_uhrzeit:
        Parameter: nein
        Rückgabewert: nein

    > Generiere_zufallsname:
        Parameter: nein
        Rückgabewert: ja

    > Drucke_info:
        Parameter: ja
        Rückgabewert: nein

    > Ist_volljährig:
        Parameter: ja
        Rückgabewert: ja

    > Alarm:
        Parameter: nein
        Rückgabewert: nein

    > Berechne_note:
        Parameter: ja
        Rückgabewert: ja

</details>
