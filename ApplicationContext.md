- This is extenstion of BeanFactory with more enterprise features like event propogation and internationalization.
  
  
- Application Context features -> provides entrpeise specfic features also 
	 1. Publishing events to registered listners by resolving property files.
	 2. methods of accessing application components.
	 3. Support internationalization.
	 4. Loading file resources in generic manner.

- ApplicationContext Implementation Classes 
	- There are different types of application containers provided by Spring for different requirements.
	- Containers are as follows 
	  
		1. AnnotationConfigApplicationContext Container.
		2. AnnotationConfigWebApplicationContext
		3. XmlWebApplicationContext
		4. FileSystemXmlApplicationContext
		5. ClassPathXmlApplicationContext.
		   
	1. Container 1 : `AnnotationConfigApplicationContext`
		- This class was introduced in Spring 3.0
		- It accepts class annotated with `@Configuration`, `@Component` and `JSR - 330` complaint classes.
		- The constructir of this container accepts `one or more classes`.
		- Example :
	```
	ApplicationContext context = new AnnotationConfigApplicationContext(Appconfig1 , Appconfig2);
	```
`AppConfig1 and AppConfig2 have the same bean declaration.`

2. Container : `AnnotationConfigWebApplicationContext


