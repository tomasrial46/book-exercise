# Gateway Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-GDA-* issues.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

La implementación de GDA (Gateway Device App) se encarga de recopilar datos de rendimiento del sistema, como la utilización de la CPU y la memoria, a intervalos regulares. Además, gestiona y programa estas tareas de recolección de datos y registra la información recopilada utilizando el sistema de logs.

How does your implementation work?

- Módulo SystemPerformanceManager:

    Se crea este módulo para gestionar la programación de las tareas de recopilación de datos de rendimiento del sistema.

- Clase BaseSystemUtilTask:

    Una clase base que proporciona funcionalidades principales para las tareas de monitoreo del rendimiento del sistema.

- Clases SystemCpuUtilTask y SystemMemUtilTask:

    Estas clases heredan de BaseSystemUtilTask y se encargan de recopilar métricas de utilización de CPU y memoria del sistema local.

- Integración con SystemPerformanceManager:

    SystemCpuUtilTask y SystemMemUtilTask se conectan con SystemPerformanceManager, lo que permite iniciar y detener las tareas de monitoreo del rendimiento.

- Registro y Programación de Datos:

    Los datos recopilados se registran mediante el sistema de logs a intervalos predefinidos. La aplicación utiliza un mecanismo de sondeo (polling) que recopila y registra las métricas de rendimiento del sistema.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/java-components/tree/labmodule02


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- SystemCpuUtilTaskTest
- SystemMemUtilTaskTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- GatewayDeviceAppTest
- SystemOerformanceManagerTest (Modificado para poder ser usado con funciones booleanas)
- 

EOF.
