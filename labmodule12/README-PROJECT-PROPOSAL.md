# Lab Module 12 - Semester Project Proposal

## Description

Describe your idea in 1 paragraph (at least 2 or 3 sentences).

En este proyecto, he ampliado una arquitectura IoT ya existente para incorporar un nuevo sensor de luz (LightSensor) y un actuador de luz (LEDLightActuator). La implementación cubre tanto el dispositivo cliente (CDA, en Python) como el gateway (GDA, en Java), permitiendo la recolección de datos de luz ambiental y la activación remota del LED desde la nube.

## What - The Problem 

What problem are you trying to solve and why does it matter? Write 1 to 2 paragraphs in response.

Actualmente, muchos sistemas IoT de monitoreo ambiental solo se enfocan en sensores de temperatura o humedad, dejando de lado la luminosidad, que es crucial para ambientes de trabajo, ahorro energético o agricultura de precisión. No poder medir y controlar las condiciones lumínicas limita el potencial de automatización.

Este proyecto aborda esa limitación implementando un sensor de luz que puede monitorear constantemente el nivel de iluminación. Y un actuador que es un ventilador pero que podría ser cualquier otro tipo de dispositivo.

## Why - Who Cares? 

Why do you care about this particular problem? Write 1 to 2 paragraphs in response.

Nos importa este problema porque los sistemas inteligentes deben adaptarse no solo al clima, sino también a las condiciones lumínicas o térmicas. Por ejemplo, en un invernadero, si la temperatura supera cierto umbral detectado por sensores, se puede activar automáticamente un ventilador para regular el ambiente y proteger las plantas del exceso de calor. Esto no solo mejora el control del entorno, sino que también contribuye al ahorro energético y al cuidado de los cultivos.


## How - Expected Technical Approach

How do you plan to tackle this problem technically?

El enfoque técnico se basa en el uso de MQTT/CoAP como protocolo de comunicación. El CDA recolecta datos del LightSensor y los envía al GDA. El GDA reenvía esta información a la nube. Estos datos definen la activación del ventilador.


## Results - Expected Outcomes 

If your project is successful, what outcome do you expect (e.g. what will happen if everything works)? Write 1 to 2 paragraphs describing your expected outcomes.

Que los datos lleguen correctamente al cloud.

EOF.
