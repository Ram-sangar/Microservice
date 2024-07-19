# Microservice
First Microservice Project
Eureka :-
only need eureka server,spring web dependency
add annotation in application file @EnableDiscoveryClient

properties:-
spring.application.name=eureka-server
server.port=8761
eureka.client.registerWithEureka=false
eureka.client.fetchRegistry=false

if any error in logging not in dependency then press refresh button in intellij.....

___________________________________________________________________________________________________________________________

Product service:-
dependency:-JPA,MYSQL,LOMBOK,EUREKA SERVICE
add annotation in application file @EnableDiscoveryClient
create Integration-user-model,erole,service

properties:-
spring.application.name=product-microservice

server.port=8762
eureka.client.serviceUrl.defaultZone=http://localhost:8761/eureka
eureka.instance.preferIpAddress=true
eureka.client.fetch-registry=true

eureka.client.register-with-eureka=true

spring.jpa.hibernate.ddl-auto=update
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.datasource.url=jdbc:mysql://localhost:3306/product_schema
spring.datasource.username=root
spring.datasource.password=root

spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect
spring.jpa.generate-ddl=true
spring.jpa.show=true
logging.level.org.hibernate.SQL=DEBUG
logging.level.org.hibernate.type=TRACE



