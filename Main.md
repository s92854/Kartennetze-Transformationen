# Einführung

Manipulation durch Wahl der Projektion

# Klausur
1 Spickzettel:
* 2 Blatt Din A4
	* Vorder- und Rückseite darf beschrieben sein
	* keine Regel, was drauf stehen soll
	* handgeschrieben
	* Namen rauf
	* Abstract der Leseaufgaben raufschreiben
	* farblich
	* muss für jede Klausur neu geschrieben

# Grundlagen
## Form der Erde

IUGG 1980 Grundlage für das WGS84

### Erdradius des Rotationsellipsoids nach Bessel 1841, Hayford 1909, IUGG 1980

Berechnungen in Metern:

#### Bessel 1841

RV1=6370264,422
RO1=6370291


#### Hayford 1909

RV2=6371221,284
RO2=6371229,333


#### IUGG 1980

RV3=6371000,685
RO3=6371008,667


Für Netzberechnungen im Maßstab 1:2 Mio. und kleiner (1:3 Mio., 1:4 Mio., etc.) ist als Kugelradius R = 6371km zu verwenden


### Longitude
* Synonym: Meridiane = Längengrad
* verlaufen in Nord-Süd-Richtung
* werden in °Ost und °West angegeben
* Distanz zwischen den Meridianen ist am Äquator am größten und an den Polen am niedrigsten
* am Äquator ist ein rechter Winkel zwischen ihnen
* sind wie erddurchdringende Flächen
* jeder Meridian ist gleich lang
* jeder Meridian ist ein Halbkreis

## Bogenminute in Kilometern = 1 Seemeile
$$\frac{40.000km}{360*60}=1,851km$$

## Fläche Deutschland berechnen
$\delta = 90° - \Phi$


## Begriffe
* Azimutale Abbildung = Eine Fläche mit Verwendung einer Hilfsfläche
* Kegelprojektion
* Zylinderprojektion
* Normale, Erdachsige Abbildungen
* Transversale, Querachsige Abbildungen
* Vermittelnde Projektionen/Abbildungen = Projektionen, die ein wenig flächenverzerrt und ein wenig winkelverzerrt sind
* Orthodrome = Großkreis; kürzeste Entfernung zwischen zwei Punkten
* Loxodrome = Schneidet alle Breiten in gleichem Winkel

### Echte oder Unechte Abbildung?
siehe AB

A = 1
B = 0
C = 0
D = 1
E = 0
F = 0

## Eigenschaften von Abbildungen
Längentreue bezieht sich immer auf eine Richtung
> wenn Längentreue in Nord-Süd Richtung: trotzdem ist am Äquator Längentreue gegeben

## Strahlensatz am Einheitskreis
$\frac{PN'}{PO} = \frac{AN}{AO}$

$S = PN'$

$S = \frac{AN * PO}{AO}$

$s = \frac{sin\delta * (1 + d)}{d + cos\delta}$

&nbsp;

### Herleitungen

$sin\delta = \frac{AN}{1} = AN$

&nbsp;

$AO = d + AM$

$cos\delta = \frac{AM}{1}$

$AO = d + cos\delta$

&nbsp;

$PO = 1 + d$

#### Berechnungen von s in 10° Schritten
Für

00° = 0
10° = 0,1745
20° = 0,3490
30° = 0,5234
40° = 0,6972
50° = 0,8996
60° = 1,0392
70° = 1,2037
80° = 1,3592
90° = 1,5

## Azimutalabbildungen
Für d = 0 (Gnomische Projektion):
$\phi > 0$


## Doppelwinkelfunktion

$s=\frac{sind\delta * (1+d)}{d+cos\delta}$

$s=\frac{sin\delta*2}{1+cos\delta}$

$s=\frac{2*2sin(\frac{\delta}{2})*cos(\frac{\delta}{2})}{1+2cos^2(\frac{\delta}{2})-1}$

$s=\frac{4*sin(\frac{\delta{2})*cos(\frac{\delta}{2}))}{2*cos(\frac{\delta}{2}))}$

&nbsp;

i) $sin(2\xi)=2sin\xi*cos\xi$

$sin\delta=2sin(\frac{\delta}{2})*cos(\frac{\delta}{2}$

ii) $cos(2\xi)=2cos^2(\xi)-1$

$cos(\delta)=2cos^2(\frac{delta}{2})-1$


## Exkurs: Transformationen
### Geographic Coordinate System (GCS)
Definiert wo die Daten auf der Erdoberfläche verortet sind
* Verwendet eine dreidimensionalen sphäroidischen Oberfläche
* Positionen werden daher in Winkelmaßeinheiten (meist Grad) angegeben
* Benötigt außerdem einen Nullmeridian und ein Datum
* Zur Verwendung mit globalen Datensätzen geeignet
* ArcGIS projiziert die Daten zu Bearbeitungs- und Analysezwecken auf ein lokales planares Koordinatensystem

### Projected Coordinte System (PCS)
Definiert wie Daten auf einer flachen, zweidimensionalen Oberfläche dargestellt werden
* Positionen werden in linearen Einheiten (bspw. Meter) angegeben
* Verfügen über konstante Längen, Winkel und Flächen
* Basieren stets auf einem geographischen Koordinatensystem
* Insbesondere zur Verwendung mit lokalen Datensätzen geeignet
* Zur zweidimensionalen Ausgabe in Form von Karten sollte stets ein projiziertes Koordinatensystem verwendet werden

### EPSG (European Petrol Survey Group)


7-Parameter-Helmerttransformation
