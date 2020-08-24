# BPR: Bayesian Personalized Ranking from Implicit Feedback

Este *paper*, escrito por autores de la Universidad de Hildesheim, muestra cómo, a través de un método probabilístico basado en Bayes, se le puede entregar a un usuario un *ranking* personalizado de ítems que le puedan interesar.

Uno de los aspectos que me interesó de esta lectura, es que todas las explicaciones eran formalizadas en notación matemática, definiendo cada conjunto y fórmula por utilizar. Esto, si bien me complicó bastante debido a mi falta de práctica en ese ámbito, me pareció imprescindible para la calidad de métodos que fueron propuestos en este *paper*, ya que tenía un enfoque extremadamente matemático; a mi juicio, bastante más que las lecturas anteriores.

En cuanto a los resultados, esta investigación deja bastante claro lo importante que puede llegar a ser realizar una optimización de los métodos del estado del arte. Aquí los autores explican de manera corta y precisa los dos métodos que decidieron optimizar (MF y kNN) y explicaron por qué su algoritmo LearnBPR podía adaptar y mejorar sus resultados.

Me pareció pertinente también que utilizaran un breve espacio al final del *paper* para mencionar que se compararon los resultados con los métodos de rankings no personalizados. No se necesitó de una gran explicación para señalar que los resultados de los mejores métodos de rankings personalizados sobrepasan por una gran cantidad a los resultados de cualquier método con ranking no personalizado.

Esta optimización bayesiana para sistemas recomendadores, es definitivamente una forma conveniente de mejorar las recomendaciones para métodos de gradiente descendiente. Y a pesar de ser un algoritmo complejo de obtener y demostrar, su aplicación no resulta del todo difícil, según lo que yo percibí. Sin duda este ha sido un gran aporte al mundo RecSys, y eso lo evidencian los buenos resultados mostrados en esta investigación.