# Performance of Recommender Algorithms on Top-N Recommendation Tasks

En este *paper*, escrito por Cremonesi, Koren y Turrin, se evalúan distintos métodos de filtrado colaborativo, adaptado para recomendaciones de modo Top-N. Para probar los algoritmos, se usaron los *datasets* de Movielens y Netflix.

Para llevar a cabo esta tarea, primero que todo, adaptaron los datos originales para crear un nuevo set de *test*. Se creó un *test set T* que contiene todos los *ratings* de 5 estrellas puestos por los diferentes usuarios. Así, si la película *i*, con calificación perfecta para el usuario, al compararla con otras 1000 películas al azar y sin calificar, se encuentra dentro de las N recomendaciones entregadas para él, se tendría un éxito. Esto me pareció creativo y arriesgado a la vez, ya que no se parece a las otras formas de evaluar el rendimiento de un algoritmo.

Se podría considerar que una película de 4 estrellas sí es recomendable.

Matriz Train (M) = Netflix Train

Matriz Test (T) = ratings de 5 estrellas

eligen 1000 items al azar no rankeados por el usuario u

nueva forma de marcar éxitos. Se asume que si el ítem *i* entra en el top-N (con otros ítems que no debieran ser del interés del usuario), la recomendación está correctamente realizada.

Explican y justifican de buena forma las decisiones que toman, realizando comparaciones con otros métodos, como por ejemplo, la no normalización de los ratings.

Idea de quitar los elementos más populares, incrementó rendimientos, como el de cor-kNN.