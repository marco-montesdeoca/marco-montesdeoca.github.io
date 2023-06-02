## Proyectos

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
