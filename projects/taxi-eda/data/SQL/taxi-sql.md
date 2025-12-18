## Proyecto Zuber — Análisis de Transporte Urbano

### Objetivo
Consultar datos mediante consultas SQL para extraer datos relevantes para su análisis.

### Metodología
- Extracción y agregación de datos mediante SQL
- Integración de datasets (viajes, clima, ubicaciones)
- Análisis exploratorio y validación de hipótesis en Python
> "Esta consulta integra los conceptos principales trabajados en el proyecto: filtrado de datos, uniones entre tablas (JOINs), clasificación condicional y agregación de información."

### SQL (documentación visual)
> Debido a restricciones de la plataforma, los queries no pueden exportarse.
> A continuación se documentan mediante capturas.
> "Se presentan las consultas más relevantes con explicación detallada de su lógica y resultados."

#### Clasificación de condiciones climáticas y duración del viaje
Esta consulta clasifica las condiciones climáticas en **Good** y **Bad** a partir de la descripción del clima,
y analiza la duración de los viajes para un trayecto específico los días sábado.
**Qué hace esta consulta:**
- Une los datos de viajes con los registros meteorológicos mediante un `INNER JOIN`.
- Clasifica el clima como **Bad** cuando hay lluvia o tormenta, y **Good** en el resto de los casos.
- Filtra viajes con una ruta específica (pickup 50 → dropoff 63).
- Selecciona únicamente viajes realizados en sábado.
- Extrae la duración del viaje en segundos para su análisis posterior.
[Clasificación de clima y duración del viaje](image.png) 
**Resultado observado:**
Los datos muestran la duración de los trayectos segmentada por condiciones climáticas,
lo que permite comparar tiempos de viaje entre escenarios de clima favorable y adverso.
Esta información se utiliza posteriormente para validar la hipótesis sobre el impacto del clima
en la duración de los viajes.

> Nota: Esta consulta forma parte del análisis exploratorio previo a la validación estadística
> realizada en Python.