## Origen y descripción de los datos archivo Datos SMN Ushuaia 2020-2021
***Son datos provenientes del servicio meteorológico nacional, con datos de la ciudad de Ushuaia para los años 2020 y 2021.***
*La obtención de los mismos se realizo mediante consulta por mail al centro de información meteorológica del servicio meteorológico nacional (SMN) y posterior envio de los datos de su parte por el mismo medio.*

------------


##### Diccionario de datos
| Variable | Descripción | Tipo de Dato   |
| ------------ | ------------ | ------------ |
| Fecha | Fecha formato dd/mm/yyyy. | Fecha (datetime) |
| Temperatura Máxima | Temperatura máxima registrada para esa fecha. | Real (flotante, un decimal) |
| Temperatura Mínima | Temperatura mínima registrada para esa fecha. | Real (flotante, un decimal) |
| Temperatura Media | Temperatura media calculada para esa fecha. | Real (flotante, un decimal) |
| Temperatura Rocío | Temperatura rocío registrada para esa fecha. | Real (flotante, un decimal) |
| Presión Estación | Presión en la estación de monitoreo hectopascales (hPa) | Real (flotante, un decimal)  |
| Presión Mar | Presión a nivel del mar hectopascales (hPa) | Real (flotante, un decimal) |
| Precipitación | Precipitación en esa fecha en milimetros (mm).  | Real (flotante, un decimal) milímetros. |
| Hum. Relat. | Porcentaje de humedad relativa en esa fecha. | Entero |
| Heliofanía (horas) | Horas de sol. | Real (flotante). |
| Nubosidad | Nubosidad en octavos codigo: 0: Sin nubes, 1: 1 octavo o menos, pero con nubosidad, 2: 2 octavos, 3: 3 octavos, 4: 4 octavos, 5: 5 octavos, 6: 6 octavos, 7: 7 octavos o más pero no 8 octavos, 8: 8 octavos (cubierto, sin claros), 9: cielo invisible (oscurecido) por niebla y/u otro fenómeno meteorológico, /: Cubierta nubosa no discernible por otras razones distintas de niebla y/u otro fenómeno meteorológico, la observación no fue realizada. | Entero |
| Viento Máximo Dirección | Dirección predominante del viento en decagrados. Codigo: 2 = NNE, 5 = NE, 7 = ENE, 9 = E, 11 = ESE, 14 = SE, 16 = SSE, 18 = S, 20 = SSO, 23 = SO, 25 = OSO, 27 = O, 29 = ONO, 32 = NO, 34 = NNO, 36 = N, 0 = CALMA, 99 = DIRECCIÓN VARIABLE, \N = SIN DATO | Entero   |
| Viento Máximo Intensidad | Intensidad máxima del viento en esa fecha en metros por segundo (m/s) | Real (flotante, un decimal) |
| Vto Medio Intensidad | Intensidad media del viento en esa fecha en metros por segundo(m/s) | Real (flotante, un decimal) metros por segundo. |

*El archivo contiene 731 instancias una por cada día de cada año (366 en 2020 y 365 en 2021).
Los datos faltantes están reflejados con la cadena “\N".*
