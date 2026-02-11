# Algoritmos de Visión Artificial y Conteo de Objetos

Este repositorio consolida la implementación de técnicas fundamentales de Procesamiento Digital de Imágenes (PDI) utilizando Python y OpenCV.

El proyecto culmina con una aplicación práctica de detección y conteo automático de dados en secuencias de video, aplicando segmentación por color y morfología matemática.

## Funcionalidad Destacada: Contador de Dados
Se procesan videos de "tiradas" de dados para identificar el resultado numérico.
* Segmentación: Separación del objeto (dado) del fondo mediante umbralización.
* Morfología Matemática: Uso de operaciones de Clausura (Closing) y Erosión para eliminar ruido y separar objetos conectados.
* Etiquetado de Componentes Conexos: Para contar los puntos (pips) o identificar los dados individuales.

## Módulos Técnicos

### 1. Preprocesamiento y Mejora
Implementación de técnicas básicas para preparar las imágenes antes del análisis complejo:
* Transformaciones de Intensidad: Ajustes de brillo y contraste para normalizar condiciones de luz.
* Ecualización de Histogramas: Mejora automática del contraste global.

### 2. Detección de Bordes y Umbralización
Extracción de características estructurales de la imagen:
* Filtros de Bordes: Implementación de operadores Sobel y Laplaciano para destacar contornos.
* Umbralización Automática (Otsu): Algoritmo para encontrar el umbral óptimo de binarización sin intervención manual, fundamental para la segmentación dinámica.

### 3. Morfología y Segmentación por Color
Técnicas avanzadas para el aislamiento de objetos específicos:
* Espacios de Color: Conversión y filtrado en espacios HSV/RGB para aislar objetos por su crominancia.
* Operaciones Morfológicas: Definición de Elementos Estructurantes (kernels) para dilatar, erosionar y limpiar máscaras binarias.

## Tecnologías
* Python 3
* OpenCV (cv2): Librería principal de visión computacional.
* NumPy: Manipulación matricial de imágenes.
* Matplotlib: Visualización de resultados e histogramas.

## Estructura del Repositorio
* /src: Scripts con la lógica de procesamiento.
* /videos: Archivos de entrada ("tiradas") para probar el algoritmo de conteo.
* /docs: Consignas y documentación técnica de los métodos implementados.

---
*Desarrollado en el marco de la asignatura Procesamiento Digital de Imágenes - Tecnicatura Universitaria en Inteligencia Artificial (UNR).*
