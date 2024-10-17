# Tema 2 Historia Ciclo de vida de una aplicación de Aprendizaje de Máquina (AM)
## Resumen 
### Video: Introduccion a Machine Learning
- El cerebro humano reconoce lo que esta viendo, la inteligencia artificial limita el reconocimiento a los datos que tenga
- Reglas + Datos --PrgramacionTradicion--> Resultados
- Machine Learning: Dar respuesta a programa, y que reconozca en un conjunto de datos aquellos que tengas esas caracteristicas
- Funcion de perdida y optimizados (mejora la aproximacion) --> Parametros clave para ML

### Fases tipicas en el ciclo de vida de una aplicación de AM
1. **Identificacion del Problema**
Definir el objetivo del proyecto y determinar el AM que puede ayudar a darle solucion.

2. **Recolección de Datos**
Obtencion de datos *relevantes, precisos y representativos*.

3. **Preparación de Datos**
Limpiar datos, caracterizar valores faltantes, normalizar y escalar las caracteristicas, y dividir los datos en conjuntos de entrenamiento y prueba.

4. **Ingenieria de Modelos**
Seleccion y entranamiento de modelos de AM. Incluye seleccion de algoritmos, creacion de caracteristicas y realizacion de ajustes de hiperparámetros.

5. **Evaluación del Modelo**
Desempeño y evaluacion piloto en función de la precisión, la exactitud, el recall, la F1-score, entre otras métricas.

### Video: ¿Cómo seleccionar el MEJOR MODELO en un problema de Machine Learning?
- Mejor modelo = Mejores predicciones
- Parametros: Variables numericas internas que el algoritmo aprende
- Hiperparámetros: Variables numericas externas, se dijan al programar el algoritmo.
- Afinacion de hiperparametro: Seleccion de mejores valores hiperparametros
- Para evaluar el modelos, se pude hacer:
    - Sets de entrenamiento, validacion y prueba.
    - Validacion cruzada y *k-fold cross-validation*.
- Prediccion: Calculo de valor numerico, apartir de datos numericos de entrada.
- Metrica de Desempeño: Formula matematica, que permite estimar la eficiencia del modelo. Eje: RMSE: Root Mean Square Error
![alt text](RMSE.JPG)
- Entre menor sea el valor de RMSE, mejores seran las predicciones
- **Modelos de ML:** Maquina de Soporte Vectorial, Bosque Aleatorio, Red Neuronal
- Aquel modelo que obtenga un RMSE menor, sera mejor la prediccion.
- El modelo tambien depende de la capacidad del equipo que corre el programa de ML.

6. **Despliegue**
Poner a trabajar el modelo en un entorno real.

### Video: El DESPLIEGUE en el Machine Learning (MLOps)
- Machine Learning Enginnering: Conjunt de practicas, que busca lograr el desplieuge de modelos de ML de forma *eficiente*.
- Requerimientos para elegir el tipo de despliegue:
    - Tipo de prediccion: En tiempo real (prediccion inmediata) o por lotes (prediccion no inmediata)
    - Latencia: Tiempo de respuesta requerido, desde la introduccion de la informacion y la prediccion
    - Rendimiento: Numero de solicitudes por segundo que pude aguantar el modelo
    - Complejidad del modelo: Capacidad de Maquina
    - Despliegue en la nube: Predicciones a traves de internet. Modelos complejos y de alta latencia.
    - Despliegue on the edge: En el dispositivo, modelos poco complejos y de baja latencia. (dispositivos moviles).
- Herramientas de despligue mas usadas: 
    - **Locales:** No permiten llevar el modelo a produccion. Se despliegan localmente
        - FlaskAPI: Empaqueta modelo como API, para ingresar desde nuestro navegador.
        - TensorFlow o TorchServe: Pocas lineas de codigo, permiten desplegar modelos localmente.
        - On the edge
    - **Out of the box:** 
        - StreamLite: Se aloja el codigo en un servidor, con ciertas restricciones de memoria y computo
    - **En la nube**
        - El computo se hace en servidores remotos. Eje: AWS, Google Could, etc.
        - Incluye todo el servicio de ML Operations


7. **Mantenimiento y actualizacion**
Monitoreo del desempeño del modelo en producción y realizar actualizaciones periódicas para mantener su precisión y relevancia. 

### Video: EL MONITORIO en el Machine Learning
- Machine Learning Operations!
- Desplegar el modelo no es la ultima fase del proceso, porque puede sufrir una degradacion en el desempeño
- Los fallos en el desempeño pueden ser por: Fallos de Software (factores externos) y Fallos del Modelo
    - Fallos del modelo: Los mas comunes son "Variacion en la distribucion". Deriva de datos y deriva de conceptos.
- Tipos de Monitoreo
    - Monitoreo con metricas globales: No permite ver ls razones de fondo que dan esa degradacion.
    - Monitoreo a traves de sitribuciones estadisticas: Periodicamente calcular pruebas estadisticas, y ver diferencias significativas, si las hay, habria deriva de datos. Si es razonablemente gradne, seria Deriva de Cooncepto.

## Material Complementario

### Video: ¿Qué hace un MLOps? Antonio Feregrino 



