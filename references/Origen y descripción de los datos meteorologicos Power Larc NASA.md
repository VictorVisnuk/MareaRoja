## Origen de los datos meteorologicos Power Larc NASA.
Son datos provenientes del *Power Project* de la Administración Nacional de Aeronáutica y el Espacio (**NASA** por sus siglas en inglés).
La obtencion de los mismos se realizó mediante descarga desde la pagina web https://power.larc.nasa.gov/data-access-viewer/ el dia 25/10/2023 desde donde podes seleccionar el punto del planeta deseado y las variables a incluir y permite descargarlas en distintos formatos.

##### Diccionario de datos
| Variable | Descripción | Tipo de Dato   |
| ------------ | ------------ | ------------ |
| YEAR| Año del dato| Entero|
| DOY | Dia del año (0-366)| Entero |
| ALLSKY_SFC_PAR_TOT| Radiación descendiente de onda corta todo el cielo (W/m2) | Real (flotante, dos decimales) |
| CLRSKY_SFC_PAR_TOT| Radiación descendiente de onda corta cielo despejado (W/m2)| Real (flotante, dos decimales) |
| T2M | Temperatura a 2 metros (°C)|  Real (flotante, dos decimales) |
| T2MDEW | Punto de rocío/escarcha a 2 metros (°C) |  Real (flotante, dos decimales) |
| T2MWET | Temperatura de bulbo húmedo a 2 metros (C) |  Real (flotante, dos decimales) |
| TS | Temperatura de la superficie de la tierra (°C)|  Real (flotante, dos decimales) |
| T2M_RANGE | Rango de temperatura a 2 metros (°C)|  Real (flotante, dos decimales) |
| T2M_MAX | Temperatura maxima a 2 metros (°C)|  Real (flotante, dos decimales) |
| T2M_MIN | Temperatura minima a 2 metros (°C)|  Real (flotante, dos decimales) |
| QV2M | Humedad especifica a 2 metros (g/kg)|  Real (flotante, dos decimales) |
| RH2M | Humedad relativa a 2 metros (%)|  Real (flotante, dos decimales) |
| PRECTOTCORR | Precipitación corregida (mm/día)|  Real (flotante, dos decimales) |
| PS | Presión superficie (kPa)|  Real (flotante, dos decimales) |
| WS2M | Velocidad del viento a 2 metros (m/s)|  Real (flotante, dos decimales) |
| WS2M_MAX | Velocidad del viento maxima a 2 metros (m/s)|  Real (flotante, dos decimales) |
| WS2M_MIN | Velocidad del viento minima a 2 metros (m/s)|  Real (flotante, dos decimales) |
| WS2M_RANGE | Rango velocidad del viento a 2 metros (m/s) (°C)|  Real (flotante, dos decimales) |
| WD2M | Dirección del viento a 2 metros (grados)|  Real (flotante, dos decimales) |



*El archivo contiene 730 instancias una por cada día de cada año (365 en 2021 y 365 en 2022).
