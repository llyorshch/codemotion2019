# Codemotion 2019 Notes

Notes about the conference. Just the highlights. Zero fat.

In this document you can find our notes.

In the file [PITCHME.md](PITCHME.md) you can find the [Marp](https://marp.app/#get-started) presentation. To preview the presentation you can execute the following command:

```bash
marp -p PITCHME.md -o dist/PITCHME.html
```

## September 24 - Tuesday

### [01 🧷] - Thinking like a Founder - Chad Arimura

#### Asistentes

- Jorge Mora - **Quiero hablar de esta presentación**
- Victor Ibañez
- ...

#### Jorge's notes

- CEO's functions:
  - People
    - Choose wisely and empower your team
  - Vision
    - Just a north star
  - Capital
    - Fear the treadmill
- Culture
  - YOU are the culture. Less words. Acts.
  - Shitty or incoherent culture brings a shitty incoherent company.

### Speeding up Innovation - Arun Gupta

#### Asistentes

- Jorge Mora
- Victor Ibañez
- Alex García

#### Jorge's notes

- "You don't hire a VP of innovation."
- "There is no economy of scale in software". In other words, 1000 crappy programmers don't make a good software project just because they are many whether or not they are very well organized.
- Cloud Native
  - Self service. No waiting. (No Jira tickets).
- Diversity in software is good to avoid epidemic errors. This is valid for software and for people.
- The "availability theather", that is, pretending that your application is highly available just because you have a DR that you have never tested properly. PRACTICE FAILOVER.
- "YOU CANNOT PREDICT FAILURE. FAILURE HAPPENS." Be prepared for that. The answer is "Chaos engineering".

### [02 🧷] - The Reactive Revolution - Josh Long ----> PENDIENTE DE QUE LE SALGA UN "PADRE". ¿Juankar?

#### Asistentes

- Jorge Mora
- Victor Ibañez
- Juan Carlos Rivera
- Alex García

#### Jorge's notes

- [Talk source code](https://github.com/joshlong/reactive-revolution)
- [Reactive Spring Book](http://www.reactivespring.io/)
- [Reactive Streams spec](http://www.reactive-streams.org/)
- [RSocket](http://rsocket.io/)
- Reactive means disconnecting the thread that got the request from the thread that will return the response. Let the system do other things meanwhile.
- "Make jar, not war!"
- "Java 8 is morally bad"
- Let the client control the flow
- Router function to declare endpoints

#### JC's notes

- Spring Reactive Web module in start.spring.io / ReactiveCrudRepository / Mono VS Flush
- [Spring Podcasts](https://spring.io/team/jlong)
- Spring initializer (dependency: Spring Reactive Web)

### [03 🧷] - Lo nuevo de CSS - Sonia Ruiz

#### Asistentes

- Alberto Chovares
- Javi Ruiz **VA a hablar de esta presentación**
- Alex García (Youtube) **Quiero hablar de esta presentación**

#### Alex's notes

- CSS History
- Can I Use
- New Properties & Samples:
  - Pie Chart -> conic-gradient (70%)
  - Media queries
    - hover /pointer:coarse (85%)
    - width >= (0%)
  - Slider -> scroll-snap (85%)
  - Pseudo-classes
    - has (parent selector - 0%)

### [04 🧷] - The Future of Serverless Java - Chad Arimura

#### Asistentes

- Jorge Mora **VA a hablar de esta presentación**
- Juan Carlos Rivera
- ...

#### Jorge's notes

- 80% of the world is using Java
- But Java is not popular in serverless environments
- And the trend is quite bad
- Java optimizations for serverless applications
  - Class Data Sharing (JVM Enhancement)
  - [Project Portola](https://openjdk.java.net/projects/portola/), a port of the JDK to the Alpine Linux distribution.
  - [SubstrateVM](https://github.com/oracle/graal/tree/master/substratevm), a framework that allows ahead-of-time (AOT) compilation of Java applications.
  - [jlink](https://docs.oracle.com/javase/9/tools/jlink.htm), a tool to create reduced JDKs
  - JDK 10+ provides better integration with containers (recognizes cgroup limits)
  - Language improvments
    - Less ceremony
      - var
      - Text blocks with """
      - switch expressions
  - Simplified native code access with [Project Panama](https://openjdk.java.net/projects/panama/)

#### JC's notes

- Java 11
  - Introduction of var reduces BoilerPlate
  - New switch expressions
  - Improvements lambda
  - Text Blocks (""")

### [05 🧷] - Interfaces en tiempo real con Angular y Redux - Antonio Pérez y Manuel Maldonado @apcano1978 (Digital 55)

#### Asistentes

- Alex García **VA a hablar de esta presentación**
- Alberto Chovares
- Javi Ruiz?

#### Alex's notes

- Angular application with Redux pattern, using NgRX
- Advantages of using redux:
  - reduce number of components
  - events between components
  - multiple datasources
  - real-time events
  - problems arising from asynchrony
- Redux concepts: store, actions & reducers
- Sample use case: CRUD with websocket inconming events

### Artificial Stupidity - Alex Fernández

#### Asistentes

- Jorge Mora
- ...

#### Jorge's notes

- Just a funny talk about artificial intelligence

### Kotlin Multiplatform - David González (Mixtiles)

#### Asistentes

- Alex García

### Alex's notes

- Kotlin multiplatform as common libraries in a project with iOS & Android native apps.
- Easier for Android. Plugins needed for building from XCode
- Cannot debug on iOS (extra plugins for logging)
- Conclusion:
  - good solution for a product with native apps
  - still unstable

### Google Assistant's Smart Home API in practice

#### Asistentes

- Victor Ibañez
- ...

### [06 🧷] - One Click Development Environments - Pablo Chico de Guzman

#### Asistentes

- Jorge Mora
- Victor Ibañez
- Juan Carlos Rivera **Quiero hablar de esta presentación** Jorge: Juan carlos, ¿Presentas tú esta?
- Alex García

#### Jorge's notes

- [Okteto](https://okteto.com/) - K8s for developers
- People does not develop with docker or k8s. People uses native development and docker just for dependencies.
- Good app to demonstrate the use of k8s: [Hipster Shop: Cloud-Native Microservices Demo Application](https://github.com/GoogleCloudPlatform/microservices-demo)
- To enable Cloud Native Development:
  - Mutable pods. YES, mutable. To sync code.
  - Development images with development tools included
- [VS Code Server](https://github.com/cdr/code-server)
- Also good to develop in a remote cloud environment

#### JC's notes

- PaaS for a development environment in Kubernetes [Okteto](https//cloud.okteto.com)
- How can a development environment be classified?
  - Replicable: All developers will have the same experiencie
  - Integrated: As much similar to production as possible.
  - Efficient: Fast to install and work with
- Vagrant: Allow us to create and configure lightweight, reproducible, and portable development environments.
- Types of environments:
  - Local: Fast but not replicable
  - Vagrant: Slow
  - Docker: Slow
  - Kubernetes: Slow
  - Cloud Native development - Really fast, the bad part is that you dont have your IDE with your extensions to keep working on it
  - New plugin VS Code Remote SSH - You can create a SSH connection to a remote machine (development) and you can debug using your IDE.
  - It provides you the possibility to develop directly inside a pod of kubernetes or a container it avoids the creation of the container when the development changes.

### [07 🧷] - Descubriendo Quarkus, java sub-atómico en acción - Katia Aresti y Aurea Amunozhe

#### Asistentes

- Jorge Mora
- Victor Ibañez **VA a hablar de esta presentación**
- Juan Carlos Rivera
- Alex García

#### Jorge's notes

- [Quarkus](https://quarkus.io/) is a new thing. Not yet ready for production.
- microservices and serverless environment for Java EE people
- Includes hot reloading!
- Includes both reactive and imperative programming
- Bootstrap with an archetype
- Quarkus is based in many projects to provide functionality (REST, Vert.x, Netty, etc. )
- Direct rivals of Spring Boot. No integration foreseen.
- Demo: [Harry Potter Quarkus](https://github.com/infinispan-demos/harry-potter-quarkus)

#### JC's notes

- Quarkus: Red Hat initiative, it allows you to create app java that can run in cloud native. Hot reloading (supersonic Java)
- Deployment in a declarative way
- GraalVM: It does not provide dynamic classloading and reflection

### [08 🧷] - How to build Javascript-powered Smartglasses (without any soldering knowledge) - Ruben van der Leun

#### Asistentes

- Alex García **VA a hablar de esta presentación**

#### Alex's notes

- He wanted to create his own low-cost smart-glasses after using Vuzix (based on Google-Glass)
- Use of Vufine connected to a Powerbank and a Raspberry Pi
- Rubeye - platform meant for wearables -
- Mobile app synchronized with glasses:
  - Character recognition
  - Youtube
  - Google Maps
- Conclusions
  - Too expensive (unfeasible production)
  - Lot of time invested
  - Useful for prototypes

### [09 🧷] - El futuro era esto: Reconocimiento facial sobre video en tiempo real sin servidores - Javier Ramirez

#### Asistentes

- Jorge Mora
- Victor Ibañez **VA a hablar de esta presentación**
- Juan Carlos Rivera
- ...

#### Jorge's notes

- [Amazon Rekognition](https://aws.amazon.com/es/rekognition/)
- [Amazon Kinesis Video Stream](https://aws.amazon.com/es/kinesis/video-streams/)
- Don't be evil using this technology
- AWS Lambda: You can provide Amazon your code and when an event is triggered, that code will be executed in Amazon and will provide you the result. You pay by millisecond that the code is running. You dont care about the server.

Me das tu código y cuando pase un evento, lo ejecutas. PAgas por milisegundo que hay en ejecución. No te importa nada del servidor.

### Dev Tools para Kubernetes - Pablo Chico de Guzman y Micael Gallego Carrillo

#### Asistentes

- Jorge Mora
- Victor Ibañez
- Juan Carlos Rivera
- ...

#### Jorge's notes

- Optimizations to enable developing in a K8s environment
  - [JIB](https://github.com/GoogleContainerTools/jib) to create optimized docker images for development
  - [Okteto](https://okteto.com/) - K8s for developers
    - Hot reloading of java classes in the k8s container
  - Other tools
    - [Telepresence](https://www.telepresence.io/)
    - [KubeFwd](https://kubefwd.com/)

#### JC's notes

- Kubernetes native application
- Layer's optimization. It splits code of libraries by layers. That way you send less information
- Jib -> Google container Tools (jib-maven-plugin)
- Jib allows you to build and upload that image by layers as easy as 'compile jib:build'

### [10 🧷] - Tips para mejorar la gestión de tu tiempo - Adolfo Sanz De Diego

#### Asistentes

- Javier del Aguila **VA a hablar de esta presentación**
- Juan Carlos Rivera

#### JC's notes

- Videos gestión del tiempo

  - Gettings Things Done (GT) | David Allen
  - The 7 habits of highly effective people | Stephen Covey

- Charlas TED
  - How to gain control of your free Time | Laura Vanderkam
  - How to stop screweing yourself over
  - La regla de los 5 segundos para no procrastinar
  - What makes a good life?
- Tips varios:
  - Sé proactivo y haz primero lo primero
  - Concepto "The Pareto Principle" -> Do more by Doing Less
    80 / 20 rule -> El 80% de las consecuencias provienen del 20% de las causas
    https://es.wikipedia.org/wiki/Principio_de_Pareto
- Herramientas
  - Calendario, Lista de tareas, Otras listas, Alarmas, Reglas de correo...

### GITTogether: Front(end) to the backend - Beatriz De Miguel Pérez

#### Asistentes

- Alex García
- Alberto Chovares
- Javi Ruiz

#### Alex's notes

- Javascript backend with NodeJS
- MVC Architecture layers
- Express Frontend app
- MongoDB
- For beginners

## September 25 - Wednesday

### [11 🧷] - Taking Back “Software Engineering” by Dave Farley

#### Asistentes

- Jorge Mora **VA a hablar de esta presentación**
- Victor Ibañez
- ...

#### Jorge's notes

- "UML is only a tool. It's not engineering"
- Solid disciplines are made with solid principles
- SCRUM is project management stuff. It's not SE. There is no word about coding in the SCRUM spec.
- Craftsmanship
  - Production is not a problem (we simply copy bytes to deliver a product). The problem is design.
- Software industry
  - Craft <-- We are here
  - Mass production <-- WRONG
  - Lean production techniques <-- We WANT to be here (but we are not here yet)
- We are always building the fist bridge, the first rocket, etc.
- The scale of what we build varies a lot (hut vs. skyscraper)
- Dave's definition of engineering
  - **Engineering** is the application of an empirical, scientific approach to finding efficient solutions to practical problems.
- Fundamentals of the engineering approach:
  - Iterative
  - Employs feedback
  - Incremental
  - Experimental
  - Empirical
- Iterative vs. Incremental  
  ![Iterative vs. Incremental](images/incrementalVsIterative.png)
- The most expensive user story: "As the President of the U.S.A. I want to send a man to the moon before the end of this decade". JFK 1961.
- If you have a BIG challenge, you have to be experimental. Waterfall was not an option to send a man to the moon.
- The first engineer. 🙇🏻‍  
  ![Margaret Hamilton](images/margaret_hamilton.jpg)
- Experimentation and learning: The Ranger Programme (to "hit" the moon)  
  ![The Ranger Programme](images/Dave_Farley_Being_Experimental.jpg)
- Just guessing is not good enough. You have to measure it!
- Be empirical
- Continuous delivery as an engineering principle
- Don't be _like_ engineers. **Be** engineers.

### [12 🧷] - Are Web Components the Betamax of Web Development? - Horacio Gonzalez (OVH) @LostInBrittany

#### Asistentes

- Alex García **VA a hablar de esta presentación**
- Alberto Chovares
- Javi Ruiz

#### Alex's notes

- Betamax history
- Comparison between Vue, Angular and Vue
- Ionic 4 / Stencil or Polymer as a solution nowadays
- Webcomponent are based in the low level html standard

### Building Reactive Pipelines: How to go from scalable apps to (ridiculously) scalable systems - Mark Heckler

#### Asistentes

- Jorge Mora
- Victor Ibañez
- Juan Carlos Rivera  **¿Juan Carlos, quieres hablar tú de esta?**
- ...

#### Jorge's notes

- Definition of reactive programming  
  ![Definition of reactive programming](images/MarkHeckler_Reactive_programming_definition.jpg)
- [Spring Cloud Stream](https://spring.io/projects/spring-cloud-stream)
- Connecting two processors with configuration 😮
  ![Connecting two processors with configuration](images/MarkHeckler_connecting_Processors.jpg)
- Resources  
  ![Resources](images/MarkHeckler_Resources.jpg)

#### JC's notes

- Mark Heckler twitter: @mkheck
- Important blogs posts:
  - https://thehecklers.com/ - Spanish springs news (https://springnoticias.io/)
- Reactive Programming: Keys are source, processor and sink
- Reactive streams (publisher, subscriber, subscription and processor --> Spring: Source, processor and sink)
- Dependency in spring initializer (start.spring.io) is Reactive cloud stream
- You can define in which microservice the binding is: spring.cloud.stream.bindings.output.destination=source
- You can define the functions name: spring.cloud.stream.bindings.function.definition=checkIn
- Decide the class using annotations: @EnableBinding(Source.class)
- Decide the processor using annotations: @EnableBinding(Processor.class)
- lombok - @Value (setters and getters implicit) @AllArgsConstructor
- Flux<Model>
- [Example](https://github.com/mkheck/building-reactive-pipelines)

### Midiendo la calidad de código en WTF/min (con ejemplos de código real que... - David Gómez

#### Asistentes

- Jorge Mora
- Juan Carlos Rivera
- ...

#### Jorge's notes

- Funny talk about crappy code. 😂
- Highly inspired by Clean Code by Uncle Bob

#### JC's notes

- Clean code
- What about building a hall of fame of WTF of bad code that will be published when they are fixed.
- Code must be written by a developer, not by a computer
- Devs spend most of time reading code and not writing it.
- Tips:
  - Be careful with comments, we need to describe why it does it and not what it does
  - Review javadoc of spring framework, is really good
  - Exceptions: Catch only if you know what to do with them, not just throwing them again.
  - Remove unnecessary code

### Visualización de Datos Interactiva en aplicaciones con Vue.js y React - Javier Abadía (StyleSage) @javierabadia

#### Asistentes

- Alex García
- Alberto Chovares
- Javi Ruiz?

#### Alex's notes

- Charts with only D3JS, only Vue, or only React. Combined charts using D3 & Vue & React
- Animation with Vue or React, needs external libraries
- Hover events
- Responsive charts

### [13 🧷] - ¡GraalVM y Micronaut: compañeros perfectos! - Iván López (el humilde)

#### Asistentes

- Jorge Mora
- Victor Ibañez **VA a hablar de esta presentación**
- Juan Carlos Rivera
- ...

#### Jorge's notes

- Micronaut was designed to take advantage of AOT instead of reflection and other non-friendly GraalVM techniques.

#### JC's notes

- GraalVM: Oracle's virtual machine undertands several language (java, scala, groovy, y a parte ruby, python, js, r)
- Micronaut:
  - Framework for microservices in JVM
  - Is AoT (Ahead of compilation): At runtime, it generates metadata classes so it does not have to keep them in memory, it does not matter if the app is really big.
  - It provides Cloud Native
  - Micronaut Data (toolkit for data access, similar to spring data)
  - Compilation Time really really high but the time to boost ys really low.

### Web Scrapping como nunca te lo contaron. Atajos y técnicas de Evasión de contramedidas - Jorge Barrachina (ESRI) @NTKOG

#### Asistentes

- Alex García
- Alberto Chovares
- Javi Ruiz

#### Alex's notes

- Legal notes to know what's legal to be scrapped
- Real use cases of unlegal scrapped data
- Bots
- Scrapping tools
  - Parallel
  - Puppeteer
- Conclusion: theorical and moral talk

### Operational Serverless - Vicenç García Altés

#### Asistentes

- Jorge Mora
- ...

#### Jorge's notes

![Trap](images/trap.gif)

### Afrontando el mal software - César Alberca (Autentia) @cesalberca

#### Asistentes

- Alex García
- Alberto Chovares
- Javi Ruiz

#### Alex's notes

- SOLID principle
- Design patterns: commans, decoratos, chain of responsability
- Talk for beginners

### [14 🧷] - React hooks, bye bye to classes - ~~Victor Ibáñez Aparicio~~ Carlos P. Jimeno

#### Asistentes

- Jorge Mora
- Alex García **VA a hablar de esta presentación**

#### Jorge's notes

- Super cool talk to get to know React Hooks in 40 min. 👏🏻
- [Slides](https://slides.com/carlosperezjimeno/reacthooks#/)

### Alex' notes

- Hooks:
  - useState (Toggle)
  - useEffect (Scroll)
  - useContext (Theme)
- Powerful useReducer + useContext combination
- Custom hooks:
  - useChecked
  - useArray

## Cloud-native monitoring with Prometheus

#### Asistentes

- Victor Ibañez
- ...

### [15 🧷] - Perfectionism, Impostor Syndrome and Anxiety - Understanding your fears and learning to be kind to yourself - Jo Franchetti

#### Asistentes

- Javier del Aguila **VA a hablar de esta presentación**

## Wrap-up

#### Jorge's notes

- Unbalanced talks. Some of them very good with international speakers, some very poor. Luckily, the poor ones were the few.
- Overall, a very well organized conference. Watching the conferences in a cinema was great.
- Most popular technologies:
  - K8
  - Serverless
  - Reactive programming
  - ML
