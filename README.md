# Microservicios-productos
Aplicación orientada a micro-servicios, se desarrolla utilizando Netflix OSS (Eureka, Ribbon, Histrix, Zuul) , Spring cloud, Spring Boot, Apache maven, Java


Microservice-registration   ==> port: 1111      ==> dashboard de Eureka, encargado de descubrir los microservicios 
Microservice-edgeserver     ==> port: 8080      ==> Balanceador de carga, Zuul
Microservice-Hystrix-d...   ==> port: 8383      ==> Dashboard para el circuit Breaker, Hystrix    
Productos-Backend           ==> port: 2222      ==> Contiene los datos de los productos, se comunica vía rest
productos-client            ==> port: 3333      ==> Proyecto consumidor del microservicio productos, proyecto central.
