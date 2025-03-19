# Constrained Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

La implementación en el CDA gestiona los datos de sensores y actuadores, permitiendo su serialización y deserialización en formato JSON. Se encarga de capturar, procesar y transmitir los datos recopilados por los sensores del dispositivo, así como de recibir y ejecutar comandos en los actuadores. Además, administra la comunicación con el GDA a través de protocolos como MQTT y CoAP.

SensorDataManager y ActuatorDataManager son los componentes principales que manejan la adquisición y transformación de datos en el CDA. Estos módulos procesan la información del hardware del dispositivo y la convierten en un formato estructurado antes de enviarla al GDA. T

How does your implementation work?

La implementación funciona mediante la gestión estructurada de los datos del dispositivo en clases específicas para sensores y actuadores. Cuando se inicia el sistema, SensorDataManager comienza a recopilar información de los sensores y la serializa a JSON antes de transmitirla. Al mismo tiempo, ActuatorDataManager monitorea los mensajes entrantes, los deserializa y ejecuta las acciones correspondientes en los actuadores del dispositivo.

El CDA utiliza MQTT o CoAP para enviar y recibir datos, asegurando una comunicación eficiente con el GDA. Los datos enviados incluyen valores de sensores como temperatura, humedad o presión, mientras que los datos recibidos contienen comandos que los actuadores deben ejecutar. Finalmente, cuando el sistema se apaga, los gestores de datos detienen sus procesos y cierran las conexiones activas.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/python-components/tree/labmodule05


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- DataUtilTest
- 
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest
- DataIntegrationTest
- 

EOF.
