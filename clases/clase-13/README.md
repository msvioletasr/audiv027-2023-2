# Space Invaders con comando de voz

Integrantes: Violeta Silva, Joaquín Suazo, Fae Ávila y Kamila Mansilla

Link a p5.js en Fullscreen: [https://editor.p5js.org/msvioletasr/full/TyKuLwPm0](https://editor.p5js.org/msvioletasr/full/vjKT1tBln)

Link a p5.js embed: https://editor.p5js.org/msvioletasr/full/vjKT1tBln

# Introducción:

Este proyecto consiste en un videojuego clásico de Space Invaders controlado por voz, haciendo uso de la Teachable Machine de Google

# Materiales: 

-Computador o celular

-Micrófono

-Conexión a internet

-Voz

-p5.js

-Teachable Machine

-p5js.org

-Tutoriales de Youtube

# Referentes:

Para este proyecto tomamos como referencia una serie de videos que enseñan a hacer el juego Space Invaders. Usamos estos videos como la base para crear el juego y entender cómo modificar lo que necesitáramos:

[Programming Space Invaders in P5.js - Part 1 ](https://www.youtube.com/watch?v=ZQ3M7cltjks&list=PLBDInqUM5B25FzygoJ9Ifg1TZXmIHz4zh)
- ![Captura de pantalla 2023-11-10 180553](https://github.com/joaquinsuazo/audiv027-2023-2/assets/128074599/5c704b62-451a-4aa1-b547-7ac9b12f89bc)

Para poder incorporar los comandos de voz usamos otro video tutorial como guía:

 [Coding Challenge #147: Chrome Dinosaur Game (with Speech Commands machine learning model!)](https://www.youtube.com/watch?v=l0HoJHc-63Q)
- ![Captura de pantalla 2023-11-10 175948](https://github.com/joaquinsuazo/audiv027-2023-2/assets/128074599/a76677ec-1b7b-46d4-b2cd-0270026c27da)

Además, usamos el conocimiento ya adquirido del trabajo anterior para crear el modelo entrenado e implementarlo p5.js

Por último, cualquier otra duda que teníamos consultamos p5js.org.

# Registro:

Para empezar sabíamos que queríamos seguir la línea del trabajo anterior, o sea, Sound Classification y comando de voz, pero ahora aplicado a un proyecto más complejo.

Nos interesó la idea de hacer un videojuego que se pudiera controlar con la voz, por lo que comenzamos a buscar en Youtube tutoriales para usar como referentes. De todos los que vimos, los videos sobre Space Invaders fueron nuestros favoritos, por lo que decidimos usar estos.

Fuimos recreando el código en p5 para lograr entender cómo funcionaba y poder editar lo que necesitáramos luego. Principalmente, vimos cómo funcionaban los comandos de movimiento y acciones como disparar.

Una vez hecho esto, entrenamos el modelo usando Teachable Machine con tres comandos: "Derecha", "Izquierda" y "Dispara":

https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/f204a541-1263-4556-87ca-ff4369441b00

https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/1237d86f-4296-44c5-959e-62635bd4abbf

A continuación se puede ver el modelo entrenado: 

![Screenshot_6](https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/7d465431-3cb8-4bf5-8271-58954043a329)

Luego de esto, exportamos el modelo a un sitio web para poder usar el modelo.json en el proyecto:

![Screenshot_7](https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/5b8a5885-ab65-41da-9810-5e19e0896fe4)

Esta vez usamos la función preload para incorporar nuestro modelo, ya que es lo que se hizo en el tutorial:

![Screenshot_10](https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/d0b0c72d-9907-41b6-b992-e9e2e28ff422)


Con el modelo ya entrenado, debíamos ahora incorporarlo al juego. Para esto, nos guiamos con el tutorial antes mencionado, en el que se muestra un código para ejecutar el comando:

![Screenshot_3](https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/c9eda465-da72-4dcf-8257-03bf81b345a2)

Le hicimos algunas modificaciones a este código. Primero, cambiamos el "up" a lo que había aprendido nuestro modelo, "derecha", "izquierda" y "dispara".

![Screenshot_1](https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/4b43e5a7-7644-4df7-acdf-fa3479021f9a)

Además, en vez de unicorn.jump, escribimos las acciones que la nave hacía con keyPressed, que se puede ver a continuación:

![Screenshot_4](https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/483d1358-5fa7-4e10-a365-a2a7b0246f6f)

En la siguiente imagen se pueden ver algunos de los comandos en el código final:

![Screenshot_5](https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/91863e11-0d96-4d68-9bb9-826c01480851)

En el siguiente video se ve el videojuego funcionando correctamente:

https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/6c1ac7e5-6502-4132-8157-2c207545bb17

Una vez hecho esto, el videojuego funcionaba correctamente y solamente quedaba ajustar algunos detalles para mejorar la experiencia del jugador.
Algunos de estos detalles fueron:

-Aumentar el timer a 60 segundos

-Aumentar la cantidad de pixeles que el jugador se mueve hacia la izquierda y derecha

-Hacer que los enemigos se muevan más lento y bajen menos cada línea

-Cambiar los gráficos a unos propios hechos por la integrante Kamila Mansilla

-Traducir el texto a español y escribir las instrucciones correctas

A continuación se puede ver cómo era el videojuego base del tutorial:

![Screenshot_8](https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/cadd6a24-e47b-40c8-a185-29b564a06fc2)

Y nuestro videojuego final:

![Screenshot_9](https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/c5972c55-2ed6-4e8e-9d6e-d4d86f20bb6c)

Junto a un video funcionando:

https://github.com/msvioletasr/audiv027-2023-2/assets/142625864/c942cca1-3177-4ff5-83c6-b72d817cbe0a

# Conclusión

En conclusión, sentimos que gracias a la experiencia adquirida del trabajo anterior no nos fue tan difícil incorporar el modelo a nuestro trabajo. 

Lo más desafiante de este proyecto fue que ahora debíamos hacer que los comandos movieran la nave, en vez de solamente identificar nuestras voces. No habían muchos tutoriales sobre cómo hacer esto, pero el que encontramos fue extremadamente util. Tuvimos algunos problemas que solamente pudimos solucionar mediante prueba y error, ya que no había información tan específica para esos casos.

Además, siguiendo los tutoriales, logramos comprender por qué el código funciona, ya que incorporamos los distintos elementos poco a poco. Esto nos permitió hacer cambios luego a cosas específicas, como el tamaño de los elementos, el timer, colores, etc.

Pudimos ver que hay oportunidades muy interesantes para crear todo tipo de cosas en p5.js usando la inteligencia artificial, sobretodo ahora que es más accesible. 
