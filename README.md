<h1>#Spring Boot Overview</h1>
Spring Boot uses Spring MVC, Spring REST, Spring Core, Spring AOP ....
Spring Team provides free Spring Tool Suite (IDE Plugins)
<h2>Configure project at Spring initializr Website</h2> 
  Go to start.spring.io. Choose the latest stable version and create Spring boot project! Unzip and import as Maven Project in Eclipse! 
<hr>
Code: <br>
@SpringBootApplication // Annotation for Spring Boot App
public class MyspringbootappApplication {

	public static void main(String[] args) {
		SpringApplication.run(MyspringbootappApplication.class, args); // run the app
<h2>Creating a REST API Controller</h2>
