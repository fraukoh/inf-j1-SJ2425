# Aufgabe -Verzweigung mit logischen Operatoren (UND):


In diesem Projekt soll überprüft werden, ob eine Anmeldung zur
Führerscheinprüfung möglich ist oder nicht. Die Bedingung für eine
Zulassung lautet wie folgt: Der Fahrschüler muss mindestens 17 Jahre alt
sein und mindestens 16 Theoriestunden absolviert haben.

``` python
alter = int(input("Bitte Alter eingeben: "))
stunden = int(input("Bitte Anzahl der Theoriestunden eingeben: "))
if stunden > 15 and alter > 16:
    print("Sie sind zur Prüfung zugelassen.")
else:
    print("Sie sind nicht zur Prüfung zugelassen.") 
```

    Bitte Alter eingeben:  17
    Bitte Anzahl der Theoriestunden eingeben:  5

    Sie sind nicht zur Prüfung zugelassen.

[Struktogramm](Aufgaben-verknuepfte-Bedingungen_files/figure-html/a392f0ca-0625-460a-9947-4d1efed2e36d-1-1f922415-49b8-4e8c-a29a-93e3b3099a8e.png)

# Aufgabe - Verzweigung mit verknüpften Bedingungen (ODER):

In diesem Projekt soll überprüft werden, ob ein Besucher eines Tierparks
ein Kind (bis 12 Jahre) oder ein Senior (ab 60 Jahre) ist. Kinder und
Senioren zahlen 8,00 Euro Eintritt, für alle anderen beträgt der
Eintrittspreis 12,00 Euro.

``` python
alter = int(input("Bitte Alter eingeben: "))
if alter <= 12 or alter >= 60:
    print("Der Eintrittspreis beträgt 8,00 €")
else:
    print("Der Eintrittspreis beträgt 12,00 €")
```

    Bitte Alter eingeben:  59

    Der Eintrittspreis beträgt 12,00 €

[Struktogramm](Aufgaben-verknuepfte-Bedingungen_files/figure-html/103c87b1-d83e-4b90-a10a-58078e136ec4-1-daf87717-c3a6-49f1-925b-d794048bbb1a.png)

# Aufgabe - Verzweigung mit logischen Operatoren (NICHT):

Die Firma Rent A Car in Stuttgart vermietet Oldtimer für 50,00 € pro
Tag. Alle Kunden, die nicht in Stuttgart wohnen, erhalten einen
Sonderrabatt von 10%. Das Projekt soll nach Eingabe des Wohnorts und der
Mietdauer die Mietkosten ermitteln und anzeigen.

``` python
ort = input("Bitte den Wohnort eingeben: ")
mietdauer = int(input("Bitte Mietdauer (in Tagen) eingeben: "))
kosten = mietdauer * 50
if not ort == "Stuttgart":
    kosten = kosten * 0.9
print("Der Mietpreis beträgt:", kosten)
```

    Bitte den Wohnort eingeben:  Tübingen
    Bitte Mietdauer (in Tagen) eingeben:  3

    Der Mietpreis beträgt: 135.0

[Struktogramm](Aufgaben-verknuepfte-Bedingungen_files/figure-html/2fdb6219-efc8-44ea-999e-3a1fda6b5520-1-c505e6c5-5d7d-4c2d-9638-5311dbd27d6b.png)
