# Constrained Device Application (Connected Devices)

## Lab Module 06

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Mi implementación del MqttClientConnector permite establecer una conexión con un broker MQTT, publicar mensajes en distintos tópicos y suscribirse a ellos según lo definido por el CDA. Se configura automáticamente usando los parámetros del archivo PiotConfig.props, como el host, puerto y tiempo de keep-alive. 

How does your implementation work?

El funcionamiento se basa en la biblioteca paho.mqtt.client, que facilita el manejo de conexiones, suscripciones y publicaciones. La clase se inicializa con un ID de cliente único y utiliza métodos como connectClient, disconnectClient, publishMessage y subscribeToTopic. Estos métodos permiten probar de forma controlada el envío y recepción de mensajes dentro del entorno IoT definido en el proyecto.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/python-components/tree/labmodule06


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
- 
- 

EOF.
