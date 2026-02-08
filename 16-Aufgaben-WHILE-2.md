# Aufgabe: Die Schildkröten-Rettung

Eine kleine Schildkröte will einen Fluss überqueren. Sie schafft pro Tag nur einen Meter, aber der Fluss ist 12 Meter breit. Leider rutscht sie jede Nacht im Schlaf einen Meter zurück, außer am letzten Tag, wenn sie das Ziel erreicht. Schreibe ein Programm, das berechnet, wie viele Tage die Schildkröte braucht, um das andere Ufer zu erreichen.

```python
flussbreite = 12
position = 0
tage = 0
while position < flussbreite:
    tage = tage + 1
    position = position + 1
    print("Tag", tage, ": Die Schildkröte ist bei Meter", position)
    if position < flussbreite:
        position = position - 1
        print("Oh nein! In der Nacht ist sie auf Meter", position, "zurückgerutscht.")
print("Geschafft! Nach", tage, "Tagen ist die Schildkröte am anderen Ufer.")
```

# Aufgabe: Der Hausaufgaben-Zauberer

Du hast einen magischen Stift, der jeden Tag eine deiner Hausaufgaben erledigt. Leider zaubert er manchmal eine neue dazu, wenn du nicht aufpasst! Schreibe ein Programm, das zählt, wie viele Tage du brauchst, bis alle Hausaufgaben erledigt sind. Am Anfang hast du 5 Hausaufgaben. Jeden zweiten Tag kommt eine neue dazu.

```python
hausaufgaben = 5
tage = 0
while hausaufgaben > 0:
    tage = tage + 1
    print("Tag", tage, ": Noch", hausaufgaben, "Hausaufgaben übrig.")
    hausaufgaben = hausaufgaben - 1
    if tage % 2 == 0:
        print("Oh nein, der Stift hat eine neue Hausaufgabe gezaubert!")
        hausaufgaben = hausaufgaben + 1
print("Hurra! Nach", tage, "Tagen sind alle Hausaufgaben erledigt!")
```

# Aufgabe: Der schlafende Wecker

Du hast einen Wecker, der dich jeden Morgen fragt, ob du aufstehen willst. Du bist aber sehr müde und drückst immer wieder auf "Snooze" (Schlummertaste). Schreibe ein Programm, das so lange "Noch 5 Minuten..." ausgibt, bis du "ja" (also aufstehen) eingibst.

```python
antwort = "nein"
versuche = 0
while antwort != "ja":
    versuche = versuche + 1
    print("Noch 5 Minuten...")
    antwort = input("Willst du jetzt aufstehen? (ja/nein): ")
print("Super! Nach", versuche, "Snooze-Runden bist du endlich aufgestanden!")
``` 