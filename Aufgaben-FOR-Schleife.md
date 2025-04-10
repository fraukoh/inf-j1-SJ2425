# Aufgabe: Taschengeld


Schreiben Sie ein Programm, das den Betrag des Taschengelds in
Abhängigkeit vom Alter ausgibt. Das Taschengeld wird vom 6. bis zum 21.
Lebensjahr ausgezahlt. Dabei sind der Anfangsbetrag und die jährliche
Erhöhung vom Benutzer einzugeben.

``` python
taschengeld = float(input("Wie hoch ist das erste Taschengeld? "))
erhoehung = float(input("Jährliche Erhöhung des Taschengelds: "))
for alter in range(6, 22):
    print("Alter", alter, ":", taschengeld, "€")
    taschengeld = taschengeld + erhoehung
```

    Wie hoch ist das erste Taschengeld?  1
    Jährliche Erhöhung des Taschengelds:  2

    Alter 6 : 1.0 €
    Alter 7 : 3.0 €
    Alter 8 : 5.0 €
    Alter 9 : 7.0 €
    Alter 10 : 9.0 €
    Alter 11 : 11.0 €
    Alter 12 : 13.0 €
    Alter 13 : 15.0 €
    Alter 14 : 17.0 €
    Alter 15 : 19.0 €
    Alter 16 : 21.0 €
    Alter 17 : 23.0 €
    Alter 18 : 25.0 €
    Alter 19 : 27.0 €
    Alter 20 : 29.0 €
    Alter 21 : 31.0 €

[Struktogramm](Aufgaben-FOR-Schleife_files/figure-html/cell-3-1-73ce9ef3-dce1-4ce2-8bd9-d26b1369a823.png)

# Aufgabe: Finanzplan

In diesem Projekt soll überprüft werden, welchen Zielwert eine
Finanzanlage, die zu einem bestimmten Zinssatz für eine bestimme
Anlagedauer (in Jahren) durch Zinseszins-Vermehrung erreicht. Für jedes
Jahr, die die Finanzanlage läuft, soll der Wert am Ende des Jahres
ausgegeben werden.

``` python
#Hier den Programmcode eingeben und mit STRG+ENTER ausführen
betrag = float(input("Betrag: "))
zinssatz = float(input("Zinssatz: "))
jahre = int(input("Laufzeit in Jahren: "))
for jahr in range(1, jahre + 1):
    betrag = betrag * (1 + zinssatz/100)
    print ("Jahr", jahr, ":", betrag)
```

    Betrag:  10000
    Zinssatz:  2
    Laufzeit in Jahren:  4

    Jahr 1 : 10200.0
    Jahr 2 : 10404.0
    Jahr 3 : 10612.08
    Jahr 4 : 10824.3216

[Struktogramm](Aufgaben-FOR-Schleife_files/figure-html/cell-6-1-7f26a608-7491-4820-8e65-6ad00bfea030.png)

# Aufgabe: Smartphone-Akku

Erstelle ein Programm, das simuliert, wie sich der Akkustand eines
Smartphones über 10 Stunden entlädt. Der Startakkustand und die
stündliche Entladung in Prozent sollen eingegeben werden.

``` python
akku = int(input("Aktueller Akkustand in %? "))
entladung = int(input("Entladung pro Stunde in %? "))
for stunde in range(1, 11):
    akku = akku - entladung
    print("Nach", stunde, "Stunden:", akku, "%")
```

    Aktueller Akkustand in %?  90
    Entladung pro Stunde in %?  3

    Nach 1 Stunden: 87 %
    Nach 2 Stunden: 84 %
    Nach 3 Stunden: 81 %
    Nach 4 Stunden: 78 %
    Nach 5 Stunden: 75 %
    Nach 6 Stunden: 72 %
    Nach 7 Stunden: 69 %
    Nach 8 Stunden: 66 %
    Nach 9 Stunden: 63 %
    Nach 10 Stunden: 60 %

[Struktogramm](Aufgaben-FOR-Schleife_files/figure-html/cell-9-1-38c3f38a-1839-4c83-9026-d5f53c927a13.png)

# Aufgabe: TikTok-Follower

Schreibe ein Programm, das berechnet, wie viele Follower ein
TikTok-Account nach einer Woche hat, wenn täglich neue dazukommen. Die
Anfangszahl und die täglichen neuen Follower sollen eingegeben werden.

``` python
follower = int(input("Aktuelle Followerzahl? "))
neue = int(input("Neue Follower pro Tag? "))
for tag in range(1, 8):
    follower = follower + neue
    print("Tag", tag, ":", follower, "Follower")
```

    Aktuelle Followerzahl?  550
    Neue Follower pro Tag?  15

    Tag 1 : 565 Follower
    Tag 2 : 580 Follower
    Tag 3 : 595 Follower
    Tag 4 : 610 Follower
    Tag 5 : 625 Follower
    Tag 6 : 640 Follower
    Tag 7 : 655 Follower

[Struktogramm](Aufgaben-FOR-Schleife_files/figure-html/cell-12-1-17423e08-e6c0-4083-9b9d-2e678c553f0e.png)

# Aufgabe: Süßigkeiten-Rechner

Erstelle ein Programm, das berechnet, wie viele Süßigkeiten du in einer
Woche isst. Gib die Anzahl der täglichen Süßigkeiten ein und lass dir
für 7 Tage die Gesamtsumme anzeigen.

``` python
gesamt = 0
taeglich = int(input("Wie viele Süßigkeiten isst du pro Tag? "))
for tag in range(1, 8):
    gesamt = gesamt + taeglich
    print("Nach", tag, "Tagen:", gesamt, "Süßigkeiten")
```

    Wie viele Süßigkeiten isst du pro Tag?  3

    Nach 1 Tagen: 3 Süßigkeiten
    Nach 2 Tagen: 6 Süßigkeiten
    Nach 3 Tagen: 9 Süßigkeiten
    Nach 4 Tagen: 12 Süßigkeiten
    Nach 5 Tagen: 15 Süßigkeiten
    Nach 6 Tagen: 18 Süßigkeiten
    Nach 7 Tagen: 21 Süßigkeiten

[Struktogramm](Aufgaben-FOR-Schleife_files/figure-html/cell-15-1-edc130e7-9327-4bc4-a0a3-6eb9a2ca8f58.png)
