

``` python
 %load_ext sql
```

``` python
%sql sqlite:///buecherei.db
```

``` python
%%sql
-- Erstellen der Tabelle Autoren
CREATE TABLE Autoren (
    AutorID INTEGER PRIMARY KEY,
    Name TEXT NOT NULL,
    Geburtsjahr INTEGER
);

-- Erstellen der Tabelle Kategorien
CREATE TABLE Kategorien (
    KategorieID INTEGER PRIMARY KEY,
    Bezeichnung TEXT NOT NULL
);

-- Erstellen der Tabelle Bücher
CREATE TABLE Bücher (
    BuchID INTEGER PRIMARY KEY,
    Titel TEXT NOT NULL,
    AutorID INTEGER,
    KategorieID INTEGER,
    FOREIGN KEY (AutorID) REFERENCES Autoren(AutorID),
    FOREIGN KEY (KategorieID) REFERENCES Kategorien(KategorieID)
);

-- Erstellen der Tabelle Ausleihen
CREATE TABLE Ausleihen (
    AusleihID INTEGER PRIMARY KEY,
    BuchID INTEGER,
    Ausleihdatum DATE,
    Rückgabedatum DATE,
    FOREIGN KEY (BuchID) REFERENCES Bücher(BuchID)
);
```

       sqlite://
     * sqlite:///buecherei.db
    (sqlite3.OperationalError) table Autoren already exists
    [SQL: -- Erstellen der Tabelle Autoren
    CREATE TABLE Autoren (
        AutorID INTEGER PRIMARY KEY,
        Name TEXT NOT NULL,
        Geburtsjahr INTEGER
    );]
    (Background on this error at: https://sqlalche.me/e/20/e3q8)

``` python
%%sql
-- Einfügen von Autoren
INSERT INTO Autoren (Name, Geburtsjahr) VALUES
('Max Mustermann', 1980),
('Erika Musterfrau', 1975),
('Hans Müller', 1990),
('Anna Schmidt', 1985),
('Peter Meier', 1978),
('Julia Becker', 1992),
('Thomas Wagner', 1983),
('Laura Schneider', 1987),
('Michael Fischer', 1981),
('Sophie Weber', 1995),
('Daniel Hoffmann', 1984),
('Lisa Koch', 1991),
('Markus Richter', 1979),
('Nina Braun', 1986),
('Felix Klein', 1993),
('Clara Zimmermann', 1982),
('Tobias Hartmann', 1988),
('Sarah Peters', 1994),
('Jan Schwarz', 1989),
('Leonie Weiß', 1996);

-- Einfügen von Kategorien
INSERT INTO Kategorien (Bezeichnung) VALUES
('Fiktion'),
('Sachbuch'),
('Fantasy'),
('Science Fiction'),
('Biografie'),
('Romantik'),
('Thriller'),
('Kinderbuch'),
('Historischer Roman'),
('Krimi'),
('Gesundheit'),
('Reise'),
('Kochen'),
('Technologie'),
('Philosophie'),
('Psychologie'),
('Natur'),
('Sport'),
('Kunst'),
('Musik');

-- Einfügen von Büchern
INSERT INTO Bücher (Titel, AutorID, KategorieID) VALUES
('Das Geheimnis der alten Bibliothek', 1, 1),
('Die Kunst des Kochens', 2, 13),
('Die Reise ins Ungewisse', 3, 12),
('Der letzte Wunsch', 4, 3),
('Die Biografie eines Lebens', 5, 5),
('Die Schatten der Vergangenheit', 6, 1),
('Die Magie der Sterne', 7, 4),
('Die Macht der Gedanken', 8, 16),
('Die Welt der Technik', 9, 14),
('Die Farben der Natur', 10, 17),
('Die Geheimnisse der Psychologie', 11, 15),
('Die Abenteuer des kleinen Prinzen', 12, 8),
('Die Geschichte der Menschheit', 13, 2),
('Die Liebe in Zeiten der Cholera', 14, 6),
('Die Entdeckung der Langsamkeit', 15, 1),
('Die Philosophie des Glücks', 16, 18),
('Die Geheimnisse der alten Meister', 17, 19),
('Die Welt der Musik', 18, 20),
('Die Zukunft der Menschheit', 19, 4),
('Die Reise durch die Zeit', 20, 3);

-- Einfügen von Ausleihen
INSERT INTO Ausleihen (BuchID, Ausleihdatum, Rückgabedatum) VALUES
(1, '2024-01-01', '2024-01-15'),
(2, '2024-01-05', '2024-01-20'),
(3, '2024-01-10', '2024-01-25'),
(4, '2024-01-15', '2024-01-30'),
(5, '2024-01-20', '2024-02-05'),
(6, '2024-01-25', '2024-02-10'),
(7, '2024-02-01', '2024-02-15'),
(8, '2024-02-05', '2024-02-20'),
(9, '2024-02-10', '2024-02-25'),
(10, '2024-02-15', '2024-03-01'),
(11, '2024-02-20', '2024-03-05'),
(12, '2024-02-25', '2024-03-10'),
(13, '2024-03-01', '2024-03-15'),
(14, '2024-03-05', '2024-03-20'),
(15, '2024-03-10', '2024-03-25'),
(16, '2024-03-15', '2024-03-30'),
(17, '2024-03-20', '2024-04-05'),
(18, '2024-03-25', '2024-04-10'),
(19, '2024-04-01', '2024-04-15'),
(20, '2024-04-05', '2024-04-20');
```

       sqlite://
     * sqlite:///buecherei.db
    20 rows affected.
    20 rows affected.
    20 rows affected.
    20 rows affected.

    []

``` python
%%sql
SELECT * FROM Autoren;
```

       sqlite://
     * sqlite:///buecherei.db
    Done.

<table data-quarto-postprocess="true">
<thead>
<tr class="header">
<th data-quarto-table-cell-role="th">AutorID</th>
<th data-quarto-table-cell-role="th">Name</th>
<th data-quarto-table-cell-role="th">Geburtsjahr</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1</td>
<td>Max Mustermann</td>
<td>1980</td>
</tr>
<tr class="even">
<td>2</td>
<td>Erika Musterfrau</td>
<td>1975</td>
</tr>
<tr class="odd">
<td>3</td>
<td>Hans Müller</td>
<td>1990</td>
</tr>
<tr class="even">
<td>4</td>
<td>Anna Schmidt</td>
<td>1985</td>
</tr>
<tr class="odd">
<td>5</td>
<td>Peter Meier</td>
<td>1978</td>
</tr>
<tr class="even">
<td>6</td>
<td>Julia Becker</td>
<td>1992</td>
</tr>
<tr class="odd">
<td>7</td>
<td>Thomas Wagner</td>
<td>1983</td>
</tr>
<tr class="even">
<td>8</td>
<td>Laura Schneider</td>
<td>1987</td>
</tr>
<tr class="odd">
<td>9</td>
<td>Michael Fischer</td>
<td>1981</td>
</tr>
<tr class="even">
<td>10</td>
<td>Sophie Weber</td>
<td>1995</td>
</tr>
<tr class="odd">
<td>11</td>
<td>Daniel Hoffmann</td>
<td>1984</td>
</tr>
<tr class="even">
<td>12</td>
<td>Lisa Koch</td>
<td>1991</td>
</tr>
<tr class="odd">
<td>13</td>
<td>Markus Richter</td>
<td>1979</td>
</tr>
<tr class="even">
<td>14</td>
<td>Nina Braun</td>
<td>1986</td>
</tr>
<tr class="odd">
<td>15</td>
<td>Felix Klein</td>
<td>1993</td>
</tr>
<tr class="even">
<td>16</td>
<td>Clara Zimmermann</td>
<td>1982</td>
</tr>
<tr class="odd">
<td>17</td>
<td>Tobias Hartmann</td>
<td>1988</td>
</tr>
<tr class="even">
<td>18</td>
<td>Sarah Peters</td>
<td>1994</td>
</tr>
<tr class="odd">
<td>19</td>
<td>Jan Schwarz</td>
<td>1989</td>
</tr>
<tr class="even">
<td>20</td>
<td>Leonie Weiß</td>
<td>1996</td>
</tr>
</tbody>
</table>
