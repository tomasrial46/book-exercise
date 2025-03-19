# Gateway Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

La implementación en el GDA gestiona los datos provenientes de los sensores y actuadores del CDA. Se encarga de recibir la información de los dispositivos conectados, procesarla y reenviarla a plataformas en la nube o sistemas de análisis. También maneja comandos enviados desde sistemas externos hacia el CDA, permitiendo la ejecución de acciones en los actuadores.

DeviceDataManager es el componente principal del GDA, responsable de la gestión de conexiones y del procesamiento de los datos. Maneja protocolos como MQTT y CoAP para la comunicación con los dispositivos y administra la transmisión eficiente de datos. Además, supervisa el rendimiento del sistema, incluyendo el uso de CPU y memoria, para garantizar una operación estable.

How does your implementation work?

La implementación funciona a través de una arquitectura modular que permite la gestión de datos y conexiones. Cuando se inicia el GDA, DeviceDataManager configura y establece las conexiones necesarias para comunicarse con el CDA mediante MQTT o CoAP. Luego, procesa los datos recibidos de los sensores, los almacena o los reenvía a servicios en la nube según sea necesario.

Cuando se reciben comandos, el GDA los traduce a un formato comprensible y los envía al CDA para su ejecución en los actuadores. DeviceDataManager también supervisa el rendimiento del sistema a través de SystemPerformanceManager, asegurando un funcionamiento óptimo. Al finalizar, el GDA cierra las conexiones activas y detiene la monitorización del sistema para evitar consumos innecesarios de recursos.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/java-components/tree/labmodule05


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ActuatorDataTest, SensorDataTest, SystemPerformanceDataTest, SystemStateDataTest
- DataUtilTest
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest
- DataIntegrationTest
- DeviceDataManagerNoCommsTest
- GatewayDeviceAppTest

EOF.
