# Data Analyst

## Acerca de mí
👨‍💻 Soy ingeniero industrial con experiencia en mejora continua, análisis estadístico y programación en Python. Tengo sólidos conocimientos en metodologías como Six Sigma y mejora de procesos. He implementado KPI’s y dashboards que facilitan la toma de decisiones y la detección de causas raíz o tendencias, utilizando herramientas como Power BI y Excel. Mi enfoque en liderazgo, trabajo en equipo y comunicación efectiva ha sido clave para el éxito de estos proyectos.

🎯Actualmente, me acabo de certificar como Data Analyst a través de un bootcamp en TripleTen. En este programa, estoy adquiriendo habilidades avanzadas en programación como Python y SQL, utilizando GitHub, refinando mis capacidades de tratamiento de datos y fortaleciendo mis habilidades para presentar datos de manera efectiva. 

⚙Mis habilidades incluyen:

🥋 Certificación YellowBelt, conocimiento en lean Manufacturing y SixSigma.

⚙ Dominio avanzado de Excel, PowerBI y Bizagi modeler.

✨ Además, hablo español nativo, inglés avanzado y actualmente me encuentro estudiando Japones. 

📈 Análisis de datos utilizando herramientas de Lean Manufacturing, análisis de procesos,

🗺 Información adicional:

✈ Cuento con disponibilidad para trabajar en remoto y reubicarme en Santiago de Chile. 
______________________________________________________________________________________________________________

## Proyectos seleccionados

### Dashboard de OEE y cuadro de perdida de tiempos.
- El objetivo de este proyecto fue realizar un 
#### Herramientas
<img alt="excel" src="https://img.shields.io/badge/Excel-green?style=for-the-badge&logoSize=auto&color=darkgreen"> <img alt="Power Bi" src="https://img.shields.io/badge/Power%20Bi-yellow?style=for-the-badge&logoSize=auto&labelColor=black&color=yellow">
<img alt="power_query" src="https://img.shields.io/badge/PowerQuery-yellow?style=for-the-badge&logoSize=auto&color=yellow"> <img alt="Transformación de datos" src="https://img.shields.io/badge/Transformaci%C3%B3n%20de%20datos-black?style=for-the-badge&logoSize=auto&color=blue"> <img alt="Visualización de datos" src="https://img.shields.io/badge/Visualizaci%C3%B3n%20de%20datos-black?style=for-the-badge&logoSize=auto&color=blue">


## Analisis de retención de usuarios de un gimnasio.  

Uno de los problemas más comunes que enfrentan los gimnasios es la perdida de clientes, así que en este proyecto analizo el comportamiento de los usuarios, mediante los datos analiticos presentados, busco predecir la perdida de usuarios del siguiente mes, utilizando machine learning para un caso de clasificación binaria, donde pruebo dos métodos 1) Regresión logistica y 2) bosque aleatorio, evaluando sus resultados y tomando la decisión de cual utilizar. A su vez, creo cluster para clasificar a los usuarios de acuerdo a su comportamiento y posteriormente calcular la tasa de cancelación de cada una de los clusters, obteniendo como resultado un perfil de usuario objetivo que suele cancelar su suscripción el proximo mes.

### Herramientas y tipo de proyecto

![Static Badge](https://img.shields.io/badge/sklearn-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/pandas-blue?style=for-the-badge&logo=pandas)
 | ![Static Badge](https://img.shields.io/badge/matplotlib.pyplot-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/seaborn-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/machine%20learning-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/clustering-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/ETL-blue?style=for-the-badge)| 

### Metodología
**Preprocesamiento de datos:**   
Se estandarizaron los nombres de las columnas, se verificaron y limpiaron los valores ausentes y duplicados.

**Analisis Exploratorio de datos (EDA):**  
- Se analizaron los patrones de los usuarios que cancelaron y los que permanecen.
- Se realizo un mapa de calor para definir las caracteristicas con mayor colerración para los usuarios que cancelaron.

**Modelado predictivo:**  
Para predecir la cancelación de los usuarios del proximo mes, se entrearon dos modelos, regresión logística y bosque aleatorio. y se evaluaron para elegir el mejor modelo. Obteniendo una presición de 85% y 84% respectivamente  

**Clustering:**  
Se crea una matriz de distancias para obtener el valor de grupos para k-means y generar nuestros grupos de segmentación.

### Preguntas clave
-¿Cuál es la probabilidad de perdida (para el próximo mes) para cada cliente?  
-¿Cual es el perfil de usuarios que suele cancelar?  
-¿Que factores impactan la pérdida?   

### Visualizaciones destacadas

1. Mapa de calor segmentación de usuarios por tasa de cancelación (churn)
Como podemos observar en el mapa de calor las caracteristicas con mayor correlación son:

- Con 95% month to end contract con el periodo de contrato,
- Con 95% avg class frequency total y avg class frecuency current month
- Con 45% promo friends y partner

<img src="assets /img/heatmap_gym.png" alt="Mapa de calor por cancelación" style="width:100%">

3. Análisis de clústers
Mediante la matriz de distancia creamos grupos posibles para posteriormente generar nuestros clústers.
<img src="assets /img/Cluster_gyms.png" alt="Analisis de clústers" style="width:100%">


### Conclusiones y recomendaciones

Al crear grupos mediante clúster logramos obtener grupos interesantes, tomando como punto de partida el grupo con mayor tasa de cancelación, obtuvimos que el grupo 2 que representa el 20.5% de la población total posicionándose como el segundo grupo más grande, lo cual representa una gran oportunidad, el análisis arrojo que el 100% de los usuarios del grupo 2 se encuentran cerca de las instalaciones, el 67.6% no cuenta con un partner y el rango de edad va de los 25 a 30 años, por lo que se puede ofrecer descuentos a esos usuarios dentro de ese rango de edad, en los horarios de menos flujo de personas, así mejorando nuestra ocupación de las instalaciones y incrementando la retención de usuarios de este grupo. Se sugiere realizar un estudio A/B, donde el grupo B sea un grupo seleccionado de los usuarios de este clúster y probando la estrategia de retención de los usuarios mencionada anteriormente. Esto se puede llevar a cabo mediante una campaña de marketing por mensajes de texto, ya que se cuenta con el 90% de los números de teléfono de los usuarios. 

Propuestas:
- Campañas de marketing por telefono: El 90% de los usuarios proporcionaron su número para contacto, conviritiendose en un excelente canal de comunicación.
- Realizar una prueba A/B con una campaña personalizada para usuarios de 25 a 30 años con promoción en horarios con menos flujo para incrementar la retención y el uso de las instalaciones.
- Fomentar las actividades grupales en los usuarios más jovenes ya que los usuarios que participan en estas actividades suelen renovar su suscripción.




