# Constrained Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
La implementación mejora la seguridad del cliente MQTT mediante cifrado y permite el control remoto del humidificador. El dispositivo ahora puede recibir instrucciones del GDA a través de un topic específico y actuar en consecuencia.
La implementación mejora la seguridad del cliente MQTT mediante cifrado y permite el control remoto del humidificador. El dispositivo ahora puede recibir instrucciones del GDA a través de un topic específico y actuar en consecuencia.

How does your implementation work?

El cifrado se implementa usando tls_set junto con un certificado para establecer una conexión segura. Al recibir datos del topic, el cliente MQTT los procesa, el DeviceDataManager convierte el JSON en un objeto ActuatorData con ayuda de DataUtil, y el ActuatorDataManager actualiza el humidificador según lo indicado.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/python-components/tree/labmodule10


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
- DeviceDataManagerIntegrationTest
- DeviceDataManagerWithCommsTest
- DeviceDataManagerCallbackTest
- CoapClientPerformanceTest (mi ordenador no fue capaz de ejecutar el test con las 10000 iteraciones ya que tardaba mucho en cada una del bucle)
- MqttClientPerformanceTest:

        Connect and Disconnect: 1005.615245 ms
        
        Testing Publish: QoS = 0 | msgs = 10000 | payload size = 264 | start = 1748357429465917.8 | end = 1748357430335180.0 | elapsed = 0.8692623700000001
        Testing Publish: QoS = 1 | msgs = 10000 | payload size = 264 | start = 1748357431338123.2 | end = 1748357433984347.0 | elapsed = 2.646223843
        Testing Publish: QoS = 2 | msgs = 10000 | payload size = 264 | start = 1748357434988039.2 | end = 1748357440679236.2 | elapsed = 5.691196902

    QoS 0 fue el más rápido.
    QoS 2 fue el más lento, tomando más del 5x el tiempo de QoS 0.

EOF.
