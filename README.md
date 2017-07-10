# RESTCodeGen

Utility to generate a Spring Boot and gradle based application (deployable as a microservice) for exposing a resource via RESTFUL APIs. The generation of the application / APIscan be controlled via declarative config provided in appconfig.yaml. 

Given a resource (say car):

Generated code:
 - Spring Boot main application class 'Application.java' (if set to true in appconfig)
 - Model for the resource (Car.java) backed by a Abstract entity (AbstractEntity) for common attributes like ID etc
 - Controller to route http requests (CarController)
 - Service interfaces and implementation (CarService, CarServiceImpl)
 - Spring data Repository (CarRepository.java)
