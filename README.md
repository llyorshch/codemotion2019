# Codemotion 2019 Notes

Notes about the conference. Just the highlights. Zero fat.

## September 24 - Tuesday

### Thinking like a Founder - Chad Arimura

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

- "You don't hire a VP of innovation."
- "There is no economy of scale in software". In other words, 1000 crappy programmers don't make a good software project just because they are many whether or not they are very well organized.
- Cloud Native
  - Self service. No waiting. (No Jira tickets).
- Diversity in software is good to avoid epidemic errors. This is valid for software and for people.
- The "availability theather", that is, pretending that your application is highly available just because you have a DR that you have never tested properly. PRACTICE FAILOVER.
- "YOU CANNOT PREDICT FAILURE. FAILURE HAPPENS." Be prepared for that. The answer is "Chaos engineering".

### The Reactive Revolution - Josh Long

- [Talk source code](https://github.com/joshlong/reactive-revolution)
- [Reactive Spring Book](http://www.reactivespring.io/)
- [Reactive Streams spec](http://www.reactive-streams.org/)
- [RSocket](http://rsocket.io/)
- Reactive means disconnecting the thread that got the request from the thread that will return the response. Let the system do other things meanwhile.
- "Make jar, not war!"
- "Java 8 is morally bad"
- Let the client control the flow
- Router function to declare endpoints

### The Future of Serverless Java - Chad Arimura

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

### Artificial Stupidity - Alex Fernández

- Just a funny talk about artificial intelligence

### One Click Development Environments - Pablo Chico de Guzman

- [Okteto](https://okteto.com/) - K8s for developers
- People does not develop with docker or k8s. People uses native development and docker just for dependencies.
- Good app to demonstrate the use of k8s: [Hipster Shop: Cloud-Native Microservices Demo Application](https://github.com/GoogleCloudPlatform/microservices-demo)
- To enable Cloud Native Development:
  - Mutable pods. YES, mutable. To sync code.
  - Development images with development tools included
- [VS Code Server](https://github.com/cdr/code-server)
- Also good to develop in a remote cloud environment

### Descubriendo Quarkus, java sub-atómico en acción - Katia Aresti y Aurea Amunozhe

- [Quarkus](https://quarkus.io/) is a new thing. Not yet ready for production.
- microservices and serverless environment for Java EE people
- Includes hot reloading!
- Includes both reactive and imperative programming
- Bootstrap with an archetype
- Quarkus is based in many projects to provide functionality (REST, Vert.x, Netty, etc. )
- Direct rivals of Spring Boot. No integration foreseen.
- Demo: [Harry Potter Quarkus](https://github.com/infinispan-demos/harry-potter-quarkus)

### El futuro era esto: Reconocimiento facial sobre video en tiempo real sin servidores - Javier Ramirez

- [Amazon Rekognition](https://aws.amazon.com/es/rekognition/)
- [Amazon Kinesis Video Stream](https://aws.amazon.com/es/kinesis/video-streams/)
- Don't be evil using this technology

### Dev Tools para Kubernetes - Pablo Chico de Guzman y Micael Gallego Carrillo

- Optimizations to enable developing in a K8s environment
  - [JIB](https://github.com/GoogleContainerTools/jib) to create optimized docker images for development
  - [Okteto](https://okteto.com/) - K8s for developers
    - Hot reloading of java classes in the k8s container
  - Other tools
    - [Telepresence](https://www.telepresence.io/)
    - [KubeFwd](https://kubefwd.com/)

## September 25 - Wednesday
