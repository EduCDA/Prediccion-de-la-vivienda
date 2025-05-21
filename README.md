# Predicción del Precio de la Vivienda

## Objetivo
Este repositorio tiene como objetivo predecir el precio de una vivienda utilizando un modelo de redes neuronales entrenado con datos reales de viviendas. El modelo tiene en cuenta diversas características de la vivienda para estimar su precio de manera precisa.

## ¿Cómo funciona?
El sistema está implementado como una API desarrollada en Flask. El flujo de funcionamiento es el siguiente:

1. **Entrenamiento y modelo**: El modelo de red neuronal ha sido previamente entrenado con un conjunto de datos de viviendas y se encuentra almacenado en la carpeta `modelos/`.
2. **API principal**: El archivo `main.py` contiene la lógica principal de la API. Aquí se cargan el modelo y los transformadores necesarios para procesar los datos de entrada y realizar la predicción.
3. **Pruebas**: El archivo `test_api.py` permite enviar datos de prueba a la API. Simplemente modifica los valores de las características de la vivienda en este archivo para probar diferentes escenarios.

## ¿Cómo probarlo?
Sigue estos pasos para probar la API y el modelo:

1. **Ejecuta la API**
   
   Abre una terminal en la carpeta `api_redneuronal` y ejecuta:
   
   ```bash
   py main.py
   ```
   Esto iniciará el servidor Flask y dejará la API escuchando peticiones.

2. **Modifica los datos de prueba**
   
   Abre el archivo `test_api.py` y edita los valores de las características de la vivienda que deseas predecir. Puedes cambiar los datos para simular diferentes viviendas.

3. **Ejecuta el script de prueba**
   
   En la misma terminal (o en otra), ejecuta:
   
   ```bash
   py test_api.py
   ```
   El script enviará los datos a la API y mostrará por consola:
   - El precio real esperado (si lo incluiste en los datos)
   - El precio predicho por el modelo
   - La diferencia entre ambos valores

## Estructura principal del repositorio
- `api_redneuronal/main.py`: Lógica principal de la API y del modelo.
- `api_redneuronal/test_api.py`: Script para probar la API con diferentes datos de vivienda.
- `api_redneuronal/modelos/`: Carpeta donde se almacena el modelo entrenado.
- `api_redneuronal/archivos_transformers/`: Transformadores para preprocesar los datos.

## Requisitos
- Python 3.x
- Las dependencias necesarias están listadas en `requirements.txt`.

## Notas
- Puedes modificar y ampliar los datos de entrada según las características de las viviendas que desees analizar.
- El modelo puede ser reentrenado con nuevos datos para mejorar la precisión.

---

¡Esperamos que este proyecto te ayude a predecir precios de viviendas de manera eficiente y sencilla!
