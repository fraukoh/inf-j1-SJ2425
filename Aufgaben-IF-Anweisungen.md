# Aufgabe: Abikarten


In diesem Projekt soll überprüft werden, welcher Betrag zu zahlen ist,
wenn eine Karte für den Abiball 30,00 Euro kostet und für Bestellungen
von drei oder mehr Karten ein Rabatt von 20% gewährt wird.

``` python
print(40*"-")
print("Berechnung des Preises für Abikarten")
print(40*"-")
anzahl = int(input("Anzahl der gewünschten Karten: "))
betrag = anzahl * 30
if anzahl > 2:
    betrag = betrag * 0.8
print("Der Preis für die Karten beträgt:", betrag, "€")
```

    ----------------------------------------
    Berechnung des Preises für Abikarten
    ----------------------------------------
    Der Preis für die Karten beträgt: 72.0 €

    Anzahl der gewünschten Karten:  3

[Struktogramm](Aufgaben-IF-Anweisungen_files/figure-html/4878a343-73e8-4b42-b283-2c196d26c7fb-1-27c2663d-54e3-4b42-93d9-5c5971e7d510.png)

# Aufgabe: Prüfung, ob der Mindestpreis erreicht ist

In diesem Projekt können Gebote für einen zum Kauf angebotenen Artikel
abgegeben werden. In dem Programmcode ist der Mindestpreis (hier 24.99)
hinterlegt. Ist der von dem Anwender vorgeschlagene Kaufpreis geringer,
wird der Text „Ihr Angebotspreis liegt unterhalb des Mindestpreises!“
ausgegeben. Andernfalls erscheint der Text „Herzlichen Glückwunsch, Sie
haben den Artikel erworben!“.

``` python
preis = float(input("Wieviel wollen Sie zahlen? "))
if preis < 24.99:
    print("Ihr Angebotspreis liegt unterhalb des Mindestpreises!")
else:
    print("Herzlichen Glückwunsch, Sie haben den Artikel erworben!")
```

    Wieviel wollen Sie zahlen?  24.98

    Ihr Angebotspreis liegt unterhalb des Mindestpreises!

[Struktogramm](Aufgaben-IF-Anweisungen_files/figure-html/5ca320c2-a775-4f76-bb6e-2566e99a9762-1-4e6bc43c-615b-4121-8888-5be4594f7bb5.png)
