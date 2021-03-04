# Chest-X-Ray-Abnormality_Detection
 Chest X-Ray Abnormality Detection
Este proyecto trata de resolver la problemática que tienen los radiólogos de identificar y diagnosticar un tipo de anomalía de tórax en una radiografía mediante la aplicación del modelo de detección y clasificación YOLOv5.

Partiendo de un dataset de 18000 imágenes y un csv con las coordenadas de los bounding boxes y la clase de anomalía que se detecta en cada uno de ellos, se pretende adaptar el modelo YOLOv5 pre entrenado con el dataset COCO para que sea capaz de diagnosticar este tipo de anomalías. En este caso se aplica aprendizaje por transferencia, aprovechando el modelo pre entrenado y entrenando las últimas capas para las clases y las imágenes que aplican al problema. 

El cuaderno YOLOv5s.ipynb contiene el código utilizado durante toda la fase de análisis, entrenamiento y aplicación del modelo en un conjunto de test. 

Los scripts train.py test.py y detect.py son los utilizados para el entrenamiento, validación y test del modelo.

El archivo vinbigdaka.yaml es el que contiene la configuración para el entrenamiento del modelo. En él se especifican las clases, el número de clases y la ubicación de los datos de entrenamiento y validación.

El archivo hyp.yaml es el utilizado para modificar los hyperparametros del modelo. 