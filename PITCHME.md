---
marp: true
theme: uncover
---

<!--  Reglas generales -->

# Codemotion 2019

#### Mimacom|Flowable expedition selected notes & things we learned

---

<!-- Jorge -->

#### Thinking like a Founder - Chad Arimura

* CEO's functions:
  * **People** 🧍🏻 Choose wisely and empower your team
  * **Vision** 👁 Just a north star
  * **Capital** 🏃‍♀️ Fear the treadmill
* Culture
  * YOU are the culture. Less words. Acts.
  * **Shitty or incoherent culture brings a shitty incoherent company.** ⬅️ FUCKIN'AMEN

---

#### Taking Back “Software Engineering”

###### By Dave Farley

* "UML is only a tool. It's not engineering"
* Solid disciplines are made with solid principles
* **SCRUM is project management stuff. It's not SE. There is no word about coding in the SCRUM spec.**
* Craftsmanship: Production is not a problem (we simply copy bytes to deliver a product). The problem is design.

---

#### Taking Back “Software Engineering”

* Software industry
  * Craft ⬅️ We are here
  * Mass production ⬅️ WRONG
  * Lean production techniques ⬅️ We WANT to be here (but we are not here yet)

---

#### Taking Back “Software Engineering”

* The most expensive user story: "As the President of the U.S.A. I want to send a man to the moon before the end of this decade". JFK 1961
* Be experimental. Waterfall is not an option for big challenges: The Ranger Programme (to "hit" the moon)  
* Just guessing is not good enough. You have to measure it! Be empirical

---

#### The first engineer 🙇🏻‍

![Margaret Hamilton](images/margaret_hamilton.jpg)

Margaret Hamilton

---

# <!--fit--> Don't be _like_ engineers. **Be** engineers

---

#### The Future of Serverless Java - Chad Arimura

* 80% of the world is using Java, but Java is not popular in serverless environments and the trend is quite bad
* Java optimizations for serverless applications
  * Class Data Sharing (JVM Enhancement)
  * [Project Portola](https://openjdk.java.net/projects/portola/), a port of the JDK to the Alpine Linux distribution.
  * [SubstrateVM](https://github.com/oracle/graal/tree/master/substratevm), a framework that allows ahead-of-time (AOT) compilation of Java applications.
  * [jlink](https://docs.oracle.com/javase/9/tools/jlink.htm), a tool to create reduced JDKs

---

#### The Future of Serverless Java - Chad Arimura

  * Language improvements
    * Less ceremony
      - var
      - Text blocks with """
      - Switch expressions
  * JDK 10+ provides better integration with containers (recognizes cgroup limits)
  * Simplified native code access with [Project Panama](https://openjdk.java.net/projects/panama/)

---

<!-- Victor -->
![bg Cambio](images/cambio1.jpg)

---

#### ¡GraalVM y Micronaut: compañeros perfectos! - Iván López (El simpático)

- GraalVM: VM políglota de Oracle
- Sin reflexión ni runtime proxies
  ![width:600](images/graalvm_architecture.png)

---

#### Descubriendo Quarkus, java sub-atómico en acción - Katia Aresti y Aurea Amunozhe

- Quakus 1.0.0 Final --> 25 de Noviembre 2019
- Container First
- Standards-based (RESTEasy and JAX-RS, Hibernate ORM and JPA, Netty, Eclipse Vert.x, Eclipse MicroProfile, Apache Camel, Spring, etc)
- Microservice First: Fast startup time and code turn around to Java apps

---

#### Descubriendo Quarkus, java sub-atómico en acción - Katia Aresti y Aurea Amunozhe

![width:800px](images/quarkus_rest_crud_size.png)
![width:900px](images/quarkus_rest_crud_time.png)

---

#### El futuro era esto: Reconocimiento facial sobre video en tiempo real sin servidores - Javier Ramirez

- AWS Rekognition
- Análisis de imágenes, videos y reconocimiento facial<br/>
  ![width:1000px](images/aws_architecture.png)

---

<!-- Javi Ruiz -->
![bg Cambio](images/cambio2.jpg)

---
## Lo nuevo de CSS (Sonia Ruiz)

---

#### Presente

<style scoped>table { font-size: 15px;  width: 100%}</style>

|                                                                                                                                       |                                              |
| :------------------------------------------------------------------------------------------------------------------------------------ | :------------------------------------------- |
| **Custom Properties**                                                                                                                 |                                              |
| Variables en css                                                                                                                      | ![h:150](images/jruiz/custom-properties.jpg) |
| **Calc**                                                                                                                              |                                              |
| Calculo entre distintas tipos de medidas.<br/> En un futuro se agregarán:<br/> max(), min(), clamp() <br/>y funciones trigonométricas | ![h:150](images/jruiz/calc.png)              |
| **Conic Gradients**                                                                                                                   |                                              |
| Hacer un pie chart solo con css<br/>70% de compatibilidad en navegadores                                                              | ![h:200](images/jruiz/conic.png)             |

---

#### Futuro

<style scoped>table { font-size: 15px; width: 100%}</style>

|                                                                                                      |                                     |
| :--------------------------------------------------------------------------------------------------- | :---------------------------------- |
| **Custom Selectors**                                                                                 |                                     |
| Damos formato a todos los parrafos hijos<br/> de encabezados del 1 al 6                              | ![h:50](images/jruiz/selectors.png) |
| **Scroll Snap**                                                                                      |                                     |
| Sliders con css, para pc o movil                                                                     | ![h:150](images/jruiz/slider.png)   |
| **Pseudo Clases**                                                                                    | Selectores según tipos y estado     |
| **Has**                                                                                              |                                     |
| Seleccionamos todos los elementos enlace<br/> que tengan como hijo directo una imágen                | ![h:30](images/jruiz/has.png)       |
| **Is**                                                                                               |                                     |
| Seleccionamos todos los parrafos que tenga<br/> como padre un elemento de clase header, main, footer | ![h:30](images/jruiz/is.png)        |
| **Not**                                                                                              |                                     |
| Seleccionamos todos los elementos li que no<br/> tengan la clase moreinfo                            | ![h:30](images/jruiz/li.png)        |

---

<style scoped>table { font-size: 15px; width: 100%}</style>

|                                                                                                                                             |                                    |
| :------------------------------------------------------------------------------------------------------------------------------------------ | :--------------------------------- |
| **Sticky**                                                                                                                                  |                                    |
| Fijar un elemento en pantalla, hasta que<br/> aparezca otro con posicionamiento sticky.<br/> Tambien sirve para la fila header de una tabla | ![h:300](images/jruiz/sticky.png)  |
| **Fuentes variables**                                                                                                                       |                                    |
| Con un único archivo de fuente, tenemos los textos con apariencias de fuente distintos                                                      | ![h:300](images/jruiz/fuentes.png) |

---

###### Todas estas propiedades son muy chulas, pero todavía no están 100% soportadas por todos los navegadores.

###### Os aconsejo consultarlas antes de usarlas en:

###### <https://caniuse.com/#home>

<style scoped>table { font-size: 20px; width: 100%}</style>

|                                                                  |                                     |
| :--------------------------------------------------------------- | :---------------------------------- |
| **Feature Queries**                                              |                                     |
| Para aplicar estilos según sean o no soportados por el navegador | ![h:200](images/jruiz/features.png) |

---

###### Para conocer que más cosas tendremos a futuro visitad:

<http://cssdb.org>

---

<!-- Alex -->
![bg contain](images/cambio3.jpg)

---

#### Interfaces en tiempo real con Angular y Redux - Antonio Pérez y Manuel Maldonado

- Típicos problemas en aplicaciones frontend
- Patrón Flux:
  - Store como única fuente de verdad
  - Acciones como reglas para cambiar el estado del Store
- Valoración del uso de Redux en un proyecto

---

#### Interfaces en tiempo real con Angular y Redux - Antonio Pérez y Manuel Maldonado

- Ejemplo práctico del uso en Angular con NgRx con múltiples fuentes de datos
  - Módulos
  - Estructura recomendada
  - Acciones -> Efectos -> Acciones

---

#### How to build Javascript-powered Smartglasses - Ruben van der Leun

- Smartglasses / Vuzix prototype
- Motivación
- 3 elementos hardware:
  - Vufine
  - Raspberri Pi
  - Powerbank

---

#### How to build Javascript-powered Smartglasses - Ruben van der Leun

- Software: Rubeye platform connected with a Webapp
- Demo: navegador, cámara, Youtube, GoogleMaps, Face-Recognition
- Conclusiones
- Nuevos retos

---

#### Are Web Components the Betamax of Web Development? - Horacio Gonzalez

- Concepto de Componente Web (W3C)
  - Elementos customizados
  - Shadow DOM
  - Plantilla
- Historia Betamax

---

#### Are Web Components the Betamax of Web Development? - Horacio Gonzalez

- Componentes Web compatibles con todos los navegadores
- Ionic
  - AngularJS -> Angular
  - Stencil
- Polymer, deprecated?
- Los componentes web valen la pensa, son el estándar

---

#### React hooks, bye bye to classes - Carlos P. Jimeno

- Hooks:
  - useState (Toggle)
  - useEffect (Scroll)
  - useContext (Theme)
- Powerful useReducer + useContext combination
- Custom hooks:
  - useChecked
  - useArray

---

#### React hooks, bye bye to classes - ~~Carlos P. Jimeno~~ Victor Ibáñez

![width:300px](images/React_hooks_bye_bye_classes.jpg)

---

<!-- Juan Carlos -->
![bg Cambio](images/cambio4.jpg)

---


#### Building Reactive Pipelines - Mark Heckler

- Procesamiento de datos asíncrono, no bloqueante y orientado a eventos
- Reactive Stream API
- Reactive Cloud Stream (requiere una cola de mensajería: Kafka, RabbitMQ)
- Publisher<T>, Processor<T,R>, Subscriber<T>, Subscription.
- Mono vs Flux

---

#### Building Reactive Pipelines - Mark Heckler

- Publisher @EnableBinding(Source.class)
- Processor @EnableBinding(Processor.class)
- Subscriber @EnableBinding(Sink.class)

---

#### One Click Development Environments - Pablo Chico de Guzman

- Entorno de desarrollo: replicable, integrado, rápido

|             | Replicable | Integrado | Rápido |
| ----------- | ---------- | --------- | ------ |
| **Local**   | NO         | NO        | SÍ     |
| **Vagrant** | SÍ         | SÍ        | NO     |
| **Docker**  | SÍ         | SÍ        | NO     |

---

#### One Click Development Environments - Pablo Chico de Guzman

- Cloud Native Development: pod mutables, cambio de imagen local en el pod
  - Sincronización código desde el propio editor en local hasta el pod

|                  | Replicable | Integrado | Rápido |
| ---------------- | ---------- | --------- | ------ |
| **Cloud Native** | SÍ         | SÍ        | SÍ     |

- Visual Studio Code Remote development

---

<!-- Javier del Águila -->
![bg Cambio](images/cambio5.jpg)

---

#### Tips para mejorar la gestión de tu tiempo

**Adolfo Sanz De Diego**

- Creador de una comunidad, organizador de hackathones, profesor de universidad, imparte cursos de tecnología, asesor técnico y padre de dos hijas

---

#### Planificar

- Lista Tareas: Cortas, concretas y agendables
- **Agendar** y poner alarmas

|                   | Urgente | No Urgente |
| ----------------- | ------- | ---------- |
| **Importante**    | Hazlo!  | Agéndalo   |
| **No Importante** | Delega  | Olvida     |

---

#### Consejos

- Si <2 min hazlo
- Aprende a decir que no (O posponer)
- Conoce tus herramientas
- Orden
- Automatizar: scripts, filtros de email, etc..

---

#### Distracciones

- Darse de baja de listas de correo
- Redes sociales cerradas
- Cerrar pestañas que no utilicemos
- Primero lo primero/importante
- Regla de los 5 segundos

---

#### Interrupciones

- Modo no molestar en móvil y pc
- Correo 2/3 veces al día
- Una cosa a la vez
- Mejor una llamada que un mail
- Cascos
- Reuniones <1h con agenda clara

---

#### Perfectionism, Impostor Syndrome and Anxiety - Understanding your fears and learning to be kind to yourself

**Jo Franchetti**

---

#### Sindrome del impostor

- Sensación de que los demás son mejores que tú
- Miedo a pedir ayuda por parecer ignorante
- Pánico a justificar en el daily tu trabajo diario -> sobreesfuerzo
- Sensación de que no mereces estar donde estás y de que van a descubrir que eres un fraude
- Miedo a colaborar en un proyecto opensource por no estar al nivel

---

#### Perfeccionismo

- Autoexigirse un nivel inalcanzable
- Preocupación por lo que piensen los demás
- "Bastante bien" no es suficiente
- Miedo a entregar un trabajo porque alguien pueda encontrar un error
- Dejar cosas inacabadas por no conseguir exáctamente lo que se pretendía en un principio
- Pedir ayuda es no ser perfecto

---

#### Consejos

- "Perfecto" es un enemigo de "muy bien"
- Pedir ayuda te hace mejorar y ahorrar tiempo
- Nadie te va a criticar más que tú mismo
- Si alguien encuentra un error, es una oportunidad para aprender
- Hablar de tus problemas y ayudar a los demás

---

_"We learn most when reality does NOT match our predictions"_

**Dave Farley**

---

#### Wrap-up

* El nivel de las charlas fue muy variable.
* La organización, excelente.
* Vale la pena para:

  1) Mantenerse al corriente, enterarse de en qué dirección van las cosas, etc.
  2) Hacer equipo y ¡pasarlo bien!

---

Tenéis toda la información y las slides de esta charla en el siguiente repositorio:

https://gitlab.edorasware.com/solutionsES/codemotion2019

---
# <!--fit--> 🍕 ¡Gracias!
