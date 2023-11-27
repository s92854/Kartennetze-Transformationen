# Übung 1: ArcGIS Pro

1. Das shapefile „Landkreis_Goerlitz“ liegt im alten, heute nicht mehr amtlichen Lagereferenzsystem des Freistaates Sachsen vor.

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

2. a) Welcher Name wird für das heute amtliche Lagebezugssystem von Sachsen auf den Internetseiten der „Geobasisinformation und Vermessung“ Sachsen verwendet?

UTM für das ebene Koordinatensystem ETRS89

3. Um das shapefile „Landkreis_Goerlitz“ zu transformieren, stellen Sie in ArcGIS Pro das projizierte Koordinatensystem „ETRS 1989 UTM Zone 33N (N-zE)“ ein. ESRI bietet zur Transformation zwei Methoden (ohne die beiden Methoden mit Umweg über WGS84) an.

a) Wie heißen die beiden Methoden und bei welcher Methode handelt es sich um eine 7-Parameter-Transformation und bei welcher um einen gitterbasierten Transformationsansatz?

  1. RD/83_To_ETRS_1989_2_NTv2 - Gitterbasierter Transformationsansatz [Ostd.: 0.03m]
  2. RD/83_To_ETRS_1989_1 - 7-Paramter Transformation [ges. D: 1m]

b) Wenden Sie beide Methoden an und speichern Sie die beiden umprojizierten shapefiles jeweils unter dem passenden Namen „Landkreis_Goerlitz_ESRI_7Parameter“ und „Landkreis_Goerlitz_ESRI_Gitter“ ab.

[Transformationen.zip](https://github.com/s92854/Kartennetze-Transformationen/files/13476442/Transformationen.zip)

4.
