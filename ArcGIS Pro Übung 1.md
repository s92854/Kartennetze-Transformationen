# Übung 1: ArcGIS Pro

1. **Grundlagen**

Das shapefile „Landkreis_Goerlitz“ liegt im alten, heute nicht mehr amtlichen Lagereferenzsystem des Freistaates Sachsen vor.

a) Wie lautet der Name des verwendeten projizierten Koordinatensystems bei ESRI?

RD 83 GK Zone 5

&nbsp;

b) Welchen (EPSG)-Code hat es?

3399

&nbsp;

c) Welche Projektion wird verwendet?

Gauss Kruger

&nbsp;

d) Auf welchem Datum und Spheroid basiert es?

Datum: D Rauenberg 1983

Spheroid: Bessel 1841

&nbsp;

e) Für welchen Bereich von Sachsen ist es definiert (Area of Use, Min. Lat., Min. Long., Max. Lat., Max. Long.)?

Area of Use: Deutschland – Ost Deutschland alle Staaten/Bundesländer

Min. Lat.: 50.200

Min. Long.: 9.920

Max. Lat.: 54.740

Max. Long.: 15.040

&nbsp;

2. **Name**

a) Welcher Name wird für das heute amtliche Lagebezugssystem von Sachsen auf den Internetseiten der „Geobasisinformation und Vermessung“ Sachsen verwendet?

UTM für das ebene Koordinatensystem ETRS89

&nbsp;

3. **Transformationen**

Um das shapefile „Landkreis_Goerlitz“ zu transformieren, stellen Sie in ArcGIS Pro das projizierte Koordinatensystem „ETRS 1989 UTM Zone 33N (N-zE)“ ein. ESRI bietet zur Transformation zwei Methoden (ohne die beiden Methoden mit Umweg über WGS84) an.

a) Wie heißen die beiden Methoden und bei welcher Methode handelt es sich um eine 7-Parameter-Transformation und bei welcher um einen gitterbasierten Transformationsansatz?

  1. RD/83_To_ETRS_1989_2_NTv2 - Gitterbasierter Transformationsansatz [Ostd.: 0.03m]
  2. RD/83_To_ETRS_1989_1 - 7-Paramter Transformation [ges. D: 1m]

&nbsp;

b) Wenden Sie beide Methoden an und speichern Sie die beiden umprojizierten shapefiles jeweils unter dem passenden Namen „Landkreis_Goerlitz_ESRI_7Parameter“ und „Landkreis_Goerlitz_ESRI_Gitter“ ab.

[Transformationen.zip](https://github.com/s92854/Kartennetze-Transformationen/files/13476442/Transformationen.zip)

&nbsp;

4. **7-Parameter Transformation**

a)

Auf Basis des [pdf](https://github.com/s92854/Kartennetze-Transformationen/files/13587918/Beschreibung_Transformation_RD-83_SN-ost.pdf), welches man auf der Landesvermessungsseite für Sachsen Ost findet, ergibt folgende Transformation:

<img width="500" src="https://github.com/s92854/Kartennetze-Transformationen/assets/134683810/2b936154-7125-4e05-909d-c8d1765a47c4">

&nbsp;

Anschließend muss man die Projektion noch anwenden, indem man ein ETRS89 KS auswählt und dann die eigene Transformation:

<img width="500" src="https://github.com/s92854/Kartennetze-Transformationen/assets/134683810/e23dbdf8-fde9-4d3a-90a8-060c048fc914">

&nbsp;

b) Positionsvektor

c) 

<img width="400" src="https://github.com/s92854/Kartennetze-Transformationen/assets/134683810/328da7af-4937-4b1a-8ea2-5366a73922d8">

&nbsp;

5. **Genauigkeit**

Laut der [Codetabelle](https://www.landesvermessung.sachsen.de/prod_fest_raum_fest/EPSG-Code-Tabelle.pdf) der Landesvermessung Sachsen, hat die Gittertransformation mit 3cm Genauigkeit die höchste Genauigkeit und die regionale 7-Parameter-Transformation mit 1m die zweit höchste Genauigkeit.

<img width="800" src="https://github.com/s92854/Kartennetze-Transformationen/assets/134683810/f62098f9-78e1-4c1b-8272-d0a721755a60">

&nbsp;

6. **Abstände messen**

Durch Messen ergaben sich folgende Abstände untereinander:

* ESRI-Gitter - Eigene ≈ 50 mm
* ESRI-7-PAR - Eigene ≈ 260 mm
* ESRI-7-PAR - ESRI-Gitter ≈ 30 mm
