# Aufgabe: Mietzuschuss


Schreiben Sie ein Programm, das den Mietzuschuss in Abhängigkeit vom
Mietpreis berechnet. Bei einer Miete von weniger als 500,00 Euro beträgt
der Zuschuss 2%. Von 500,00 Euro bis unter 1000,00 Euro beträgt der
Zuschuss 5% und ab 1000,00 Euro erhält man einen Zuschuss von 7%.

``` python
miete = float(input("Bitte Miete eingeben: "))
if miete < 500:
    zuschuss = miete * 0.02    
else:
    if miete < 1000:
        zuschuss = miete * 0.05        
    else:
        zuschuss = miete * 0.07       
print("Der Mietzuschuss beträgt:", zuschuss)
```

    Bitte Miete eingeben:  650

    Der Mietzuschuss beträgt: 32.5

[Struktogramm](Aufgabe-geschachtelte-IF_files/figure-html/47188da7-894f-4398-882f-c7992c414916-1-c30eaec2-50ff-4cf5-8fde-f6bbdc04e077.png)

# Aufgabe: Anmeldung berufliches Gymnasium

In diesem Projekt soll überprüft werden, ob eine Anmeldung mit einem
mittleren Bildungsabschluss an einem beruflichen Gymnasium in
Baden-Württemberg möglich ist oder nicht. Die Bedingungen dafür lauten
wie folgt: Abschlusszeugnis (Mittlerer Bildungsabschluss) der
Realschule, der zweijährigen Berufsfachschule, der Berufsaufbauschule
oder der Werkrealschule mit einem Notendurchschnitt von mindestens 3,0
aus Deutsch, Mathematik und Englisch (kein Fach schlechter als Note
ausreichend).

``` python
note_deutsch = int(input("Deutschnote: "))
note_englisch = int(input("Englischnote: "))
note_mathematik = int(input("Mathematiknote: "))
ist_zugelassen = False

if note_deutsch <= 4:
    if note_englisch <= 4:        
        if note_mathematik <= 4:
            if (note_deutsch + note_englisch + note_mathematik) / 3 <= 3:
                ist_zugelassen = True
if ist_zugelassen == True:
    print("Die Aufnahme ist möglich.")
else:
    print("Aufnahme ist nicht möglich.")
```

    Deutschnote:  3
    Englischnote:  3
    Mathematiknote:  3

    Die Aufnahme ist möglich.

[Struktogramm](Aufgabe-geschachtelte-IF_files/figure-html/846d882d-4333-49f8-975f-42b967bd9197-1-fc429b10-aa07-48dd-ad6f-37b94c1b610d.png)
