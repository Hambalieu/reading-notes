# Spring and Sockets and Functional Programming

- **WebSockets** is a *bi-directional*, *full-duplex*, *persistent connection* between a web browser and a server.
- Once a WebSocket connection is established the connection stays open until the client or server decides to close this connection.   
- A typical use case could be when an app involves multiple users communicating with each other, like in a chat.    

## Enable WebSocket in Spring
- The first thing to do is to enable the WebSocket capabilities.To do this we need to add a configuration to our application and annotate this class with ```@EnableWebSocketMessageBroker```.As its name suggests, it enables WebSocket message handling, backed by a message broker:

```
@Configuration
@EnableWebSocketMessageBroker
public class WebSocketConfig extends AbstractWebSocketMessageBrokerConfigurer {

    @Override
    public void configureMessageBroker(MessageBrokerRegistry config) {
        config.enableSimpleBroker("/topic");
        config.setApplicationDestinationPrefixes("/app");
    }

    @Override
    public void registerStompEndpoints(StompEndpointRegistry registry) {
         registry.addEndpoint("/chat");
         registry.addEndpoint("/chat").withSockJS();
    }
}
``` 

### Purely functional programming
- Purely functional programming usually designates a programming paradigm—a style of building the structure and elements of computer programs—that treats all computation as the evaluation of mathematical functions.
- Purely functional programming consists of ensuring that functions, inside the functional paradigm, will only depend on their arguments, regardless of any global or local state.
- A program is usually said to be functional when it uses some concepts of functional programming, such as first-class functions and higher-order functions.
- Purely functional data structures are persistent. Persistency is required for functional programming; without it, the same computation could return different results.
- Functional programming may use persistent non-purely functional data structures, while those data structures may not be used in purely functional programs.  

####Properties of purely functional programming

- Each evaluation strategy which ends on a purely functional program returns the same result.
- In particular, it ensures that the programmer does not have to consider in which order programs are evaluated, since eager evaluation will return the same result as lazy evaluation.
- An advantage of this is that lazy evaluation can be implemented much more easily; as all expressions will return the same result at any moment (regardless of program state), their evaluation can be delayed as much as necessary.

## Reference and Citation:
[Pure Functional Programming from Wikipedia](https://en.wikipedia.org/wiki/Purely_functional_programming)       
[Intro to websockets with Spring](https://www.baeldung.com/websockets-spring)
