---
title: ¿Está muriendo JavaScript en favor de TypeScript?
tags:
  - Javascript
  - JS
  - Bable
  - Typescript
  - Developer
twitter_creator: BABELgrupo
date: 2018-10-17 12:37:47
---

{% asset_img Blog_JSDayEs_3.jpg '' %}
_Clickbait detected_. La verdad es que sí, el título de esta entrada solo tenía el propósito de llamar la atención.

Para empezar, cabe plantearse si la pregunta ¿Está muriendo JavaScript en favor de TypeScript? tiene sentido. Técnicamente hablando, el lenguaje TypeScript es un superset de JavaScript, o lo que es lo mismo, cualquier programa escrito en JavaScript plano es un programa TypeScript perfectamente válido. Además, no hay que olvidar que un programa escrito en TypeScript necesita ser “transpilado” a su correspondiente programa JavaScript, por lo que realmente (y de momento) no es concebible un TypeScript sin JavaScript.

<!-- more -->

{% asset_img encuesta1.png 'Encuesta sobre preferencias respecto a lenguajes de programación. StackOverflow 2018' %}
<center><small>[Encuesta sobre preferencias respecto a lenguajes de programación (StackOverflow 2018)](https://insights.stackoverflow.com/survey/2018/#technology-most-loved-dreaded-and-wanted-languages)</small></center>

Quizás habría que realizar el planteamiento de otra manera con una pregunta más adecuada: ¿Superará el uso de TypeScript al de JavaScript en el ecosistema del desarrollo web moderno?

El lenguaje JavaScript -en comparación a lenguajes orientados a objetos con tipado estático y con un sistema de herencia clásico- da al programador una mayor flexibilidad a la hora de implementar sus programas gracias a su herencia basada en prototipos y a su tipado dinámico, pero a cambio se traduce en un nivel extra de complejidad y mayor fragilidad respecto a errores y defectos. En decir, la habilidad del programador resulta fundamental a la hora de evitar bugs y lograr el funcionamiento deseado.

Allá por el año 2012, JavaScript se encontraba en su versión ECMAScript 5.1 y características tan comunes en nuestro día a día como son los módulos, las clases o las promesas aún no estaban disponibles de manera nativa. A lo largo de los últimos años y con el desarrollo del estándar de ECMAScript, se han ido incorporando características con el objetivo de mejorar, entre otras cosas, la expresividad del lenguaje, la legibilidad y la mantenibilidad del código.

Fue en este año 2012 que TypeScript apareció de la mano de Microsoft, con el objetivo de solventar los problemas que presentaban las aplicaciones JavaScript de un tamaño considerable -siendo estas principalmente la complejidad y modularidad del código-. Debido a la lentitud con la que el estándar ECMAScript podía avanzar para atajar estos problemas (y a su vez los navegadores soportar las especificaciones del estándar), TypeScript intentó ser la solución que tendiese al futuro del estándar ECMAScript frente a las herramientas que surgían para facilitar las labores de desarrollo.

A día de hoy algunas de las funcionalidades que ofrecía TypeScript han sido incluidas en el estándar de ECMAScript (clases, módulos, parámetros por defecto, etc.), pero todavía existen otras que no solo suponen disponer de un “azúcar sintáctico”, sino que proporcionan algunos beneficios al desarrollador que, a mi juicio, me parecen fundamentales en la cuestión que nos planteábamos al principio: comprobación de tipos en tiempo de compilación, integración con los IDEs actuales, buena navegabilidad a lo largo de la codebase y el famoso intellisense, mayor facilidad de adaptación a los proyectos, mejor compresión a la hora de integrar nuestro código con APIs implicadas, etc. Existen no obstante argumentos en contra del uso TypeScript, pero que no comentaré en esta entrada.

Por otro lado, TypeScript va integrándose más y más en las librerías y frameworks modernos, lo que ha motivado a los desarrolladores a adaptarnos a este lenguaje y, por tanto, a incrementar su uso. Sin embargo, a día de hoy, una comparación del uso de JavaScript frente a TypeScript queda bastante decantado hacia el primero.

{% asset_img encuesta2.png 'Encuesta de uso sobre lenguajes de programación. StackOverflow 2018' %}
<center><small>[Encuesta de uso sobre lenguajes de programación (StackOverflow 2018)](https://insights.stackoverflow.com/survey/2018/#technology-programming-scripting-and-markup-languages)</small></center>

Para finalizar la entrada, remarcar que el propósito principal de la misma no era más que reflexionar sobre cómo han evolucionado ambos lenguajes y el futuro que nos depara respecto a su uso. Por mi parte, y mientras TypeScript no dé un giro radical, intentaré utilizarlo siempre que pueda (y sea la solución adecuada) en mis futuros proyectos. Así que, si en un futuro el uso de TypeScript supera al de JavaScript (y sigo vivo en ese hipotético momento), sumaré mi granito de arena.

{% raw %}
<div class="sponsor" style="border-color: #e3692e">
  <a class="logo" href="https://babel.es/"><img src="babel.png"  alt="Babel"/></a>
  <div class="bio">
    <p>
      <strong>BABEL</strong> es una empresa internacional que presta servicios tecnológicos orientados a acompañar a grandes organizaciones en su proceso de Transformación Digital. Tenemos oficinas en Barcelona, Casablanca, Ciudad de México, Lisboa, Londres, Madrid, Querétaro y Sevilla.
    </p>
    <p>
      <a href="http://trabajaen.babel.es/">¿Te gustaría trabajar con nosotros?</a>
    </p>
  </div>
</div>
{% endraw %}

{% raw %}
<div class="post-author" style="border-color: #e3692e">
  <div class="bio">Por <strong>Jorge González Valencia</strong>, Desarrollador Sénior del Centro de Desarrollo de Movilidad de BABEL.</div>
  <img class="photo" src="Jorge Gonzalez Valencia.jpg" alt="" />
</div>
{% endraw %}
