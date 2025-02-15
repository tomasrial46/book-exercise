# Constrained Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

El objetivo principal es que la aplicación recopile y registre datos básicos  de rendimiento del sistema.

How does your implementation work?

- Revisar la plantilla de la aplicación principal del CDA: Asegurarse de que la aplicación pueda iniciar y detener la funcionalidad del SystemPerformanceManager.
- Crear el módulo SystemPerformanceManager: Este módulo será responsable de programar las tareas de recolección de datos de rendimiento del sistema.
- Conectar SystemPerformanceManager con el código principal del CDA: Integrar el módulo para que la aplicación principal pueda controlar el monitoreo del rendimiento.
- Crear BaseSystemUtilTask: Una clase base que contiene la funcionalidad central que heredarán otras tareas de monitoreo del sistema.
- Crear SystemCpuUtilTask y SystemMemUtilTask: Estas tareas recopilarán métricas de utilización de CPU y memoria, respectivamente.
- Integrar las tareas en SystemPerformanceManager: Permitir que SystemPerformanceManager inicie y detenga las tareas de monitoreo de rendimiento.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/tomasrial46/python-components/tree/labmodule02

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

- ConstrainedDeviceAppTest
- SystemPerformanceManagerTest
- 

EOF.
