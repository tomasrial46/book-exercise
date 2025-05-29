# Gateway Device Application (Connected Devices)

## Lab Module 12 - Semester Project - GDA Components

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Se añaden los métodos necesarios para que sea capaz de recibir los datos nuevos que le llegan por MQTT o CoAP y se conecta a cloud para enviarlos como hace con el resto de sensores y actuadores.

How does your implementation work?

El GDA recibe datos del sensor de luz del CDA y los reenvía a la nube usando CloudClientConnector.

Cuando el GDA recibe ese comando a través del topic MQTT del actuador, el mensaje se procesa en el DefaultDataMessageListener, y se crea un ActuatorData que se reenvía al CDA para que active o desactive el ventilador.

Se han añadido tests de prueba al CloudClientConnectorTest para probar estos nuevos sensor/actuador.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/java-components/tree/labmodule12



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

- CloudClientConnectorTest
- 
- 

Capturas Cloud:
![alt text](<Imagen pegada.png>)
![alt text](<Imagen pegada (2).png>)
![alt text](<Imagen pegada (3).png>)


EOF.
