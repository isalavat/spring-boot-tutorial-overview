<h1>#Spring Boot Overview</h1>
Spring Boot uses Spring MVC, Spring REST, Spring Core, Spring AOP ....
Spring Team provides free Spring Tool Suite (IDE Plugins)
<h2>Configure project at Spring initializr Website</h2> 
  Go to start.spring.io. Choose the latest stable version and create Spring boot project! Unzip and import as Maven Project in Eclipse! 
<hr>
Code: <br>
<pre>
@SpringBootApplication // Annotation for Spring Boot App. Auto config
public class MyspringbootappApplication {
	public static void main(String[] args) {
		SpringApplication.run(MyspringbootappApplication.class, args); // run the app
</pre>
<hr>
<h2>Creating a REST API Controller</h2>
Annotations:<br>
@RestController - class annotation<br>
@GetMapping - method annotation that marks the method as GET-Request Handler
<hr>
<h2>Exploring a Project Structure:</h2><br>
mvnw - allow to run Maven Project. If Maven is not installed it will automaticly download and run the maven project.<br>
mvnw.cmd - includes commant that compiles the project<br>
pom.xml - dependencies, plugins to package jar, war files and project description etc.<br>
<h3>Annotations</h3><br>
@EnableAutoConfiguration - Enables SB's auto-config support<br>
@ComponentScan - Scanning of current and sub-packages<br>
@Configuration - Able to register extra beans with @Bean or import other configuration classes <br>
@SpringBootApplication is composed of these three annotations!<br>
It is recommended always to place your main class in the main package in order to be able to scan all the sub-packages!<br>
If there are some other non sub packages than use following annotation:<br>
@SpringBootApplication(scanBasePackages={"package1", "package2" ...})<br>
resources/application.property - derfault prop file<br>
resources/static - by default for static resources<br>
For jar packaging do not use src/main/webapp directory, since it's ingnored and will be used only for war packaging <br>
template directory - for template engine FreeMarker, Thymeleaf, Mustasche<hr>
<h2>Starter files</h2>
Go to pom.xml->Dependency Hierarchy in order to explore starter files in eclipse<br>  
Spring Boot Starter Parent<br>