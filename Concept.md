# Aprendizaje Semi-supervisado
Qué es:
El aprendizaje semi-supervisado es un enfoque híbrido que combina datos etiquetados y no etiquetados. 
En el contexto de Word2Vec, aunque las palabras no tienen etiquetas explícitas, 
se utilizan las relaciones contextuales entre palabras para crear ejemplos de entrenamiento automáticamente.

Para qué sirve:

Aprovechar grandes cantidades de texto no etiquetado

Generar datos de entrenamiento automáticamente a partir del contexto

Superar la limitación de necesitar datos etiquetados manualmente

Cómo se aplica:
Se utilizan las palabras del contexto como "etiquetas" implícitas. Por ejemplo, en la frase 
"el gato persigue al ratón", si tomamos "persigue" como palabra central, las palabras "el", "gato", "al", 
"ratón" sirven como contexto para crear ejemplos de entrenamiento.

# Skip-gram
Qué es:
Skip-gram es una arquitectura de Word2Vec que predice las palabras del contexto a partir de una palabra central.

Para qué sirve:

Capturar relaciones semánticas entre palabras

Funcionar bien con corpus pequeños

Ser eficiente para palabras poco frecuentes

Cómo se aplica:

Se representa la palabra central como one-hot encoding

Se pasa por una capa oculta para obtener el embedding

Se usa softmax en la capa de salida para predecir palabras del contexto

El objetivo real es obtener los pesos de la capa oculta (los embeddings)

# Qué es el entrenamiento de un modelo Word2Vec propio 
Es el proceso de crear embeddings desde cero utilizando nuestro propio corpus de texto, en lugar de usar modelos pre-entrenados.

# Evaluación del Modelo con Datasets de Analogías
Qué es la evaluación con datasets de analogías
Es un método formal para medir la calidad de los embeddings utilizando conjuntos de datos predefinidos que contienen relaciones semánticas y sintácticas entre palabras.

Para qué sirve
Cuantificar objetivamente la calidad del modelo

Comparar diferentes modelos o configuraciones

Identificar fortalezas y debilidades en relaciones específicas

Cómo se aplica
Se utiliza un conjunto de analogías como "A es a B como C es a D" y se mide si el modelo puede predecir correctamente D dado A, B y C.

# Qué es t-SNE (t-distributed Stochastic Neighbor Embedding)

Es una técnica de reducción de dimensionalidad no lineal que permite visualizar datos de alta dimensión en 2D o 3D preservando las relaciones locales entre puntos.

Para qué sirve en NLP
Visualizar cómo se distribuyen los embeddings en el espacio

Identificar clusters de palabras semánticamente relacionadas

Verificar si el modelo captura relaciones semánticas esperadas

Cómo se aplica
Se seleccionan palabras para visualizar

Se obtienen sus vectores de embedding

Se reduce la dimensionalidad con t-SNE

Se visualizan en 2D/3D

