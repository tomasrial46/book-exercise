# Gateway Device Application (Connected Devices)

## Lab Module 11

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

    Mi implementación permite una comunicación segura entre el Agente de Datos del Gateway (GDA) local y el servicio Ubidots, utilizando el protocolo MQTT. Esto facilita el envío de datos desde dispositivos IoT hacia la nube.

How does your implementation work?

    El sistema se construye actualizando el MqttClientConnector para gestionar conexiones, suscripciones y el manejo de mensajes. Se define una interfaz ICloudClient, que es implementada por la clase CloudClientConnector, la cual utiliza internamente el MqttClientConnector. Este conector se encarga de procesar los mensajes entrantes desde la nube y enviarlos al DeviceDataManager, permitiendo una integración fluida entre los dispositivos locales y en la nube.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/java-components/tree/labmodule11


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
- CloudClientConnectorTest
- 

Capturas Cloud:

![imagen](https://github.com/user-attachments/assets/37dd839d-adcf-46ac-9b18-8228baa3fd0d)

![imagen](https://github.com/user-attachments/assets/a73891dc-f8fd-42e7-ad05-4db82de19b53)

![imagen](https://github.com/user-attachments/assets/a331613e-f620-4c04-9f90-afe502af65e5)


EOF.
