
What is spring?

Spring is a framework that focuses on creating enterprise applications with java
so creating an application for large scale use

using spring also helps eliminate boilerplate code (repeating code) such as using
@Autowired to use Dependency injection

Dependency injection is a design pattern used by the spring framework to help define
their dependencies, it is also a core principle of the IOC in spring mainly used
to help loose coupling

a big feature of using spring is the IOC (Inversion of Control) which helps
manage dependencies.

IOC is a design pattern that refers to the reversal of the flow of control in a system



What is Spring boot?

Spring boot is built on top of Spring framework or extension of spring

spring boot makes using the spring framework simpler as it can be used to make
stand-alone spring applications that we can just run, its also typically embedded with
Tomcat, Jetty or Undertow. its also autoconfigured when 3rd party libraries are involved

Tomcat, Jetty and Undertow are open-source java based applications servers and servlets
containers for java code that are production-ready


What is a spring bean?

a spring bean is an instance of a class managed by the spring container

the container decide when to create and delete the "beans" or instance of those classes

beans are defined by the @Component annotation, most of the annotations we will use
such as @Service @Repository @RestController/@Controller,

@Entity is not a bean and is not apart of the spring framework but is apart of the JPA
and if the class we require needs to be apart of both we can use the @Entity and @Component to
enable both on that class so the ioc container can manage this class as well


What is the spring IOC Container?

the ioc container is a core concept of the Spring framework, it's responsible for creating initializing and
managing the beans one of the main purposes of this container is to preform the Dependency injections


What does  @SpringBootApplication do?

@SpringBootApplication is an annotation that does multiple things at once, it does the jobs
of the @Configuration which tags the class as a source or bean definitions for the application
the @EnableAutoConfiguration which tells spring boot to start adding beans based on classpath settings, meaning this
allows the application to automatically detect registered beans within and activates its behavior, the last
one is @ComponentScan, which tells the application to look for other components configurations and services within
the package


What is the Dispatcher Servlet?

this handles the HttpRequests and where they go, and processes the request according to how it is to be handled
using a HandlerAdapter

What is a Logger?
a logger is an object that can be used to log messages for a specific system or application.
they can help identify if a request is preformed correctly or incorrectly
