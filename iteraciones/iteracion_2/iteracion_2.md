# Iteración 2 - Primera Mejora Significativa

## Información General

**Fecha:** [5/11/2026]  
**Versión:** v2.0  
**Estado:** Prototipo funcional mejorado  
**Avance asociado:** Avance #2

---

Descripción

En la segunda iteración del proyecto se buscó mejorar el prototipo inicial del detector de fugas de gas, incorporando nuevas ideas que permitieran aumentar su funcionalidad, seguridad y autonomía.

A diferencia de la primera versión, que contemplaba principalmente un sistema de detección mediante Arduino y una alerta visual LED, en esta etapa se propuso integrar un módulo SIM800L para enviar notificaciones por SMS, un buzzer para generar alertas sonoras y una batería externa para permitir el funcionamiento independiente del computador.

Además, se comenzó a considerar el diseño de un encapsulado que permitiera proteger y organizar los componentes electrónicos.

Objetivos de esta iteración:

Mejorar el funcionamiento del sistema de detección de gas.

Evaluar la incorporación de alertas mediante SMS y sonido.

Considerar una fuente de alimentación externa para aumentar la autonomía.

Iniciar la planificación del encapsulado del dispositivo.

Identificar las mejoras necesarias para la versión final.

Cambios Respecto a v1

Hardware

Componentes propuestos:

Módulo SIM800L: permitiría enviar mensajes SMS para advertir sobre posibles fugas de gas.

Buzzer: permitiría emitir una alarma sonora al detectar una concentración peligrosa de gas.

Batería externa: permitiría alimentar el Arduino sin mantenerlo conectado permanentemente al computador.

Modificaciones planteadas:

Sistema de alertas: ampliar la alerta visual LED mediante la incorporación de notificaciones sonoras y remotas.

Sistema de alimentación: reemplazar la dependencia del computador por una fuente de energía independiente.

Componentes removidos:

Durante esta iteración no se contempló eliminar componentes principales del prototipo inicial.

Software

Nuevas funcionalidades propuestas:

Incorporar instrucciones para activar un buzzer cuando se detecte una fuga de gas.

Evaluar la programación del módulo SIM800L para enviar mensajes de advertencia.

Mantener el funcionamiento de la alerta visual LED.

Optimizaciones previstas:

Mejorar la coordinación entre el sensor de gas y los diferentes sistemas de alerta.

Adaptar el programa para incorporar nuevos componentes sin afectar el funcionamiento principal del detector.

Errores y aspectos por corregir:

Evaluar la compatibilidad de los nuevos componentes con el sistema existente.

Comprobar el funcionamiento de las nuevas alertas antes de incorporarlas a la versión final.

Diseño Mecánico

Durante esta etapa se comenzó a planificar el encapsulado del detector utilizando Fusion 360 como herramienta de diseño.

El objetivo era desarrollar una estructura capaz de contener y proteger los componentes electrónicos, considerando espacios para la ventilación, la visualización de la luz LED y el acceso a las conexiones necesarias.

También se evaluó la distribución interna de los componentes para facilitar su posterior montaje.

Resultados de Testing

Funcionalidad Lograda

✅ Se mantuvo como función principal la detección de fugas de gas mediante el sensor y Arduino.

✅ Se conservó el sistema de alerta visual mediante luz LED.

✅ Se identificaron nuevas funcionalidades para mejorar la seguridad del dispositivo.

⚠️ El envío de SMS, la alerta sonora y la alimentación mediante baterías quedaron pendientes de implementación y evaluación en la siguiente iteración.

Acciones de mejora propuestas:

Evaluar la viabilidad de incorporar los nuevos sistemas de alerta.

Avanzar en el desarrollo del encapsulado y la integración de los componentes electrónicos.

Testing con Usuarios

Durante esta etapa se consideró la importancia de evaluar la utilidad y facilidad de uso del detector.


Feedback cualitativo:

Se identificó la necesidad de que el dispositivo fuera fácil de utilizar, tuviera alertas claras y pudiera funcionar sin depender permanentemente de un computador.

Problemas Pendientes

1. Implementación de nuevas alertas

Descripción: Se propuso incorporar un módulo SIM800L y un buzzer para complementar la alerta visual, pero todavía era necesario comprobar su funcionamiento e integración.

Plan para v3: Realizar pruebas con los nuevos componentes y determinar cuáles podían incorporarse de manera confiable al sistema final.

2. Dependencia de alimentación externa

Descripción: El prototipo inicial dependía de una conexión al computador para recibir energía, lo que limitaba su autonomía y posibilidades de instalación.

Plan para v3: Implementar una fuente de alimentación mediante baterías para permitir el funcionamiento independiente del dispositivo.

3. Desarrollo del encapsulado

Descripción: Era necesario diseñar una estructura que protegiera los componentes electrónicos y permitiera su correcta distribución y ventilación.

Plan para v3: Avanzar en el diseño de Fusion 360 y desarrollar el encapsulado físico mediante corte láser en MDF.

Plan para Iteración 3 (Versión Final)

Mejoras Críticas

Hardware:

Realizar pruebas de funcionamiento con el módulo SIM800L.

Implementar el buzzer para generar alertas sonoras.

Incorporar baterías para alimentar el dispositivo.

Integrar los componentes electrónicos en una estructura física.

Software:

Programar el funcionamiento de la alarma sonora.

Evaluar el envío de notificaciones mediante SMS.

Ajustar el código para asegurar el funcionamiento de los sistemas de alerta.

Diseño:

Finalizar el modelo del encapsulado en Fusion 360.

Incorporar ventilaciones y espacios para conexiones.

Fabricar las piezas utilizando corte láser en MDF.

Realizar el montaje de los componentes.

Testing:

Comprobar el funcionamiento del sistema de detección.

Evaluar el funcionamiento del buzzer.

Verificar la autonomía mediante baterías.

Determinar si el módulo SIM800L puede integrarse correctamente.

Evaluar el funcionamiento general del prototipo final.

Archivos en esta Carpeta

v2_codigo.ino - Código correspondiente a la segunda versión, si se conserva.

v2_esquema.png - Esquema de conexiones del prototipo.

v2_modelo3d.f3d - Diseño inicial del encapsulado, si se desarrolló en esta etapa.

v2_fotos/ - Fotografías de los avances realizados.

v2_feedback.pdf - Comentarios recibidos durante el segundo avance, si fueron documentados.
