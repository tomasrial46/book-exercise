# Gateway Device Application (Connected Devices)

## Lab Module 08

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Implementación de servidor Coap para mejorar la comunicación entre dispositivos.

How does your implementation work?

La clase CoapServerGateway crea un servidor CoAP que organiza los recursos según rutas jerárquicas definidas. Al iniciar, registra manejadores que procesan los mensajes entrantes, lo que asegura flexibilidad y compatibilidad con el modelo del GDA.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/java-components/tree/labmodule08


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- 
- 
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- CoapServerGatewayTest
- 
- 

EOF.
