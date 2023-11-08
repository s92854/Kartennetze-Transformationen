# Exkurs: Transformationen
## Geographic Coordinate System (GCS)
Definiert wo die Daten auf der Erdoberfläche verortet sind
* Verwendet eine dreidimensionalen sphäroidischen Oberfläche
* Positionen werden daher in Winkelmaßeinheiten (meist Grad) angegeben
* Benötigt außerdem einen Nullmeridian und ein Datum
* Zur Verwendung mit globalen Datensätzen geeignet
* ArcGIS projiziert die Daten zu Bearbeitungs- und Analysezwecken auf ein lokales planares Koordinatensystem

## Projected Coordinte System (PCS)
Definiert wie Daten auf einer flachen, zweidimensionalen Oberfläche dargestellt werden
* Positionen werden in linearen Einheiten (bspw. Meter) angegeben
* Verfügen über konstante Längen, Winkel und Flächen
* Basieren stets auf einem geographischen Koordinatensystem
* Insbesondere zur Verwendung mit lokalen Datensätzen geeignet
* Zur zweidimensionalen Ausgabe in Form von Karten sollte stets ein projiziertes Koordinatensystem verwendet werden

## EPSG (European Petrol Survey Group)


7-Parameter-Helmerttransformation
