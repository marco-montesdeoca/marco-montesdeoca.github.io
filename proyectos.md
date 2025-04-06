## Projects

### Word Cloud

A picture is worth a thousand words. One interesting way to summarize the content of a text is through word clouds. In this type of visualization, the most frequent words in a text are displayed in larger font size.

In this script, we summarize the content of the current Chilean Constitution, as well as the proposed 2023 Constitution.
Here is the word cloud of the current document:
<img src="https://raw.githubusercontent.com/marco-montesdeoca/nubes_de_palabras/main/actual.png" width="1000" height="750">

And the word cloud for the 2023 proposal:
<img src="https://raw.githubusercontent.com/marco-montesdeoca/nubes_de_palabras/main/propuesta.png" width="1000" height="750">
What changes can you notice?
If you want to learn how to generate your own word cloud from any PDF file, check out the script. [here](https://github.com/marco-montesdeoca/nubes_de_palabras/blob/main/Nube_de_palabras.ipynb)

### Impact of Transfer Learning on Image Classification with Artificial Intelligence

Artificial Intelligence (AI) has shown its potential in multiple fields, including image classification. Massive models such as [ResNet50](https://arxiv.org/abs/1512.03385) can classify thousands of distinct regular entities, such as cars or animals, and were trained on millions of labeled images. However, their applications can go beyond their initial goals through a methodology known as Transfer Learning (TL). With TL, we can redirect a powerful model like ResNet50 toward a classification problem of our own interest.

Below, we use this model implemented in the [Keras](https://keras.io/) library, applying TL to classify two types of data.  
First, we classify histological images of normal and cancerous colon tissue.  
Then, we apply this method to classify images of high- and low-quality lemons.

<img src="https://raw.githubusercontent.com/marco-montesdeoca/marco-montesdeoca.github.io/main/TL%20impact02.png" width="500" height="300">

In the chart, we can see how applying transfer learning allows the ResNet50 model to improve from 47% to 99% accuracy when classifying histological images of normal and cancerous colon tissue.  
Similarly, by applying transfer learning, the model improves from 75% to 98% accuracy when classifying images of high- and low-quality lemons.  

The potential of this type of methodology is undeniably impressive.

* [View code for histological image classification of colon cancer](https://github.com/marco-montesdeoca/Transfer_learning/blob/main/transfer_learning.ipynb)

### Identity Matrix

Determining sequence identity is key. It helps us understand the evolutionary relationships between isolates or infer the function of a new sequence, among other applications.  
In the following Python script, we demonstrate how to apply local sequence alignments using the Smith-Waterman algorithm.

<img src="https://raw.githubusercontent.com/marco-montesdeoca/marco-montesdeoca.github.io/main/identity_matrix.png" width="300" height="300">

In the clustermap, two groups or clusters of sequences with higher identity stand out.  
Which sequences are more identical to each other?  
You can check which viruses they correspond to by copying their names (excluding the ".fasta" extension) and searching for them in the [NCBI](https://www.ncbi.nlm.nih.gov/) database. 

* [View code](https://github.com/marco-montesdeoca/identity_matrix/blob/main/identity_matrix.ipynb)

### Differential Expression

RNA sequencing using high-throughput technologies allows us to uncover expression patterns.  
In the following R script, we demonstrate how to statistically analyze expression differences.

<img src="https://raw.githubusercontent.com/marco-montesdeoca/marco-montesdeoca.github.io/main/volcano_plot.png" width="300" height="300">

The results can be summarized in a volcano plot, where expression differences are represented as a fold change factor.  
In the plot, points to the right of zero indicate genes with higher expression in the treatment condition compared to the control condition.  
Points to the left of zero indicate the opposite, lower expression in the treatment condition compared to the control condition.  
However, only the red points are considered statistically significant.  

Which genes show differential expression according to the plot?  
For more details about the data source, you can review the script.

* [View code](https://github.com/marco-montesdeoca/Differential_expression/blob/main/Differential_expression.ipynb)

[View code](index.md)
