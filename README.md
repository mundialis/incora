# incora

Inwertsetzung von Copernicus-Daten für die Raumbeobachtung” (incora)

Valorization of Copernicus data for urban monitoring (incora)

## Introduction

As part of the sustainability goals, the economical use of land as a resource has been the subject of planning interventions and political measures by the Federal Government for many years. The demands for use are particularly conflict-laden when dealing with settlement and traffic areas. Here, the data bases used for monitoring the development of residential and transport areas are of particular importance. The currently available data bases are not always up to date and show structural breaks when considering land consumption over longer periods of time. In addition, many qualitative aspects are not mapped. The project "[Inwertsetzung von Copernicus-Daten für die Raumbeobachtung (incora)](https://www.mundialis.de/en/verbessertes-siedlungsflachenmonitoring-durch-satellitengestutzte-raumbeobachtung/), which is funded by the Federal Ministry of Transport and Digital Infrastructure (BMVI), aims to use the data of the Copernicus Sentinel satellites to supplement the existing indicators of settlement and transport area development and to increase the quality and informative value of the existing indicators. The results lead to an improved information basis for measures to control and reduce land use, but can also be used economically to make land potentials visible in the existing stock. The processing of Copernicus data to derive spatial development indicators is carried out with innovative cloud computing solutions. Information needs and indicators are jointly conceived or determined and coordinated in an exchange between science, administration and planning practice.
The results will be made publicly available in spatial observation portals. Together with the project partners, the BBSR will develop and test the indicators and develop an appropriate set of indicators for nationwide area monitoring. The final provision of the results in spatial observation portals and the necessary coordination processes are primarily tasks of the BBSR.

The project is coordinated by the Institut für Landes- und Stadtentwicklungsforschung (ILS) (Institute for Regional and Urban Development Research), and is carried out jointly with the Bundesinstitut für Bau-, Stadt- und Raumforschung (BBSR) and mundialis GmbH & Co. KG.

## Kurzbeschreibung DE

Inwertsetzung von Copernicus-Daten für die Raumbeobachtung (incora). Berechnung von flächendeckenden Indikatoren für Siedlungs- und Verkehrsflächen aus Copernicus-Sentinel-Daten. Ziel des Projektvorhabens ist, Copernicus-Daten und -Dienste für die Raumbeobachtung in Wert zu setzen und dazu datenbasierte Anwendungen im Bereich "Fernerkundung/Satelliten" zu verbessern. Im Fokus steht die Ergänzung des Monitorings der Siedlungs- und Verkehrsflächen (SuV) mit Indikatoren zur Beschreibung qualitativer Aspekte des Flächenverbrauchs in Deutschland.

Förderkennzeichen: Förderkennzeichen: 19F2079C

## GRASS GIS addons

* [r.change.stats](https://github.com/mundialis/r.change.stats) - GRASS GIS addon that calculates change statistics from two discrete raster maps. 
* [r.import.worker](https://github.com/mundialis/r.import.worker) - GRASS GIS worker addon to run r.import in different mapsets.
* [r.incora](https://github.com/mundialis/r.incora) - GRASS GIS multi-addon for Incora landcover classification.
    * v.incora.training_data: creates a vector map containing training points from a set of rules containing the output classes: forest, low vegetation, water, built-up, bare soil and agriculture.
    * r.incora.postproc: uses post processing to deal with mixed pixels identified in v.incora.training_data. Mixed pixels (class 70) are removed from the map. The gaps are then filled using r.grow.distance.
    * r.incora.change: runs a change detection based on two input maps. The nomenclature is optimized for the incora project.
* [r.learn.predict.parallel](https://github.com/mundialis/r.learn.predict.parallel) - GRASS GIS addon for running r.learn.predict in parallel.
* [r.mapcalc.worker](https://github.com/mundialis/r.mapcalc.worker) - GRASS GIS worker addon to run r.mapcalc in parallel in different mapsets.

![](https://www.mundialis.de/wordpress/wp-content/uploads/2021/04/Germany_2020-scaled.jpeg)
Germany 2020 - Land cover based on Sentinel-2 data ([source](https://www.mundialis.de/en/deutschland-2020-landbedeckung-auf-basis-von-sentinel-2-daten/))
