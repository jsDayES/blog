---
title: Como escalar los equipos en el desarrollo web empresarial
tags:
  - angular
  - development
  - gft
  - management
  - team building
  - web
twitter_creator: gft_es
date: 2018-10-18 10:02:36
---

{% asset_img Matrioskes.jpg '"Matrioskes" por Miquel Bohigas Costabella' %}

  Para muchos de nosotros, el desarrollo web es, simplemente, apasionante. Estar al tanto de las últimas tendencias en desarrollo, los últimos cambios de nuestro framework de cabecera o incluso de sus competidores, son parte de nuestro día a día. Por ese motivo, seguramente, estás ahora leyendo este artículo en el blog de JSDayES.

  Aun así, es todo un reto -en este escenario tan cambiante- trasladar todo esto a nuestros proyectos profesionales. Si pensamos en el escenario del desarrollo empresarial donde, normalmente, no desarrollamos una aplicación solos sino que trabajamos en equipos de 5, 15 o 50 desarrolladores, nos enfrentamos al reto de adoptar las mejores prácticas de manera uniforme por todo el equipo.

<!-- more -->

  No voy a extenderme mucho en el detalle de los problemas que este escenario requiere superar por no hacer este artículo interminable. Hablemos de las soluciones. Ya sea definiendo arquitecturas reusables para múltiples proyectos, o trabajando en el liderazgo técnico de un proyecto suficientemente grande, estas prácticas te ayudarán.

### 1. Pon al desarrollador en el centro

Nuestro objetivo es extender las buenas prácticas y tener coherencia en los desarrollos. La mejor manera de conseguirlo es ponérselo fácil al desarrollador. Un desarrollador no quiere tener que escribir código que no le aporte valor a la solución. En ese principio se basan todos los asistentes de los IDEs durante los últimos 15 años.

Aquí puedes ayudar en dos etapas, cuando estamos comenzando una tarea y cuando estamos ejecutándola. Son dos puntos en los que podemos ayudar de diferentes maneras. En nuestra iniciativa FAST hemos creado un conjunto de herramientas que permiten ayudar a los desarrolladores, por ejemplo, desplegando un portal del desarrollador donde encontraremos todos los enlaces a la documentación.

Esto no parece muy innovador ¿no? Además, debe de permitirnos comenzar el trabajo. En nuestro caso, el portal también permite parametrizar el desarrollo que vas a comenzar y crearte la estructura de proyecto, ponerla en un nuevo repositorio git, asociar unos pipes de integración continua que se pasarán desde el primer minuto, …  incluso podríamos añadir una tarea en las pipes que acabamos de crear para que publique la documentación en el portal de manera automática y en el primer minuto.

{% asset_img UI1.png %}

### 2. Súbete a hombros de gigantes

Construir ese portal de desarrollador que hemos nombrado antes desde cero parece una tarea muy grande y lo es. Nosotros hemos acometido este proyecto integrando herramientas de terceros. Del mismo modo que usamos Angular para crear la aplicación, decidimos integrarnos con los CLI de cada herramienta a la que demos soporte. De este modo, podemos añadir soporte a nuevas tecnologías o herramientas.

Así, por ejemplo, nuestro portal se apoya en Docker para soportar la creación de múltiples proyectos en paralelo sin interferencias. Y mientras estás ejecutando la creación puedas, incluso, modificar los comandos que se ejecutan con una consola interactiva web.

¿Sólo en el servidor?

No, en nuestro caso, esta misma herramienta puede ejecutarse en cliente para ser el perfecto compañero del desarrollador. En este caso, deja de utilizar Docker para ejecutar todo en local y toman mayor relevancia sus capacidades para mantener el entorno del desarrollador actualizado, y dar soporte a la ejecución de tareas y no sólo al comienzo de las mismas.

{% asset_img UI2.png %}

La FAST UI es una aplicación que agrega y encadena la ejecución de distintas herramientas command line para completar flujos de trabajo fácilmente aprovechando el gran trabajo realizado por terceros.

{% asset_img UI3.png %}

Uno de los grandes fracasos de este tipo de herramientas es intentar ser:

- **Omnipotentes**: Es mejor hacer pocas cosas bien hechas que muchas mal. El resto las harán los desarrolladores.
- **Bi-direccionales**: El coste-beneficio de hacer que una herramienta que genera código sea capaz de interpretar los cambios manuales que el desarrollador realice, es absurdo. Cuando el desarrollador está escribiendo código, éste ya es suyo.
- **Cerradas**: No es lo mismo ayudar que restringir. Si, el tiempo que el desarrollador se ahorra con tus herramientas lo pierde luego intentando saltarse las restricciones que pones para forzar que se sigan usando, el beneficio es cero. Por eso, decidimos integrar el Shell de sistema para que puedas trabajar con el command line cuando eres mas productivo de ese modo.

¿Por qué no hacer esto como una extensión del IDE?

### 3. Elimina las dependencias de terceros

Aquí podemos incluir cosas tan dispares como no obligar al equipo a usar un IDE concreto por muy adecuado que parezca ahora, o no depender de que otro equipo te proporcione un servicio. Ya hemos hablado antes del portal del desarrollador que nos quita la dependencia de otro equipo que nos cree un repositorio o una instancia de integración continua.

En el pasado, desarrollamos plugins para IDEs pero, tras esa experiencia, hemos preferido desarrollar integraciones y permitir que el desarrollador decida cuándo usa cada herramienta. El portal de desarrollo, la aplicación compañera o los CLI que ejecutan las tareas son perfectamente usables con cualquier IDE. Sí que nos permitimos integrarlos y, por ejemplo, cuando ves tus dependencias obsoletas en FAST con un click, puedes abrir el fichero de configuración en el IDE preconfigurado…

Se me ocurre que, para terminar, comente nuestro MockServer como un ejemplo de herramienta que permite desacoplarse de terceros y, además, puede ser usada como una CLI independiente o desde FAST UI.

{% asset_img MockServer1.png %}

Decidimos extender las funcionalidades básicas que muchos mockserver ya ofrecen pensando en todo lo comentado en el artículo. De modo que, preguntando a nuestros desarrolladores, identificamos los puntos más problemáticos creando una UI para poder (en caliente) ir ajustando tu MockServer para:

- Poder decidir qué llamadas son respondidas por él y cuáles van contra un servidor de desarrollo.
- Alterar las cabeceras de las respuestas en caliente.
- Poder simular malas conexiones de red
- Modificar la respuesta ad-hoc por una respuesta estática
- Incluir una respuesta dinámica para ser programada por el desarrollador (online)

{% asset_img MockServer2.png %}

Si habéis llegado hasta aquí, espero de verdad que el artículo os haya parecido interesante, y tal vez os llevéis un par de ideas para incorporar en vuestros desarrollos. Si alguno se lo está preguntando, no vendemos FAST como un producto (no era esa la intención del artículo). Actualmente, estamos en proceso de liberarlo como open source.

{% raw %}
<div class="sponsor" style="border-color: #0c4293">
  <a class="logo" href="https://www.gft.com/microsites/gft-ready-to-grow-talents-wanted/"><img src="gft.jpg"  alt="GFT"/></a>
  <div class="bio">
    <p>
      Como socio tecnológico con amplia experiencia, el compromiso de <strong>GFT</strong> es impulsar la transformación digital en el sector de los servicios financieros. Nuestro equipo de innovación global desarrolla nuevos modelos de negocio en todos los sectores, centrándose en temas como blockchain, ingeniería cloud, Inteligencia Artificial e Internet de las cosas. Junto con nuestros clientes, construimos el mundo financiero del futuro.
    </p>
    <p>
      Fundada en 1987, la compañía cuenta con un equipo global de alrededor de 5.000 empleados.
    </p>
  </div>
</div>
{% endraw %}

{% raw %}
<div class="post-author">
  <div class="bio">Por <strong>Carlos Rubio</strong>, Senior Architect en GFT. 17 años de experiencia en sistemas front-end y middleware en los sectores de manufacturas y bancario. Actualmente, responsable de arquitectura y movilidad en GFT.</div>
  <img class="photo" src="Carlos Rubio.jpeg" alt="" />
</div>
{% endraw %}
