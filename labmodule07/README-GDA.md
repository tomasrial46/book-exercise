# Gateway Device Application (Connected Devices)

## Lab Module 07

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Mi implementación permite la comunicación bidireccional utilizando MQTT. El cliente MQTT en el GDA publica mensajes en un servidor MQTT y se suscribe a temas específicos para recibir datos en tiempo real.

How does your implementation work?
El cliente MQTT en el GDA se conecta a un broker, se suscribe a temas relevantes y publica mensajes en otros temas. Utiliza la biblioteca MQTT para Java para manejar la comunicación de manera asincrónica.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/java-components/tree/labmodule07


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

- MqttClientConnectorTest
- MqttClientControlPacketTest
- 

EOF.
