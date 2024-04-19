## Origen y descripción de los datos archivos TPM 2021 y TPM 2022
**Son datos provenientes del Laboratorio de Toxinas y Microbiología de la ciudad de Ushuaia para sus respectivos años (2021 y 2022). Los datos fueron solicitados al laboratorio el dia 23/10/2023 y fueron enviados en formato excel via correo eléctronico**

#### Diccionario de datos
| Variable | Descripción | Tipo de Dato |
| ------------ | ------------ | ------------ |
| Fecha Análisis | Fecha en la que se realizó el análisis en formato dd/mm/yyyy. | Fecha (datetime). |
| N° muestra | Numero correlativo de las distintas muestras realizadas en el año. | Entero.   |
| Producto | Molusco con el cual se realizó el examen M para mejillón, Ch para cholga. | Cadena de Caracteres. |
| Zona | Código o nombre de la zona de donde se recolecto la muestra. | Cadena de Caracteres. |
| Resultado | Resultado del examen nivel de toxina paralizante. ND para no detectado. (µg STX eq. kg)** | Real (flotante, dos decimales). |

*El archivo de 2021 contiene 160 instancias mientras que el de 2022 105 instancias, el resto del año los análisis resultaron no detectables.*
**microgramos de saxitoxina equivalente por kilo de muestra, el limite para que el producto no sea apto para consumo es 800.
