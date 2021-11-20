# Tarea 10-11 Sistemas inteligentes

## Archivo preprocessing.py
El programa preprocessing.py se encarga de leer un archivo de texto llamado amazon_cells_labeled.txt

Este programa quita las comillas del texto, y reemplaza todas las mayúsculas con minúsculas, y genera un archivo en formato .arff llamado "amazon" con las especificaciones y tags que solicita Weka para su lectura.

Los nombres de los archivos de entrada y salida pueden ser modificados en la línea 72.

El comando para ejecutar el programa es:
    python3 preprocessing.py

## Archivo knn-algorithm.py
Una vez que se generó el archivo amazon.arff, este es ingresado a Weka, que se encarga de convertir los atributos de las cadenas en un conjunto de atributos numéricos que representan la información de ocurrencia de palabras del texto contenido en las cadenas.

Posteriormente, el programa knn-algorithm.py se encarga de utilizar esos datos procesados, que fueron exportados en el archivo de processed_data.csv, e implementar el método de clasificación supervisada conocido como k-nn. Si se desea, el nombre del archivo de entrada puede ser modificado en la línea 6.

De la misma forma, en la línea 19 se puede modificar el número de vecinos con los que se realizará la ejecución.

El programa imprime en consola la matriz de confusión y las métricas de precision, recall, y f-score.

El comando para ejecutar el programa es:
    python3 knn-algorithm.py