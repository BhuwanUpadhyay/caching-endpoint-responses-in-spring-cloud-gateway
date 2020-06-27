# Caching endpoing responses in Spring Cloud Gateway

Blog: <https://bhuwanupadhyay/blog/blog-code-example-template/>

## Walkthrough

In microservice architecture the services are run in several different places at the same time means that any network delays will affect response time.
Also, othes factors like round trip time, a protocol’s handshake latency, time-to-first-byte and time-to-meaningful-response may cause the high latency of requests. To avoid this situation you can cache endpoint's responses in API Gateway. By doing this, you can reduce the number of calls made to your endpoint that ultimately helps to improve the latency of requests to your microservice.

<!--more-->

This blog post shows how it is applicable to cache response using Spring Cloud Gateway. For this you need to create two spring boot applications:
`api-gateway` and `order-service`.

## Initialize Projects

Run the following to create api gateway spring boot application:

```bash
curl https://start.spring.io/starter.tgz -d dependencies=actuator,cloud-gateway -d language=java -d platformVersion=2.3.1.RELEASE -d javaVersion=14 -d baseDir=api-gateway | tar -xzvf -
```

Run the following to create order microservice spring boot application:

```bash
curl https://start.spring.io/starter.tgz -d dependencies=actuator,webflux -d language=java -d platformVersion=2.3.1.RELEASE -d javaVersion=14 -d baseDir=order-service | tar -xzvf -
```

## Add Routing in API Gateway


## Implement Caching in API Gateway


We are done, Thanks for reading! [Github](https://github.com/BhuwanUpadhyay/blog-code-example-template)

## References
- https://bhuwanupadhyay.github.io/blog
- https://bhuwanupadhyay.github.io/cv
