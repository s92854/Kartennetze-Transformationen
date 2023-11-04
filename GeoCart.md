# Übung 1: polständige stereografische Projektion

# Übung 2: schiefachsige, flächentreue, polare Azimutalabbildung
0. Von [Natural Earth](https://www.naturalearthdata.com/downloads/) im Maßstab 1:50 Mio. [Countries](https://github.com/s92854/Kartennetze-Transformationen/files/13256657/ne_50m_admin_0_countries.zip) und [Coastlines](https://github.com/s92854/Kartennetze-Transformationen/files/13256658/ne_50m_coastline.zip) herunterladen und entpacken.
1. File > New
2. Map > New
3. Rundes Projektionssymbol (4te rechts neben Projection) > Lambert equal-area
4. Map > Databases > Add installed databases > .shp Datei beider Natural Earth zip-Files auswählen > Stylized World Topo 5400x2700.raw deaktivieren
5. Map > Nominal Scale > 1:50000000 eitragen
6. Map > Boundaries > Kartenbegrenzungen auf ϕ1=40°N, λ1=20°W und ϕ2=40°S, λ2=60°E festlegen

<img width="748" alt="image" src="https://github.com/s92854/Kartennetze-Transformationen/assets/134683810/59b6fcb7-23f6-4b28-a845-1a7f3884529c">

&nbsp;

7.Map > Projection Centre > 20°E Logitudinal einstellen

<img width="525" alt="image" src="https://github.com/s92854/Kartennetze-Transformationen/assets/134683810/d47986bf-325f-48cf-8536-8ac23588c130">

8. Map > Line Styles
    * Parallel > Tropic, Equator > Farbe, Strichstärke, Dash pattern ändern
    * Ocean > Coast > blau, Strichstärke ändern
    * Meridian & Parallel > Normal > Farbe (z.B. 173,173,173), Strichstärke (z.B. 0.3) ändern

9. Map > Graticule > Parallel & Meddian spacing auf 10°
