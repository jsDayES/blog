---
title: La dificultad de ser un programador Javascript Full Stack
tags:
  - Javascript
  - JS
  - Corus
  - Full Stack
  - Developer
date: 2018-10-16 08:57:59
---

**Programar en Javascript parece sencillo a primera vista**. Sobre todo, si se tiene en cuenta su humilde origen como pequeño complemento para ofrecer algo de dinamismo a las páginas HTML. Hoy en día la realidad es bien diferente, la complejidad de las aplicaciones y gran amplitud del ecosistema Javascript hace muy complicado ser un buen programador full-stack, con experiencia y conocimientos como para afrontar los retos que se nos plantean.

{% asset_img orquesta.jpg '"One-man band" por Andrew Malone' %}
<!-- more -->
<center><small>Photo by [Andrew Malone](https://www.flickr.com/photos/andrewmalone/5163238038 "'One man band' by Andrew Malone, on Flickr")</small></center>

A modo de pequeño repaso, revisemos algunos de los elementos que deberíamos dominar para poder ser un auténtico programador full-stack:

Aunque parezca sorprendente, el primero reto que nos encontramos es el propio lenguaje, ya que podemos programar en **Javascript 5** o en **Javascript 6** (y siguientes), e incluso optar por opciones como **Typescript**, que amplían nuestras posibilidades. Es cierto que las diferencias no son enormes, pero resulta molesto acostumbrarse a uno de estos sabores y luego tener que cambiar.

Las grandes posibilidades que estos momentos ofrecen el desarrollo en cliente y en servidor con Javascript también nos plantean un debate sobre **en qué lado de nuestras aplicaciones debemos incluir cada funcionalidad**. Tanto el side server rendering que nos permite construir todo el front en el servidor, como la capacidad de desarrollar aplicaciones complejas en el lado del cliente, hace que las decisiones sobre la arquitectura de nuestra aplicación sean cada vez más importantes.

La **comunicación entre el cliente y el servidor** ya no sólo se plantea por medio de **HTTP**, y podemos utilizar **WebSocket**, que ofrece una gran versatilidad para desarrollar aplicaciones integradas y con una capacidad de comunicación bidireccional. El soporte a Websocket es prácticamente universal y podemos apoyarnos en él para desarrollar aplicaciones modernas y dinámicas.

Los formatos de comunicación entre el cliente y el servidor tenemos el omnipresente **API REST** basadas en JSON, pero no tenemos por qué limitarnos y podemos explorar **GraphQL**, o utilizar **RAML** u **OpenAPI** para las definiciones de estos API. Desde luego definir bien la comunicación entre las diferentes piezas será clave para poder abordar desarrollos complejos con capacidad de crecimiento y evolución.

En el servidor tenemos que pensar en que **modelo de servicios, o microservicios**, vamos a construir, teniendo en cuenta tanto aspectos funcionales o de dominio, como de escalabilidad, considerando las interrelaciones entre las distintas piezas, tanto ahora, como -si es posible- en el futuro.

Por supuesto podemos platearnos qué **frameworks o librerías vamos a utilizar en el servidor**. Desde un sencillo Express a un completo NextJS, las oportunidades que nos ofrecen el ecosistema de paquetes disponibles son realmente impresionantes, casi abrumadoras.

Las **bases de datos NoSQL** han optado, en general, por un modelo clave-valor muy próximo a los objetos Javascript y podemos considerarlas como un universo muy cercado y que, desde luego, tiene que conocer un buen programador full-stack.

Sobre **frameworks el en lado cliente** la cosa sigue reñida. Una vez que se ha superado la primera impresión que nos produce la inversión de control que conlleva su utilización, prácticamente nadie duda de su utilidad. Pero la decisión de cuál utilizar no es sencilla. Lo más importante es tener en cuenta que todos estos frameworks **están basados en componentes** y es fundamental comprender como funcionan, qué nivel de aislamiento plantean, cómo gestionan los datos, etc. Si esto no se tiene en cuenta, se hacen unos desarrollos monstruosos, complemente inmanejables.

Desde luego podemos utilizar **VueJS**, el frameworks que más rápidamente está creciendo y es que es muy productivo, **ReactJS** que es una solución muy potente, con una gran acogida, o **Angular**, que una vez a superado su ruptura entre la versión JS y la versión 2, sigue siendo una opción ampliamente aceptada, pero también podemos optar por otras opciones menos conocidas que se nos ofrecen en excitante ecosistema del desarrollo cliente.

Estos frameworks se complementan habitualmente con **otras librerías** y otros elementos que, en ocasiones vienen incluidos, pero en otras debemos decidir si utilizamos un determinado router o una librería Flux, etc.

Cuando uno hace una aplicación de cierta complejidad enseguida echa en falta **componentes web avanzados**: un grid, un calendario, un árbol, etc. Es importante no andar buscando sin criterio por Internet componentes, ya que normalmente terminaremos teniendo un código de muy baja calidad, heterogéneo y sin mantenimiento. Seleccionar que componentes utilizamos es también importante.

Hoy en día el Javascript cliente (y a veces también en el servidor) se compila antes de enviarlo a producción. No es una simple minificación, es un cambio de sintaxis -por ejemplo, con **BabelJS**- para asegurarse que funcionará correctamente en navegadores antiguos que no soportan Javascript 6. Aunque cada día son menos los navegadores que no ofrecen soporte a las nuevas versiones de Javascript, no es mala idea hacer esta conversión.

El proceso de transpilación y, en general, todo el proceso de desarrollo se gestiona habitualmente con un motor de transformación. El más popular en estos momentos es **Webpack** -aunque hay otros- que se encarga de gestionar los procesos de compilación, transpilación, resolución de dependencias, empaquetado, etc.

No podemos olvidarnos de las **pruebas**, tanto unitarias, como extremo a extremo. La amplitud de soluciones para las pruebas puede ser desconcertante, pero todo el esfuerzo realizado en esta área se recupera ampliamente en cuanto el desarrollo va creciendo o se van ampliando el mantenimiento de los desarrollos.

La **seguridad** no puede ser olvidad en este repaso. Tanto en las fases de diseño, como en la implementación de cada pieza, como en las pruebas o la puesta en producción la seguridad debe ser una de nuestras prioridades.

La **gestión del proceso de desarrollo**, del versionado, la automatización de pruebas, la integración continua y -si nos atrevemos- el despliegue continuo, nos ofrecen la posibilidad de acelerar nuestro trabajo sin perder el control, haciendo que nuestro trabajo se apoye en herramientas que nos facilitan el día a día.

Espero no haberte abrumado, pero es que el desarrollo Javascript es actualmente bastante complejo y requiere de una gran cantidad de herramientas, soluciones y experiencia. En [CORUS](https://www.corusconsulting.com/) abordamos todo este basto campo con un modelo de formación continua denominado NINJA. Trabajando con cada una de las piezas en proyectos reales, teniendo el tiempo y la tranquilidad necesaria para interiorizar cada uno de los conceptos, formamos programadores auténticos programadores full-stack.

En esta misma línea [CORUS](https://www.corusconsulting.com/) apoya el JSDayES. Si quieres estar al tanto de algunas de las más interesantes novedades en Javascript, no puedes perderte el JSDayES, una oportunidad única para estar al día de todas las posibilidades que se nos ofrecen en el ecosistema del desarrollo.

{% raw %}
<div class="sponsor" style="border-color: #44ae33">
  <a class="logo" href="https://www.corusconsulting.com/"><img src="corus.png" alt="Corus" /></a>
  <div class="bio">
    <strong>CORUS</strong> es una empresa innovadora, en proceso de crecimiento y expansión internacional, con la solidez de más de 15 años de experiencia dentro del sector IT.
  </div>
</div>
{% endraw %}
