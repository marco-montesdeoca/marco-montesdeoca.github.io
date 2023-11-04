## Proyectos

### Nube de palabras

Una imagen vale más que 1000 palabras. Una manera interesante de resumir el contenido de un texto es mediante las nubes de palabras. En este tipo de visualización, las palabras más frecuentes de un texto se destacan en mayor tamaño. En este script resumimos el contenido de la constitución de Chile vigente, así como de la propuesta de constitución 2023.

Aquí tenemos la nube de palabras del documento actual:
<img src="https://raw.githubusercontent.com/marco-montesdeoca/nubes_de_palabras/main/actual.png" width="1000" height="750">

Y la nube de palabras de la propuesta 2023:
<img src="https://raw.githubusercontent.com/marco-montesdeoca/nubes_de_palabras/main/propuesta.png" width="1000" height="750">

¿Qué cambios puedes notar?

### Impacto del aprendizaje por transferencia en la clasificación de imágenes por inteligencia artificial

La inteligencia artificial (IA) ha demostrado su potencial en múltiples campos, incluida la clasificación de imágenes. Los modelos masivos como [ResNet50](https://arxiv.org/abs/1512.03385) pueden clasificar miles de entidades regulares distintas, como automóviles o animales, y se entrenaron con millones de imágenes etiquetadas. Sin embargo, sus aplicaciones pueden ir más allá de sus objetivos iniciales con una metodología conocida como aprendizaje por transferencia (TL). Con TL podemos reorientar un modelo potente como ResNet50 hacia un problema de clasificación de nuestro interés. A continuación hacemos uso de este modelo implementado en la librería [Keras](https://keras.io/) aplicando TL para clasificar imágenes de dos tipos de datos. En primer lugar clasificamos imágenes histológicas de tejido de colon normal y canceroso. Luego, aplicamos este método para clasificar imágenes de limones de alta y baja calidad.

<img src="https://raw.githubusercontent.com/marco-montesdeoca/marco-montesdeoca.github.io/main/TL%20impact02.png" width="500" height="300">

En el gráfico se aprecia cómo aplicando aprendizaje por transferencia el modelo ResNet50 sube desde un 47% hasta un 99% de exactitud al clasificar imágenes histológicas de tejido de colon normal y canceroso. De manera similar, al aplicar aprendizaje por transferencia el modelo sube desde un 75% hasta un 98% de exactitud al clasificar imágenes de limones de alta y baja calidad. 
El potencial de este tipo de metodología es sin duda impresionante.

* [Ver código clasificación imágenes histológicas de cáncer de colon](https://github.com/marco-montesdeoca/Transfer_learning/blob/main/transfer_learning.ipynb)
* Código clasificación imágenes de calidad de limones estará disponible pronto.

### Matriz de identidad

Determinar la identidad entre secuencias es clave. Nos ayuda a entender las relaciones evolutivas entre aislados, o a inferir la función de una secuencia nueva, entre otros. En el siguiente script en Python podemos ver como aplicar alineamientos locales de secuencias mediante el algoritmo Smith-Waterman.

<img src="https://raw.githubusercontent.com/marco-montesdeoca/marco-montesdeoca.github.io/main/identity_matrix.png" width="300" height="300">

En el clustermap se destacan dos grupos o clusters de secuencias con mayor identidad. ¿Qué secuencias son más idénticas entre sí? Puedes revisar a qué virus corresponden copiando sus nombres (sin incluir la extensión ".fasta") y buscándolos en la base de datos [NCBI](https://www.ncbi.nlm.nih.gov/). 

* [Ver código](https://github.com/marco-montesdeoca/identity_matrix/blob/main/identity_matrix.ipynb)

### Expresión diferencial

La secuenciación de ARN mediante tecnologías de alto rendimiento permiten desvelar patrones de expresión. En el siguiente script en R vemos como analizar estadísticamente las diferencias de expresión.

<img src="https://raw.githubusercontent.com/marco-montesdeoca/marco-montesdeoca.github.io/main/volcano_plot.png" width="300" height="300">

Los resultados se pueden resumir en un gráfico de volcán, donde las diferencias de expresión se indican como un factor de cambio. En el gráfico, los puntos hacia la derecha del cero indican genes con mayor expresión en la condición tratamiento con respecto a la condición control. Los puntos hacia la izquierda del cero indican lo contrario, menor expresión en la condición tratamiento con respecto a la condición control. Sin embargo, solo los puntos de color rojo se consideran estadísticamente significativos. ¿Qué genes poseen expresión diferencial según el gráfico? Para más detalles acerca del origen de los datos puedes revisar el script.

* [Ver código](https://github.com/marco-montesdeoca/Differential_expression/blob/main/Differential_expression.ipynb)

[Volver al menú principal](index.md)
