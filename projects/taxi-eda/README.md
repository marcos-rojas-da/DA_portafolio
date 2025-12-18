# Taxi Trips – Exploratory Data Analysis (Chicago)

## Objetivo
Analizar el sistema de taxis en Chicago utilizando datos procesados en Python con el fin de comprender el comportamiento del servicio de transporte.  
El análisis se enfoca en identificar patrones de demanda, desempeño de las empresas de taxis y evaluar si factores externos, como las condiciones 
climáticas influyen en la duración de los viajes.

---

## Herramientas
- Python  
- pandas  
- matplotlib  
- seaborn  
- Scipy

---

## Análisis
Se realizó un análisis exploratorio de datos (EDA) que incluyó:

- Limpieza y preparación de datos (manejo de valores faltantes, formatos de fecha y tipos de datos).
- Análisis temporal para identificar patrones de demanda según el día y la hora.
- Comparación del desempeño entre diferentes empresas de taxis en términos de número de viajes y duración promedio.
- Evaluación de la relación entre variables externas (clima) y la duración de los viajes.
- Visualización de distribuciones, tendencias y comparaciones mediante gráficos.

---

## Insights clave
- Se identificaron zonas con mayor demanda de viajes, concentrando la mayoría de los trayectos.
- Se detectó una empresa de taxis líder en volumen de viajes frente al resto de competidores.
- Los viajes presentan variaciones claras según el momento del día, con picos en horarios específicos.
- Mediante pruebas de hipótesis estadísticas, se analizó el impacto del clima en la duración de los viajes.

---

## Hipótesis sobre el clima
Se planteó la hipótesis de que las condiciones climáticas adversas (por ejemplo, lluvia) incrementan la duración promedio de los viajes.  
Para evaluarla, se aplicó una metodología estadística rigurosa que incluyó:
- **Prueba de Levene:** Para verificar la igualdad de varianzas entre grupos
- **Prueba t-student de 2 muestras independientes:** Para comparar los promedios de duración entre viajes en condiciones climáticas normales y adversas
- **bajo un umbral de decisión estadística del 5%** para evaluar el impacto del clima.
Debido a que existen diferencias estadísticamente significativas, se rechaza la Hipótesis Nula (es decir, sí hay evidencia 
para afirmar que los viajes pueden durar más).

Los resultados indicaron que efectivamente, el clima puede llegar a afectar la duración de los viajes.

---

## Conclusiones
El análisis permitió comprender mejor los patrones de uso del sistema de taxis en Chicago y el desempeño de las empresas involucradas.  
Los resultados obtenidos pueden apoyar la toma de decisiones relacionadas con la optimización del servicio, asignación de 
recursos y evaluación del impacto de factores externos como el clima.