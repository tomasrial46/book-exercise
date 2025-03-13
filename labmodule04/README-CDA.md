# Constrained Device Application (Connected Devices)

## Lab Module 04

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Mi implementación permite la simulación y prueba de un sistema de IoT sin necesidad de hardware físico, utilizando el emulador Sense HAT. 
A través de la CDA, se generan datos de sensores de temperatura, humedad y presión, y se procesan comandos de actuación para simular el control de dispositivos como humidificadores y sistemas HVAC. 
Además, la pantalla LED del emulador se utiliza para visualizar mensajes, facilitando la validación del comportamiento del sistema.

How does your implementation work?

La implementación se basa en la interacción entre la CDA y el emulador Sense HAT. 
Los sensores simulados del emulador generan datos en tiempo real, los cuales son recogidos por la CDA para su procesamiento y análisis. 
Cuando se envía un comando a un actuador (como encender o apagar un humidificador), la CDA ejecuta la acción correspondiente y actualiza la pantalla LED del emulador para visualizarlo. 

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/python-components/tree/labmodule04


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

- SenseHatEmulatorQuickTest
- HumidityEmulatorTaskTest, PressureEmulatorTaskTest, TemperatureEmulatorTaskTest
- HumidifierEmulatorTaskTest, HvacEmulatorTaskTest, LedDisplayEmulatorTaskTest
- SensorEmulatorManagerTest
- ActuatorEmulatorManagerTest

EOF.
