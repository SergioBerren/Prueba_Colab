# # Introducción al Machine Learning con una predicción simple

## Objetivo del ejercicio

Este ejercicio está pensado como una introducción al Machine Learning para estudiantes que no tienen conocimientos previos sobre esta área.

La idea es utilizar un ejemplo sencillo para explicar cómo los datos pueden utilizarse para encontrar relaciones entre variables y realizar predicciones básicas.

En este caso se utilizará un dataset que relaciona la temperatura con las ventas de helados. El objetivo será comprobar si existe una relación entre ambas variables y utilizar un modelo sencillo para predecir las ventas a partir de la temperatura.

La duración estimada de la sesión es de entre 60 y 90 minutos.

---

## Dataset

Archivo: icecream_sales_temperature.csv

El dataset contiene tres columnas:

day  
Fecha del registro.

temperature_c  
Temperatura en grados Celsius.

icecream_sales  
Número de helados vendidos ese día.

El objetivo del ejercicio es predecir el número de helados vendidos en función de la temperatura.

Antes de comenzar con el modelo se plantea al alumnado una pregunta sencilla:

Cuando hace más calor, ¿se venden más helados?

La idea es utilizar los datos para comprobar si esta intuición se cumple.

---

## Conceptos que introduciría en clase

Durante la sesión se introducirían algunos conceptos básicos necesarios para entender el ejercicio.

### Dataset

Primero se explica qué es un dataset. Se puede definir como un conjunto de datos organizados normalmente en forma de tabla, donde cada fila representa una observación y cada columna representa una variable.

### Variables

También se explica qué es una variable y la diferencia entre variable independiente y variable dependiente.

En este ejercicio:

La temperatura sería la variable independiente, ya que es la variable que utilizamos para intentar explicar otra.

Las ventas de helados serían la variable dependiente, ya que es la variable que queremos predecir.

### Exploración de datos

Antes de construir cualquier modelo es importante explorar los datos. Para ello se utilizan herramientas de pandas que permiten ver las primeras filas del dataset, conocer los tipos de datos o calcular estadísticas básicas.

### Visualización de datos

La visualización ayuda a entender mejor los datos. En este ejercicio se utilizan gráficos sencillos como histogramas y gráficos de dispersión para observar la distribución de la temperatura y la posible relación entre temperatura y ventas.

### Modelo predictivo

Una vez entendidos los datos se introduce el concepto de modelo de Machine Learning. En este caso se utiliza una regresión lineal, que es uno de los modelos más sencillos.

La regresión lineal intenta encontrar una línea que represente lo mejor posible la relación entre dos variables.

---

## Preguntas que haría al grupo

Durante la sesión se pueden realizar algunas preguntas para fomentar la participación del alumnado.

Por ejemplo:

¿Creéis que existe relación entre la temperatura y las ventas de helados?

Si mañana la temperatura fuese de 35 grados, ¿pensáis que se venderían más o menos helados que en un día de 20 grados?

Observando el gráfico de dispersión, ¿qué patrón observáis?

¿Creéis que la temperatura es el único factor que puede influir en las ventas de helados?

En este último caso normalmente aparecen ideas interesantes como la lluvia, el día de la semana, si es fin de semana, si hay turismo o si es periodo de vacaciones.

---

## Actividad práctica para los estudiantes

Una vez explicado el ejercicio se propone una pequeña actividad para que los estudiantes experimenten con el código.

### Ejercicio 1

Modificar la temperatura utilizada en la predicción final.

Por ejemplo, en lugar de utilizar:

model.predict([[30]])

Probar con otras temperaturas como 25 o 35 grados y observar cómo cambia el resultado.

Después se puede preguntar a los estudiantes si el resultado tiene sentido.

### Ejercicio 2

Añadir un nuevo dato al dataset con una temperatura más alta, por ejemplo 40 grados, y pensar aproximadamente cuántos helados podrían venderse.

Después se puede comparar la estimación del alumnado con la predicción del modelo.

### Ejercicio 3

Modificar el dataset añadiendo un nuevo registro con valores inventados y observar si cambia la visualización del gráfico.

Esto permite entender cómo los datos afectan al modelo.

---

## Partes que podrían resultar más complicadas para el alumnado

### Comprender la regresión lineal

Para estudiantes sin conocimientos matemáticos el concepto de regresión puede resultar abstracto.

Una forma sencilla de explicarlo es decir que el modelo intenta dibujar una línea que pase lo más cerca posible de todos los puntos del gráfico.

Los puntos representan los datos reales y la línea representa la tendencia general que el modelo ha aprendido.

### Entender cómo aprende el modelo

También puede resultar difícil entender qué significa que el modelo "aprenda".

Una explicación sencilla es que el modelo analiza los ejemplos que le damos y busca una relación entre las variables.

Es parecido a cuando una persona aprende a estimar precios después de haber visto muchos ejemplos.

### Comprender el train-test split

La división entre datos de entrenamiento y datos de prueba también puede generar dudas.

Se puede explicar de forma sencilla diciendo que una parte de los datos se utiliza para que el modelo aprenda y otra parte se guarda para comprobar si realmente ha aprendido bien.

Una analogía útil es pensar en estudiar con ejercicios y después hacer un examen con preguntas nuevas.

---

## Tecnologías utilizadas

Este ejercicio utiliza las siguientes herramientas:

Python  
pandas  
matplotlib  
scikit-learn

---

## Instalación de dependencias

Para instalar las librerías necesarias se puede utilizar:

pip install -r requirements.txt
