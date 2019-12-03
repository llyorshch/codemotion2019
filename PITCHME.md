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

- Lorem ipsum dolor sit amet, consectetur adipiscing elit.
- Mauris suscipit luctus volutpat.
- Maecenas at lacus nec velit bibendum ullamcorper.
- Lorem ipsum dolor sit amet, consectetur adipiscing elit.
- Mauris suscipit luctus volutpat.
- Maecenas at lacus nec velit bibendum ullamcorper.

---

#### Taking Back “Software Engineering” - Dave Farley

- Lorem ipsum dolor sit amet, consectetur adipiscing elit.
- Mauris suscipit luctus volutpat.
- Maecenas at lacus nec velit bibendum ullamcorper.

---

#### The Future of Serverless Java - Chad Arimura

- Lorem ipsum dolor sit amet, consectetur adipiscing elit.
- Mauris suscipit luctus volutpat.
- Maecenas at lacus nec velit bibendum ullamcorper.

---

<!-- Victor -->

#### ¡GraalVM y Micronaut: compañeros perfectos! - Iván López (El simpático)

- GraalVM: VM políglota de Oracle
- Sin reflexión ni runtime proxies
  ![width:900](images/graalvm_architecture.png)

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

#### Lo nuevo de CSS - Sonia Ruiz

- Lorem ipsum dolor sit amet, consectetur adipiscing elit.
- Mauris suscipit luctus volutpat.
- Maecenas at lacus nec velit bibendum ullamcorper.

---

<!-- Alex -->

#### Interfaces en tiempo real con Angular y Redux - Antonio Pérez y Manuel Maldonado

- Típicos problemas en aplicaciones frontend
- Patrón Flux:
  - Store como única fuente de verdad
  - Acciones como reglas para cambiar el estado del Store
- Valoración del uso de Redux en un proyecto
- Ejemplo práctico del uso en Angular con NgRx con múltiples fuentes de datos
  - Módulos
  - Estructura recomendada
  - Acciones -> Efectos -> Acciones

---

#### How to build Javascript-powered Smartglasses (without any soldering knowledge) - Ruben van der Leun

- Lorem ipsum dolor sit amet, consectetur adipiscing elit.
- Mauris suscipit luctus volutpat.
- Maecenas at lacus nec velit bibendum ullamcorper.

---

#### Are Web Components the Betamax of Web Development? - Horacio Gonzalez

- Lorem ipsum dolor sit amet, consectetur adipiscing elit.
- Mauris suscipit luctus volutpat.
- Maecenas at lacus nec velit bibendum ullamcorper.

---

#### React hooks, bye bye to classes - Carlos P. Jimeno

- Lorem ipsum dolor sit amet, consectetur adipiscing elit.
- Mauris suscipit luctus volutpat.
- Maecenas at lacus nec velit bibendum ullamcorper.

---

<!-- Juan Carlos -->

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

| | Replicable | Integrado | Rápido
| --- |  --- | --- | --- |
**Local**| NO | NO | SÍ |
**Vagrant**| SÍ | SÍ | NO |
**Docker**| SÍ | SÍ | NO |

---
#### One Click Development Environments - Pablo Chico de Guzman

- Cloud Native Development: pod mutables, cambio de imagen local en el pod
    - Sincronización código desde el propio editor en local hasta el pod

    
| | Replicable | Integrado | Rápido
| --- |  --- | --- | --- |
**Cloud Native**| SÍ | SÍ | SÍ |

- Visual Studio Code Remote development
---
<!-- Javier del Águila -->

#### Tips para mejorar la gestión de tu tiempo  

**Adolfo Sanz De Diego**

- Creador de una comunidad, organizador de hackathones, profesor de universidad, imparte cursos de tecnología, asesor técnico y padre de dos hijas
---
#### Planificar
- Lista Tareas: Cortas, concretas y agendables
- **Agendar** y poner alarmas

| | Urgente | No Urgente |
| --- |  --- | --- |
**Importante**| Hazlo! | Agéndalo | 
**No Importante**| Delega | Olvida |

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
- Pánico a justificar en el daily tu trabajo diario  -> sobreesfuerzo
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
*"We learn most when reality does NOT match our predictions"*

**Dave Farley**

---
#### Wrap-up

- PLEASE, APORTAD AQUÍ VUESTRAS CONCLUSIONES

---

# <!--fit--> :+1:
