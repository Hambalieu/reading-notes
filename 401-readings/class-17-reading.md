# Spring Authorization    

### Key point to note 

- It’s not a great idea to return a whole OAuth2User in an endpoint since it might contain information you would rather not reveal to a browser client.

### Key point when Making the Home Page Public

- To make the link visible, we also need to switch off the security on the home page by extending **WebSecurityConfigurerAdapter**:  

- The above configuration indicates a whitelist of permitted endpoints, with every other endpoint requiring authentication.

#### You want to allow:

- ```/``` since that’s the page you just made dynamic, with some of its content visible to unauthenticated users

- ```/error``` since that’s a Spring Boot endpoint for displaying errors.

- ```/webjars/**``` since you’ll want your JavaScript to run for all visitors, authenticated or not.



### Key points to note    
- You won’t see anything about ```/user``` in this configuration, though. Everything, including ```/user``` remains secure unless indicated because of the ```.anyRequest().authenticated()``` configuration at the end.

- Finally, since we are interfacing with the backend over Ajax, we’ll want to configure endpoints to respond with a 401 instead of the default behavior of redirecting to a login page. Configuring the ```authenticationEntryPoint``` achieves this for us.

### How to Add a Local User Database:

1. Choose a backend for your database, and set up some repositories (using Spring Data, say) for a custom User object that suits your needs and can be populated, fully or partially, from external authentication.    

2. Implement and expose OAuth2UserService to call the Authorization Server as well as your database. Your implementation can delegate to the default implementation, which will do the heavy lifting of calling the Authorization Server. Your implementation should return something that extends your custom User object and implements OAuth2User.      

####Hint:add a field in the User object to link to a unique identifier in the external provider (not the user’s name, but something that’s unique to the account in the external provider).



##Reference and Citation   
[Spring Boot and OAuth2](https://spring.io/guides/tutorials/spring-boot-oauth2/)