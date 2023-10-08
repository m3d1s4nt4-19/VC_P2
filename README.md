# P2 - Funciones básicas de OpenCV

## Desarrollo

### Tarea 1 - Cuenta de píxeles blancos por fila, máximo para filas y columnas y nº de valores mayores

  Para esta tarea, se toman todas las filas de la imagen en gris, y tras eliminar la última fila, que está completamente en blanco, se comprueba qué  fila  tiene más píxeles blancos, y  tras multiplicar con el umbral, se calcula las filas  que lo superan.

  De igual manera con las columnas, la imagen es separada por columnas normalizando el ccolor a la escala de grises, y tras seleccionar los valores máximos de esta división, se realiza la umbralización.

  En ambos casos se utilizan funciones de la librería matplotlib para mostrar la imagen y la gráfica que muestra las concentración

### Tarea 2 - Aplicación de Sobel a otra imagen

  En esta tarea, se ha seleccionado una imagen, y se han hecho copias a color, en gris, y en gris tras aplicar la gaussiana, todo mediante el uso de funciones de la librería OpenCV. Con la última de estas imágenes se han realizado las transfromaciones de Sobel, que se muestran posteriormente con la librería matplotlib.

### Tarea 3 - Umbralizado a la imagen resultante de Sobel + conteo de columnas y filas.

  Para el umbralizado, se ha seleccionado un número que permita ver una imagen similar a la original en el resultado,   100 en este caso. Con la función treshold de OpenCV se aplica el umbral a la foto de la tarea anterior, y con el procedimimento de la tarea 1, se obtienen las filas y columnas que superan el umbral que se calculó previamente.

### Tarea 4 - Commportamiento de las funciones para mostrarle a alguien que no cursa la asignatura

  En este caso, creo que la Laplaciana es una función muy útil para la vida diaria, en muchos ámbitos. Detectar bordes es práctico para muchos contextos, por lo que creo que además, verlo en tiempo real es aún más impresionante.

### Tarea 5 - Reinterpretación del procesamiento de imágenes.

  Para esta tarea, he incluido algo que considero interesante. Probando con la modificación de los canales de colores en la práctica 1, encontré una configuración extraña. Supongamos que las siglas RGB son una string que podemos rotar. Pues al restarle la mitad del "siguiente" valor de la rotación, se puede obtener una especie de filtro de color piel en algunos casos.

  Por ejemplo, en el primer caso:
  R -> G
  G -> B
  B -> R

  Por lo que resulta en:
  R' = R - G/2
  G' = G - B/2
  B' = B - R/2

  
