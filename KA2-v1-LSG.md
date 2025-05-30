# Klassenarbeit 2: Einführung in Programmierung mit python


Ihr Name:

## Aufgabe 1: Struktogramm erstellen \[4 P\]

Erstellen Sie ein Struktogramm zu dem folgenden Python-Code

``` python
zahl_x = 4
zahl_y = 2
ergebnis = 100
counter = 1
for i in range(5,10):
    ergebnis = zahl_x + zahl_y ** i
    print("Ergebnis Nr.", counter ,'-',  ergebnis)
    counter = counter + 1
```

Hier soll das Struktogramm als Screenshot eingefügt werden

Korrekturfeld, bitte nicht ändern.

## Aufgabe 2: Struktogramm übersetzen \[6 P\]

Übersetzen Sie das folgende Struktogramm in Python.

<figure>
<img
src="KA2-v1-LSG_files/figure-markdown_strict/494a1ecf-f8fe-499d-8a3a-3d74632f8e09-1-1930ca38-0fe7-41ce-8ac2-ba83cd9e07b1.png"
alt="grafik.png" />
<figcaption aria-hidden="true">grafik.png</figcaption>
</figure>

``` python
# Ihre Lösung bitte hier eintragen
def probe(x):
    erg = x - 2
    print("Ergebnis:", erg)
def test(a, b):
    erg = (a + b) / 2
    return erg
zahl1 = int(input("Erste Zahl: "))
zahl2 = int(input("Zweite Zahl: "))
zwischen = test(zahl1, zahl2)
probe(zwischen)
```

Korrekturfeld, bitte nicht ändern.

## Aufgabe 3: Notenberechnung \[4 P\]

Erstellen Sie ein Python-Programm, das den Benutzer nach den Noten für
drei Fächer fragt und den Durchschnitt berechnet.

Geben Sie eine Nachricht aus, die den Durchschnitt anzeigt und eine
Bewertung basierend auf dem Durchschnitt abgibt.  
Wenn der Durchschnitt kleiner als 4.0 ist, kommt eine Textmeldung “Sie
haben bestanden!”, sonst “Leider nicht bestanden. Viel Erfolg beim
nächsten Mal!”

Erwartete Ausgabe:

    Geben Sie die Note für Fach 1 ein:  2.5
    Geben Sie die Note für Fach 2 ein:  3.0
    Geben Sie die Note für Fach 3 ein:  4.0

    Der Durchschnitt ist: 3.1666666666666665
    Sie haben bestanden!

``` python
# Ihre Lösung bitte hier eintragen
note1 = float(input("Geben Sie die Note für Fach 1 ein: "))
note2 = float(input("Geben Sie die Note für Fach 2 ein: "))
note3 = float(input("Geben Sie die Note für Fach 3 ein: "))

durchschnitt = (note1 + note2 + note3) / 3
print("Der Durchschnitt ist:", durchschnitt)

if durchschnitt < 4.0:
    print("Sie haben bestanden!")
else:
    print("Leider nicht bestanden. Viel Erfolg beim nächsten Mal!")
```

Korrekturfeld, bitte nicht ändern.

## Aufgabe 4: Snack-Bestellung \[6 P\]

Vervollständigen Sie den unten stehenden Code, um den Gesamtpreis für
eine Snack-Bestellung zu berechnen und eine Rechnung auszugeben. Der
Preis für einen Snack beträgt 3 Euro.

Erwartete Ausgabe:

    Geben Sie Ihren Namen ein:  Steffi
    Wie viele Snacks möchten Sie bestellen?  12

    ------------------------------
    Snack-Rechnung für Steffi
    ------------------------------
    Zu zahlender Betrag: 36 €

``` python
def berechne_betrag(preis, menge):
    # Hier fehlt was

def erstelle_rechnung(zahlungsbetrag, name):
    # Hier fehlt was

name = input("Geben Sie Ihren Namen ein: ")
anzahl_snacks = int(input("Wie viele Snacks möchten Sie bestellen? "))
# Hier fehlt was
```

``` python
def berechne_betrag(preis, menge):
    return preis * menge

def erstelle_rechnung(zahlungsbetrag, name):
    print(30 * "-")
    print("Snack-Rechnung für", name)
    print(30 * "-")
    print("Zu zahlender Betrag:", zahlungsbetrag, "€")

name = input("Geben Sie Ihren Namen ein: ")
anzahl_snacks = int(input("Wie viele Snacks möchten Sie bestellen? "))
if anzahl_snacks <= 0:
    print("Bitte geben Sie eine positive Anzahl an Snacks ein.")
else:
    zahlungsbetrag = berechne_betrag(3, anzahl_snacks)
    erstelle_rechnung(zahlungsbetrag, name)
```

Korrekturfeld, bitte nicht ändern.

## Aufgabe 5: Volumen eines Kegels \[4 P\]

Entwickeln Sie ein Python-Programm, das das Volumen (V) eines Kegels
berechnet. Fragen Sie den Benutzer nach dem Radius (r) und der Höhe (h)
des Kegels in cm und verwenden Sie die Formel:
*V* = 1/3 *π* *r*<sup>2</sup> *h*

Überprüfen Sie, ob die Eingaben positiv sind, sonst erscheint die
Textmeldung “Falsche Eingabe. Der Radius und die Höhe müssen positiv
sein.”  
Die Zahl *π* können sie durch 3.14 ersetzen.

Erwartete Ausgabe:

    Geben Sie den Radius des Kegels ein:  3
    Geben Sie die Höhe des Kegels ein:  4

    Das Volumen des Kegels beträgt: 37.68

``` python
# Ihre Lösung bitte hier eintragen
radius = float(input("Geben Sie den Radius des Kegels ein: "))
höhe = float(input("Geben Sie die Höhe des Kegels ein: "))

if radius <= 0 or höhe <= 0:
    print("Falsche Eingabe. Der Radius und die Höhe müssen positiv sein.")
else:
    volumen = (1/3) * 3.14 * radius**2 * höhe
    print("Das Volumen des Kegels beträgt:", volumen)
```

Korrekturfeld, bitte nicht ändern.

## Aufgabe 6: Berechnungstabelle für Quadratzahlen \[6 P\]

Entwickeln Sie ein Programm, das eine Berechnungstabelle für die
Quadratzahlen der ersten n natürlichen Zahlen erstellt. Der Benutzer
gibt n ein, und das Programm gibt eine Tabelle mit den Zahlen und ihren
Quadraten aus.

Erwartete Ausgabe:

    Geben Sie eine positive ganze Zahl ein:  7

    -----------------
    Zahl    Quadrat
    -----------------
    1    1
    2    4
    3    9
    4    16
    5    25
    6    36
    7    49

``` python
# Ihre Lösung bitte hier eintragen
n = int(input("Geben Sie eine positive ganze Zahl ein: "))
print("-----------------")
print("Zahl\tQuadrat")
print("-----------------")
for i in range(1, n + 1):
    quadrat = i ** 2
    print(i,'\t', quadrat)
```

Korrekturfeld, bitte nicht ändern.
