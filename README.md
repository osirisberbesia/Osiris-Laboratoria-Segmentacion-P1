# Proyecto de Análisis de Datos.
## Segmentación Proyecto 1 


### Objetivos:


Preparar la información de la base de datos y aplicar la segmentación de clientes a través de RFM, entender el resultado de la segmentación  y sacar conclusiones que posibiliten a la empresa a tomar decisiones, las cuales son requeridas por parte de la empresa para mantener y aumentar sus ingresos, además buscar información importante que se encuentra oculta en los datos.

### Equipo:

Describe si trabajaste en dupla o individualmente.

### Herramientas y Tecnologías:

* Hojas de cálculo Excel
* OpenAI - ChatGPT


### Procesamiento y análisis:

* Antes de la exploración de datos, se importan los datos de los tres data_sets recibidos en un solo documento con la formula IMPORTRANGE.
* Una vez realizada la importación de datos, se procede a la busqueda de nulos para tomar decisiones acerca de estos.
* Para los data_set clientes, transacciones, y resumen se agregará una columna adicional para la formula "countblank" y así poder determinar con mejor exactitud cuales acciones tomar
    * Para el data_set clientes, la categoria ingreso_anual_dolar tiene un total de 24 clientes con esta información en nulo, en este data_set, para no eliminar a los clientes, se establecerá un valor de -1 de forma que:
        - Todos los clientes que tengan valor -1 en su ingreso_anual_dolar, se debe crear una alerta para actualizar la información del mismo. 
    * Para el data_set transacciones, existen los siguientes nulos:
    ![alt text](image.png)
    Los cuales, al no tener el ID del cliente ni otra fuente de datos para recuperar la información faltante, se decide omitir estos, los cuales, serán identificados con un 0 para omitir.
    * Para el data_set resumen_compras, no existe ninguna categoria con nulos. Por lo cual se trabajará con la información de todo el data set segun aplique.
    * * Para los data_sets que tienen nulos y se deben modificar a  -1 y 0 según lo explicado anteriormente, al ser data_sets importados, no se puede modificar la información dentro de ellos, por lo cual se hará una columna adicional, donde se recorra cada categoria donde están los nulos y modifique los datos a -1 o 0 según corresponda la ubicación del nulo, y se trabajará con esta columna auxiliar.

    


Describe los procesos de limpieza y exploración de datos, las técnicas de análisis aplicadas, etc.

### Resultados y Conclusiones:


Presenta los principales resultados obtenidos a partir del análisis de datos.
Resume las conclusiones extraídas del proyecto, incluyendo ideas importantes, descubrimientos relevantes y posibles recomendaciones.

### Limitaciones/Próximos Pasos:

Identifica y describe cualquier limitación o desafío encontrado durante el proyecto.
Sugiere posibles próximos pasos para extender o mejorar el proyecto de análisis de datos.

### Enlaces de interés:

Incluye el enlace a la hoja de cálculo donde desarrollaste el proyecto y/o un enlace a tu dashboard (marco 3), además de otros recursos creados para este proyecto que consideres interesante compartir.

