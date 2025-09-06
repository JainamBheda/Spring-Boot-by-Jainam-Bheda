## Bean Factory

- Spring is `Container` and behaves as `factory of Beans.`
  
- Bean factory is simple container providing advanced configuration mechanism to instantiate, configure and manage the life cycle.
  
- Beans are `JAVA objects` that are configured at `run time` by IoC container.

So Bean factory provide Dependencies injection
Bean factory creates bean only when you request it. (`Lazy Loading`).

![[BeanFactory.canvas|BeanFactory]]

So imaging the above diagram like 
a container containing too many beans 

means Bean Factory (Spring IoC container) containing too many beans(Objects).

![[Pasted image 20250829220026.png]]

The Program flow is something like this 
	1. Bean factory reads XML configuration file and as per the specification 
1. Then the student reference ask for the student object from the object factory.

Step - By step implementation to configure Bean factory in Spring 

Step1 : Create Student Class (POJO)
```
public class Student{
	private String name;
	private int age;
	public Student(){}
	public Student(String name,int age){
		this.name = name;
		this.age = age;
	}
	
	@override
	public String to_string(){
		 return "Student{" + "name='" + name + '\'' + ", age='" + age + '\'' + '}';
	}
}
```

Step 2 : XML bean configuration 
```
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans/"
        xmlns:xsi="https://www.w3.org/2001/XMLSchema-instance"
        xsi:schemaLocation="http://www.springframework.org/schema/beans/
        https://www.springframework.org/schema/beans/spring-beans.xsd">
    <bean id="student" class="com.gfg.demo.domain.Student">
        <constructor-arg name="name" value="Tina"/>
        <constructor-arg name="age" value="21"/>
    </bean>
</beans>
```

Step 2  : Main class file
