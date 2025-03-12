# Constrained Device Application (Connected Devices)

## Lab Module 03

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Mi implementación añade funcionalidades de simulación de sensores y actuación a la CDA. 
Utiliza un generador de datos para crear conjuntos de datos que representan lecturas de sensores de humedad, presión y temperatura. 
Estos datos se empaquetan como objetos de telemetría que contienen información adicional sobre el dispositivo. 
Además, se ha implementado un disparador de umbral simple que emite un comando de actuador simulado cuando se cumplen ciertas condiciones.

How does your implementation work?

    - Generación de Datos Simulados: Se utiliza un generador de datos para crear lecturas simuladas de sensores de humedad, presión y temperatura. 

    - Empaquetado de Telemetría: Los datos generados se encapsulan en objetos de telemetría que incluyen información detallada sobre el dispositivo.

    - Detección de Umbrales y Actuación Simulada: Se implementa un mecanismo que monitorea las lecturas de los sensores y, al detectar que ciertos umbrales predefinidos han    sido superados, emite comandos de actuación simulados. Estos comandos se registran mediante mensajes de log que indican que se ha procesado un evento de actuación.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/python-components/tree/labmodule03

### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ActuaTorDataTest, SensorDataTest, SystemPerformanceDataTest
- HumiditySensorSimTaskTest, PressureSensorSimTaskTest, TemperatureSensorSimTaskTest
- HumidifierActuatorSimTaskTest, HvacActuatorSimTaskTest
- BaseIoTDataTest
### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SensonAdapterManagerTest
- 
- 

EOF.
