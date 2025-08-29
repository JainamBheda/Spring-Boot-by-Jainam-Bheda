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