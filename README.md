#Data Science 2019 - Digital House /Data
##Trabajo Integrador
![](https://www.ausa.com.ar/wp-content/themes/ausa/images/logo-ausa-negro.png)
##Seguridad Vial Autopistas Ausa 
###Introducción
####Información de hechos que requirieron atención por parte de Seguridad de Vial de AUSA.

El dataset consiste en vectores de características que pertenecen a 5700+ incidentes o hechos que requirieron atención por parte de Seguridad de Vial de AUSA. 

El conjunto de datos se conforma de manera que cada registro pertenezca a un hecho diferente. Cada hecho se registra con fecha y hora, vía dónde ocurre, condiciones climáticas y vehículos involucrados.

El conjunto de datos original consta de 1 atributo de fechas, 8 atributos numéricos y 6 atributos categóricos. El atributo 'lesionados' o 'fallecidos' se utiliza como etiqueta de clasificación.

####Descripción de las columnas:
**Fecha:** Fecha del hecho.

**Autopista:** En cuál de las autopistas que administra AUSA se produjo el hecho. (También se informan zonas importantes como el distribuidor de 9 de julio y la zona de transición entre la AU1 y las AU6).
**Localización:** Detalle que da más precisión del lugar donde se produjo el hecho dentro de la autopista.
**Punto Kilométrico:** Lugar del hecho contado desde el kilometro 0 de cada autopista.

**Tipo Evento:** Categorización del hecho:
*   **Accidente:** acontecimiento inesperado, no planeado, que implica una alteración en el estado normal de las personas, elementos o funciones, con repercusiones negativas,con potencial para causar lesiones o muerte en las personas y daños o perjuicios a bienes de los actores involucrados o de terceros.
*   **Incidente:** materialización de un riesgo en un suceso concreto de escasa o nula
repercusión dañina, que puede ocasionar una reducción temporaria de la calzada o un
incremento anormal de la demanda, que afecta la seguridad vial y que puede
desencadenar en un accidente.

**Tipo de siniestro:** son descripciones acotadas o categorizadas del hecho de tránsito.

**Tipos de Vehículos:** es la clasificación por tipología de vehículos involucrados.
*   Camiones (incluye FURGON GRANDE, GRUAS).
*   Autos (incluye: TAXI, PIC UP, CAMIONETA, FURGON CHICO).
*   Motos
*   Ómnibus (Incluye: AUTOBUS y MINIBUS).

**Clima:** Estado del Clima en el momento del hecho (seleccionado manualmente).

**Estado Pavimento:** Estado del pavimento en el momento del hecho (seleccionado
manualmente).

**Fallecidos y Heridos:** Numero de involucrados en los accidentes según su estado de gravedad.



---


###  Series de tiempo

El análisis de series de tiempo se suele utilizar para proyectar o pronosticar la evolución de una variable a lo largo del tiempo, a partir de información previa sobre esa misma variable. 

#### 1) Análisis exploratorio y preprocessing

El dataset nos provee:
*   tres columnas sobre la ubicación donde se produce el incidente. 
*   tres columnas relacionadas a la fecha del incidente. (donde detectamos una inconsistencia de origen en el formato de la fecha, y para lo cual el dataset incluye una columna adicional que permite corregirlo).
*   dos columnas sobre las condiciones ambientales al momento del incidente.
*   cinco columnas sobre el tipo de incidente y los vehículos involucrados.
*   dos columnas sobre el estado y cantidad de personas involucradas.


*Otras características:*
La función "Día especial" indica la proximidad del tiempo de visita del sitio a un día especial específico (por ejemplo, el Día de la Madre, el Día de San Valentín) en el que es más probable que las sesiones finalicen con la compra. El valor de este atributo se determina considerando la dinámica del comercio electrónico, como la duración entre la fecha del pedido y la fecha de entrega. Por ejemplo, para el día de San Valentín, este valor toma un valor distinto de cero entre el 2 de febrero y el 12 de febrero, cero antes y después de esta fecha a menos que esté cerca de otro día especial, y su valor máximo de 1 el 8 de febrero. El conjunto de datos también incluye sistema operativo, navegador, región, tipo de tráfico, tipo de visitante como visitante recurrente o nuevo, un valor booleano que indica si la fecha de la visita es el fin de semana y el mes del año.

*Fuente: https://data.buenosaires.gob.ar/dataset/seguridad-vial-autopistas-ausa/archivo/187.2*


---

