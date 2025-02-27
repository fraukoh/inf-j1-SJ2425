

``` python
# Erstelle eine interessante Aufgabe, in der die Schüler input() verwenden müssen.
# Die Aufgabe sollte so gestaltet sein, dass die Schüler die Eingabe von input() nicht in einer Schleife verwenden müssen.

# In diesem Beispiel wird der Benutzer aufgefordert, eine Zahl einzugeben, und das Programm gibt zurück, ob die Zahl gerade oder ungerade ist.

# Zuerst wird der Benutzer aufgefordert, eine Zahl einzugeben.
zahl = input("Bitte geben Sie eine Zahl ein: ")

# Dann wird die Eingabe in eine Ganzzahl umgewandelt.
zahl = int(zahl)

# Wenn die Zahl modulo 2 gleich 0 ist, ist sie gerade, andernfalls ist sie ungerade.
if zahl % 2 == 0:
    print("Die Zahl ist gerade.")
else:
    print("Die Zahl ist ungerade.")

# Hier ist ein Beispiel für eine mögliche Ausgabe:
# Bitte geben Sie eine Zahl ein: 7
# Die Zahl ist ungerade.

```

``` python
# Generiere bitte eine Aufgabe zu dem Stapelspeicher als Datenstruktur

# In dieser Aufgabe sollen die Schüler eine Liste verwenden, um den Stapelspeicher zu simulieren.
# Der Stapelspeicher ist ein Datenstruktur, die nach dem LIFO-Prinzip (Last In, First Out) funktioniert.
# Die Schüler sollen eine Liste verwenden, um den Stapelspeicher zu simulieren, und die folgenden Operationen durchführen:
# - push(element): Fügt ein Element oben auf den Stapelspeicher hinzu.
# - pop(): Entfernt das oberste Element vom Stapelspeicher und gibt es zurück.

# Hier ist ein Beispiel für die Verwendung des Stapelspeichers:
# stack = []  # Initialisierung des Stapelspeichers
# push(1)  # stack = [1]
# push(2)  # stack = [1, 2]
# push(3)  # stack = [1, 2, 3]
# pop()  # stack = [1, 2], Rückgabe: 3
# pop()  # stack = [1], Rückgabe: 2
# push(4)  # stack = [1, 4]
# pop()  # stack = [1], Rückgabe: 4
# pop()  # stack = [], Rückgabe: 1
```
