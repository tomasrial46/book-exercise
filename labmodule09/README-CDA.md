# Constrained Device Application (Connected Devices)

## Lab Module 09

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Implementación de un cliente de CoAP que permite el envío y recibo de mensajes a través de su red. Dicho cliente puede realizar solicitudes del tipo GET, POST, PUT y DELETE.

How does your implementation work?

La implementación usa CoAPthon para crear un cliente CoAP que se comunica con el GDA. Construye rutas a recursos y envía solicitudes según el tipo (GET, POST, etc.), con soporte para observadores. Las respuestas se procesan y, si es necesario, se notifican a un listener que integra los datos al sistema mediante la interfaz IDataMessageListener.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/python-components/tree/labmodule09



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

- CoapClientConnectorTest
- 
- 

EOF.
