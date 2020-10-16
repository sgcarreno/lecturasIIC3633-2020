# Carousel Personalization in Music Streaming Apps with Contextual Bandits

Este *paper* escrito por Bendada et al., trata de la aplicación de *multi-armed bandits* con múltiples jugadas a *apps* de música, en las que se entregan recomendaciones mediante carruseles de artistas, álbumes o listas de reproducción.

Antes de explicar la realación entre los *bandits* y su investigación, explican brevemente de qué se trata este tipo problemas, en la sección "*2.1 Background on Multi-Armed Bandits with
Multiple Plays*". Con esta explicación no se requiere mucho conocimiento previo acerca de este tema específico, ya que una o dos lecturas de esta breve sección, pueden ser suficientes para comprender el concepto de los *multi-armed bandits* con
*multiple plays*, y poder asociarlo al resto de la investigación.

La analogía que se hace entre los *multi-armed bandits* y el carrusel, es que cada *arm* correspondería a cierto ítem, formando con los K brazos un catálogo del tipo de ítem que se quiera recomendar. De estos K se seleccionarían L ítems, los que formarían el carrusel, y estos se irán actualizando cada ciertos intervalos de tiempo. Se ve que una aplicación como esta requiere de bastante conocimiento del uso de estas aplicaciones por parte de los usuarios, lo que se confirma luego, cuando explican cómo obtener el *feedback* desde qué tarjetas vio el usuario y cuáles quizo reproducir.

Antes de mostrar los resultados, enumeran los algoritmos que fueron ocupados con una explicación corta de cada uno. Si bien yo no pude comprender los objetivos y metodologías de todos ellos, creo que ese leve nivel de detalle en las explicaciones está bien para un *paper* cuyo enfoque principal no son aquellos algoritmos.

Finalmente se muestran los resultados, en los que el algoritmo *ts-seg-pessimistic* obtiene el mejor rendimiento en las evaluaciones *offline*. Estos resultados refleja la importancia de probar con varios algoritmos y no quedarse con los más comunes, ya que la diferencia entre ellos puede ser mucha, influyendo altamente en la calidad de las recomendaciones a realizar.