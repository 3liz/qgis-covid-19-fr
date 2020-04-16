# COVID-19 dataviz in Lizmap

This is a QGIS Project showing the COVID-19 in France mainland using [Lizmap](https://github.com/3liz/lizmap-web-client) version 3.4.

![](lizmap-covid-19-fr.gif)

The Lizmap Web Client configuration and the QGIS project are provided.

### Versions

* QGIS 3.4
* Lizmap Web Client 3.4pre

### Update data

Get data by running with the [provided quick-and-dirty bash script](layers/covid_19_fr/get_data.sh)

```bash
cd layers/covid_19_fr/
chmod +x get_data.sh
./get_data.sh
```

Run it every time you need to upgrade the data. This will 

* download CSV file
* create additionnal CSV and CSVT files
* import data into the `france.gpkg` Geopackage file

### Sources

* French Covid data: https://www.data.gouv.fr/fr/datasets/donnees-hospitalieres-relatives-a-lepidemie-de-covid-19/
* Spatial data: https://github.com/gregoiredavid/france-geojson
