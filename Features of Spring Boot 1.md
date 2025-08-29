- Spring Boot is built over on the top of conventional Spring framework, providing all the features of Spring while being significantly easier to use.
- Below are key features of Spring Boot:
  
	1. **Auto - Configuration** : So spring boot automatically configures components based on dependencies. No need for manual XML setup.
	   
	2. **Easy Maintenance and creation of REST Endpoints :** with annotation like @RestController, @GetMapping, and @PostMapping, creating REST endpoint.
		```
		@RestController
		@RequestMapping("/api")
		public class MyController{
			@GetMapping("/hello")
			public String Jainam(){
				return "Hello my name is Jainam Bheda."
			}
		}
		```

	3. **Easy Deployment** : Because Spring Boot can be packaged as `JAR` or `WAR` files and deployed directly to the server or cloud environment.
	   
	4. **Microservice Based Architecture**
	