# Gateway Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Recibir asíncronamente información del CDA y procesarla.

How does your implementation work?

La comunicación se hace asíncrona usando MqttAsyncClient con soporte de encriptación, y se adapta MqttClientConnector para ello. Se agregan listeners que validan los mensajes y los envían al DeviceDataManager, que decide si el valor está fuera de rango.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/java-components/tree/labmodule10



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
- DeviceDataManagerSimpleCdaActuationTest
- CoapClientPerformanceTest:

        PUT - CON: 6 ms

        PUT - NON: 1 ms

        POST - CON: 0 ms

        POST - NON: 1 ms

Más rápido: POST - CON (0 ms)
Más lento: PUT - CON (6 ms)

- MqttClientPerformanceTest:

        Connect and Disconnect: 307 ms

        Testing Publish: QoS = 0 | msgs = 10000 | payload size = 212 | start = 1.748357E9 | end = 1.748357E9 | elapsed = 2.074
        Testing Publish: QoS = 1 | msgs = 10000 | payload size = 212 | start = 1.748357E9 | end = 1.748357E9 | elapsed = 2.388
        Testing Publish: QoS = 2 | msgs = 10000 | payload size = 212 | start = 1.748357E9 | end = 1.748357E9 | elapsed = 4.798

QoS 0 fue el más rápido. 
QoS 2 fue el más lento, tomando más del doble del tiempo de QoS 0.


EOF.
