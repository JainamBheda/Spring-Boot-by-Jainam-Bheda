## Spring Core 

-  So Spring framework is powerful, open source framework for building Java application.

## Core Idea behind Spring 

- Normally in JAVA , we create the object `manually` using `new` keyword.
- But in Spring, you just declare what you need, and `Spring creates and manages the object for you`
- This makes application easy to maintain..


Example:
```
public class Jainam{
	private Engine eng;
	
	// usually we do Engine eng = new Engine();
	// But in spring , we say "I need eng".
	
	@Autowired
	public Jainam(Engine eng){
		this.eng = eng;
	}
}
```

This creation and management of objects without new keyword is done by following features of Spring Boot.

1. [[Spring IoC Container]]
2. [[Dependency Injection]]
3. 