# Aufgabe: Reisezeit-Rechner


Sie sollen einen Reisezeit-Rechner programmieren, der für eine bestimmte
Strecke und Geschwindigkeit die benötigte Reisezeit berechnet und
ausgibt.

1.  Erstellen Sie dafür: eine Funktionberechne_reisezeit(strecke,
    geschwindigkeit), die: Als Parameter die zurückzulegende Strecke in
    Kilometern und die Durchschnittsgeschwindigkeit in km/h
    entgegennimmt Die Reisezeit in Stunden berechnet (Strecke geteilt
    durch Geschwindigkeit) Die berechnete Zeit als Dezimalwert (z.B.
    3.125 Stunden) zurückgibt

2.  Testen Sie Ihre Funktionen mit folgenden Werten: Strecke: 250 km
    Geschwindigkeit: 80 km/h

Ihr Programm soll zum Schluss eine benutzerfreundliche Meldung ausgeben:
`"Für eine Strecke von 250 km mit 80 km/h benötigen Sie: 3.125 Stunden"`

``` python
def berechne_reisezeit(strecke, geschwindigkeit):
    zeit = strecke / geschwindigkeit
    return zeit

# Demonstration
strecke_km = 250
geschwindigkeit_kmh = 80
reisezeit = berechne_reisezeit(strecke_km, geschwindigkeit_kmh)

print("Für eine Strecke von", strecke_km,  "km mit", geschwindigkeit_kmh, "km/h", "benötigen Sie:", reisezeit, "Stunden")
```

    Für eine Strecke von 250 km mit 80 km/h benötigen Sie: 3.125 Stunden

[Struktogramm](Aufgaben-Funktionen-mit-Rueckgabewert_files/figure-html/cell-3-1-image.png)

# Aufgabe: Online-Shop Endpreisberechnung

Sie sollen für einen Online-Shop eine Funktion programmieren, die den
Endpreis eines Artikels berechnet. Der Endpreis setzt sich zusammen aus
dem ursprünglichen Artikelpreis, einem prozentualen Rabatt und den
Versandkosten.

1.  Erstellen Sie eine Funktion namens berechne_endpreis, die drei
    Parameter annimmt: preis: Der ursprüngliche Artikelpreis in Euro
    rabatt_prozent: Der Rabatt in Prozent (z.B. 15 für 15%)
    versandkosten: Die Versandkosten in Euro
2.  In der Funktion sollen Sie: Den Rabattbetrag in Euro berechnen
    (Preis × Rabatt-Prozent / 100) Den Endpreis berechnen (Preis -
    Rabattbetrag + Versandkosten) und zurückgeben
3.  Testen Sie Ihre Funktion mit folgenden Werten: Artikelpreis: 79.99 €
    Rabatt: 15% Versandkosten: 12.50 €
4.  Geben Sie den berechneten Endpreis mit der Nachricht “Endpreis mit
    Versand:” aus.

``` python
def berechne_endpreis(preis, rabatt_prozent, versandkosten):
    rabatt_betrag = preis * rabatt_prozent / 100
    return preis - rabatt_betrag + versandkosten

# Demonstration
artikel_preis = 79.99
rabatt = 15  # 15% Rabatt
versandkosten = 12.50

endpreis = berechne_endpreis(artikel_preis, rabatt, versandkosten)
print("Endpreis mit Versand:", endpreis, "€")
```

    Endpreis mit Versand: 80.4915 €

[Struktogramm](Aufgaben-Funktionen-mit-Rueckgabewert_files/figure-html/cell-6-1-image.png)

# Aufgabe: Münzwert-Rechner

Sie sollen einen Münzwert-Rechner für Euro-Münzen programmieren. Der
Rechner soll den Gesamtwert einer Münzsammlung berechnen, die aus
1-Cent-, 2-Cent-, 5-Cent-, 10-Cent-, 20-Cent- und 50-Cent-Münzen
besteht.

1.  Erstellen Sie eine Funktion berechne_gesamtwert, die: Sechs
    Parameter entgegennimmt: die Anzahl der jeweiligen Münzen
    (anzahl_1c, anzahl_2c, anzahl_5c, anzahl_10c, anzahl_20c,
    anzahl_50c) Den Wert jeder Münzart in Cent berechnet Alle Werte
    addiert, um den Gesamtwert in Cent zu ermitteln Den Gesamtwert in
    Cent zurückgibt

2.  Testen Sie Ihre Funktion mit folgenden Werten:  
    10 Stück 1-Cent-Münzen  
    5 Stück 2-Cent-Münzen  
    3 Stück 5-Cent-Münzen  
    2 Stück 10-Cent-Münzen  
    1 Stück 20-Cent-Münzen  
    2 Stück 50-Cent-Münzen

3.  Geben Sie das Ergebnis in Euro aus (Cent-Wert / 100).

``` python
def berechne_gesamtwert(anzahl_1c, anzahl_2c, anzahl_5c, anzahl_10c, anzahl_20c, anzahl_50c):
    wert_1c = anzahl_1c
    wert_2c = anzahl_2c * 2
    wert_5c = anzahl_5c * 5
    wert_10c = anzahl_10c * 10
    wert_20c = anzahl_10c * 20
    wert_50c = anzahl_10c * 50

    gesamtwert = wert_1c + wert_2c + wert_5c + wert_10c + wert_20c + wert_50c
    
    return gesamtwert


gesamt_cent = berechne_gesamtwert(10, 5, 3, 2, 1, 2)
print("Der Gesamtwert Ihrer Münzsammlung beträgt:", gesamt_cent/100 , "Euro")
```

    Der Gesamtwert Ihrer Münzsammlung beträgt: 1.95 Euro

[Struktogramm](Aufgaben-Funktionen-mit-Rueckgabewert_files/figure-html/cell-9-1-image.png)

# Aufgabe: Notenpunkte-Umrechner für die gymnasiale Oberstufe

Sie sollen einen Notenpunkte-Umrechner für die gymnasiale Oberstufe
programmieren. In der Oberstufe werden Leistungen sowohl mit klassischen
Schulnoten (1,0 bis 6,0) als auch mit Punkten (15 bis 0) bewertet.

Ihr Programm soll beide Umrechnungsrichtungen ermöglichen.

Erstellen Sie zwei Funktionen:

1.  Die Funktion note_zu_punkte(note), die: Als Parameter eine
    klassische Schulnote (z.B. 1,0 / 2,3 / 3,7) entgegennimmt Diese Note
    in das entsprechende Punktesystem der Oberstufe umrechnet Die
    berechneten Punkte zurückgibt
2.  Die Funktion punkte_zu_note(punkte), die: Als Parameter eine
    Punktzahl (z.B. 15 / 10 / 5) entgegennimmt Diese Punkte in eine
    klassische Schulnote umrechnet Die berechnete Note zurückgibt

Die Umrechnungsformel für die erste Funktion lautet:
`15 - (note - 1) * 3` Umrechnungsformel für die zweite Funktion lautet:
`1 + (15 - punkte) / 3`

Führen Sie Ihre Funktionen mit folgenden Werten aus:

> Umrechnung der Noten 2,0 und 3,7 in Punkte  
> Umrechnung von 10 Punkten in eine Note

Ihr Programm soll für jede Umrechnung eine informative Ausgabe liefern.

``` python
def note_zu_punkte(note):
    return 15 - (note - 1) * 3

def punkte_zu_note(punkte):
    return 1 + (15 - punkte) / 3

# Demonstration
note1 = 2.0
note2 = 3.7

punkte1 = note_zu_punkte(note1)
punkte2 = note_zu_punkte(note2)

print("Die Note", note1, "entspricht", punkte1, "Punkten")
print("Die Note", note2, "entspricht", punkte2, "Punkten")

punkte_test = 10
note_test = punkte_zu_note(punkte_test)
print("Die Punkte", punkte_test, "entsprechen der Note", note_test)
```

    Die Note 2.0 entspricht 12.0 Punkten
    Die Note 3.7 entspricht 6.899999999999999 Punkten
    Die Punkte 10 entsprechen der Note 2.666666666666667

[Struktogramm](Aufgaben-Funktionen-mit-Rueckgabewert_files/figure-html/cell-12-1-image.png)
