# OMS-IS-FileProcessor

Java version : 1.8

packaging the application:

mvn clean install

Running the application :

There are three application properties files having details of each environments

application-sb.properties
application-stage.properties
application-prod.properties

For sandbox: java -Xmx512m -Xms512m -jar fileprocessor-0.1.0.jar --spring.config.location=classpath:/application-sb.properties

For stage: java -Xmx512m -Xms512m -jar fileprocessor-0.1.0.jar --spring.config.location=classpath:/application-stage.properties

For prod: java -Xmx512m -Xms512m -jar fileprocessor-0.1.0.jar --spring.config.location=classpath:/application-prod.properties

# CICD - FileProcessor