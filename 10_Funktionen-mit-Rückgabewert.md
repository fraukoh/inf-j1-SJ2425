# Funktionen mit Rückgabewert


Programmierer können nicht nur Parameter an eine Funktion übergeben,
sondern auch Ergebnisse mit einer Funktion an den Aufrufort
zurückliefern. Diese Ergebnisse heißen Rückgabewerte. Rückgabewerte
können sowohl Zahlen, Zeichenketten als auch Wahrheitswerte sein. Als
Beispiel hier ein Programm, welches das Quadrat einer eingegebenen Zahl
errechnet und ausgibt:

``` python
def berechne_quadratzahl(pZahl):
    quadratzahl = pZahl * pZahl
    return quadratzahl

zahl = float(input("Geben Sie bitte eine Zahl ein: "))
ergebnis = berechne_quadratzahl(zahl)
print("Die Quadratzahl von", zahl, "ist", ergebnis) 
```

    Die Quadratzahl von 4.0 ist 16.0

Die Funktion *berechne_quadratzahl()* empfängt einen Parameter
(*pZahl*). Dieser Parameter wird innerhalb der Funktion mit sich selbst
multipliziert, um die Quadratzahl zu errechnen, und anschließend in der
Variablen quadratzahl gespeichert. Danach kommt das Schlüssel wort
*return* zum Einsatz, welches die Aufgabe hat, den Inhalt der Variablen
quadratzahl an die Stelle zurückzuliefern, von der die Funktion
aufgerufen wurde. Das bedeutet hier, dass der Wert von quadratzahl an
die Variable ergebnis zurückgeliefert und dort abgespeichert wird. Die
Anweisung, mit der Python ein Wert an die aufrufende Stelle
zurückgegeben wird, heißt also *return*.

## Struktogramme

<figure>
<img
src="10_Funktionen-mit-Rückgabewert_files/figure-markdown_strict/cell-5-1-image.png"
alt="image.png" />
<figcaption aria-hidden="true">image.png</figcaption>
</figure>

## Aufgabe:

Erweitern Sie das Programm um eine Funktion
*berechne_QuadratUmfang(pSeitenlaenge)*, die als Parameter die
Seitenlänge empfängt, die von den Benutzern eingegeben wird, daraus den
Umfang des Quadrats berechnet und diesen Wert zurückgibt. Das
Hauptprogramm soll diese Funktion aufrufen und den zurückgegebenen Wert
ausgeben. Die Ausgabe des erweiterten Programms sieht dann so aus:

    Geben Sie eine Zahl ein: 6
    Die Quadratzahl von 6.0 ist 36.0
    Die Seitenlänge eines Quadrats eingeben: 5
    Der Umfang des Quadrats ist: 20.0

``` python
#Hier den Programmcode eingeben und mit STRG+ENTER ausführen
```
