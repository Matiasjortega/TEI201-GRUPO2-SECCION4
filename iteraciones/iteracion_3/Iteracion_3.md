# Iteración 3 - Versión Final

## Información General

**Fecha:** [20/11/2026]  
**Versión:** v3.0  
**Estado:** Prototipo de alta resolución - Versión final  
**Avance asociado:** Avance #3

---

Historial de Iteraciones

Propósito

Esta sección documenta la evolución del detector de fugas de gas a través de las tres iteraciones realizadas durante el proyecto. Su objetivo es demostrar cómo el prototipo fue mejorando progresivamente mediante la incorporación de nuevas funcionalidades, la identificación de problemas y la búsqueda de soluciones.

El proceso permitió transformar una propuesta inicial basada en Arduino y una alerta visual LED en un dispositivo con alertas visuales y sonoras, alimentación mediante baterías y un encapsulado diseñado para proteger sus componentes.

Estructura de Carpetas

Cada iteración cuenta con una carpeta que contiene la documentación correspondiente a esa etapa del proyecto.

iteraciones/
├── iteracion_1/    # Concepto inicial
├── iteracion_2/    # Propuestas de mejora
└── iteracion_3/    # Versión final

Evolución del Diseño

Versión 1 (Iteración 1) - Concepto Inicial

Fecha: [Fecha correspondiente]

Estado: Prototipo inicial.

Características:

En la primera iteración se desarrolló el concepto básico del detector de fugas de gas. La propuesta consistía en utilizar un Arduino conectado a un sensor de gas y una luz LED que permitiera advertir visualmente sobre la presencia de gas.

El objetivo principal era establecer una solución sencilla que permitiera detectar posibles fugas y generar una advertencia.

Problemas principales identificados:

La alerta dependía únicamente de una señal visual.

El dispositivo necesitaba estar conectado a un computador para recibir alimentación.

No se contaba con un encapsulado que protegiera los componentes.

Aprendizajes clave:

Se identificó la necesidad de incorporar mecanismos adicionales de alerta, mejorar la autonomía del dispositivo y desarrollar una estructura que facilitara su instalación y utilización.

Versión 2 (Iteración 2) - Primera Mejora

Fecha: [5/11/2026]

Estado: Prototipo funcional en proceso de mejora.

Mejoras propuestas:

Durante la segunda iteración se plantearon nuevas funcionalidades destinadas a mejorar la seguridad y autonomía del detector.

Incorporación de un módulo SIM800L para enviar alertas mediante SMS.

Incorporación de un buzzer para generar advertencias sonoras.

Utilización de baterías para permitir el funcionamiento independiente del computador.

Planificación de un encapsulado para proteger y organizar los componentes electrónicos.

Problemas pendientes:

Comprobar el funcionamiento del módulo SIM800L.

Implementar el sistema de alerta sonora.

Integrar una fuente de alimentación independiente.

Desarrollar y fabricar el encapsulado físico.

Esta iteración permitió definir las principales mejoras que se intentarían implementar en la versión final.

Versión 3 (Iteración 3) - Versión Final

Fecha: [20/11/2026] 

Estado: Prototipo final desarrollado.

Mejoras finales:

En la tercera iteración se implementaron las principales modificaciones propuestas anteriormente, buscando obtener un dispositivo más completo, autónomo y adecuado para su utilización.

Alerta sonora: se incorporó un buzzer para complementar la advertencia visual mediante LED.

Alimentación independiente: se implementó un sistema de baterías para que el Arduino pudiera funcionar sin permanecer conectado al computador.

Evaluación del módulo SIM800L: se realizaron intentos de integración para enviar mensajes SMS. Sin embargo, debido a dificultades de funcionamiento, se decidió descartar esta funcionalidad.

Encapsulado: se desarrolló el diseño final en Fusion 360 y se fabricó una estructura utilizando corte láser sobre MDF de 3 mm.

Distribución de componentes: se consideraron espacios para el sensor, la luz LED, las conexiones y los demás componentes electrónicos.

Ventilación: se incorporaron aberturas para facilitar el contacto del sensor con el aire exterior.

Resultado:

Se obtuvo una versión más completa del detector, que combina alertas visuales y sonoras, alimentación independiente y una estructura física diseñada para contener los componentes.

Aunque no fue posible incorporar las notificaciones mediante SMS, esta decisión permitió concentrar los esfuerzos en las funcionalidades principales del dispositivo.

Justificación de Cambios

Hardware

De v1 a v2:

Cambio: Se propuso incorporar un buzzer, un módulo SIM800L y una fuente de alimentación mediante baterías.

Razón: El prototipo inicial presentaba limitaciones relacionadas con su sistema de advertencia y su dependencia de una conexión al computador.

Impacto: Se amplió la propuesta inicial al considerar distintas formas de notificación y una mayor autonomía.

De v2 a v3:

Cambio: Se implementaron el buzzer y las baterías, mientras que el módulo SIM800L fue descartado después de presentar dificultades de funcionamiento.

Razón: Se buscó priorizar un sistema de alerta funcional y evitar depender de un componente que no había logrado operar correctamente.

Impacto: El dispositivo incorporó una advertencia sonora adicional y dejó de depender exclusivamente de la alimentación del computador.

Software

De v1 a v2:

Se planteó ampliar la programación inicial para permitir el funcionamiento de nuevos sistemas de alerta, especialmente el buzzer y el envío de mensajes mediante el módulo SIM800L.

De v2 a v3:

Se adaptó la programación para incorporar la alerta sonora junto con la alerta visual existente. Además, se descartó la función de envío de SMS debido a los problemas encontrados con el módulo SIM800L.

De esta manera, se priorizó el funcionamiento de los mecanismos de advertencia incorporados al prototipo final.

Diseño 3D

De v1 a v2:

Durante las primeras etapas no se contaba con un encapsulado físico. Posteriormente, se comenzó a planificar una estructura que permitiera contener los componentes electrónicos, protegerlos y facilitar su organización.

De v2 a v3:

Se avanzó en el diseño mediante Fusion 360, considerando las dimensiones de los componentes y las necesidades del detector.

Inicialmente se exploró la posibilidad de fabricar el encapsulado mediante impresión 3D. Sin embargo, se decidió utilizar corte láser sobre MDF de 3 mm.

El diseño final incluyó paredes, tapa superior, aberturas de ventilación, espacios para conexiones y un sistema para ubicar la luz LED.

Este cambio permitió desarrollar una estructura física adaptada a los materiales y métodos de fabricación disponibles.

Incorporación de Feedback

Feedback del Avance #1 → Cambios en v2

A partir de las limitaciones identificadas en la primera versión, se reconoció la necesidad de mejorar el sistema de advertencia y aumentar la autonomía del dispositivo.

Acciones tomadas:

Se propuso incorporar una alerta sonora mediante un buzzer.

Se consideró el envío de mensajes SMS utilizando un módulo SIM800L.

Se planteó utilizar baterías para alimentar el Arduino.

Se comenzó a considerar el diseño de un encapsulado.

Feedback del Avance #2 → Cambios en v3

Durante el desarrollo de las funcionalidades propuestas, se identificaron dificultades técnicas que obligaron a reconsiderar algunos elementos.

Acciones tomadas:

Se implementó el sistema de alerta sonora.

Se incorporó la alimentación mediante baterías.

Se descartó el módulo SIM800L debido a problemas de funcionamiento.

Se avanzó en el diseño y fabricación del encapsulado definitivo.


Como criterios de diseño, se priorizaron la claridad de las alertas, la facilidad de utilización y la independencia de una conexión permanente al computador.

Estas consideraciones orientaron la incorporación del buzzer, las baterías y el encapsulado del dispositivo.

Lecciones Aprendidas

Técnicas

Integración de componentes: se aprendió que agregar nuevas funcionalidades requiere comprobar la compatibilidad y el funcionamiento de cada componente antes de integrarlo al sistema completo.

Evaluación de alternativas: las dificultades con el módulo SIM800L demostraron la importancia de reconocer cuándo una solución no resulta viable y buscar alternativas que permitan mantener la funcionalidad principal.

Diseño y fabricación: se adquirió experiencia en el uso de Fusion 360 y en la adaptación de un diseño a un proceso de fabricación mediante corte láser.

De Proceso

Importancia de las iteraciones: desarrollar el proyecto en diferentes versiones permitió identificar problemas, incorporar mejoras y modificar decisiones iniciales.

Planificación: se comprendió la importancia de evaluar los materiales, componentes y métodos de fabricación disponibles antes de definir una solución final.

Resolución de problemas: las dificultades técnicas permitieron aprender a modificar el diseño sin perder de vista el objetivo principal del proyecto.

De Trabajo en Equipo

Distribución de responsabilidades: el desarrollo del prototipo requirió organizar las actividades relacionadas con la electrónica, programación y diseño del encapsulado.

Comunicación: fue importante compartir los avances y dificultades para coordinar las modificaciones del dispositivo.

Toma de decisiones: el equipo debió evaluar distintas alternativas y llegar a acuerdos, especialmente al descartar el módulo SIM800L y seleccionar el método de fabricación del encapsulado.

Conclusión del Proceso Iterativo

El desarrollo de las tres iteraciones permitió transformar una idea inicial sencilla en un prototipo con mayores funcionalidades y una estructura física definida.

Durante este proceso se identificaron limitaciones, se propusieron soluciones y se realizaron modificaciones en función de las dificultades encontradas. La incorporación del buzzer, el uso de baterías y la fabricación del encapsulado representaron los principales avances del proyecto.

Asimismo, el descarte del módulo SIM800L demostró que el proceso iterativo no consiste únicamente en agregar funcionalidades, sino también en evaluar su viabilidad y tomar decisiones que favorezcan el funcionamiento del sistema.

En conjunto, estas mejoras permitieron avanzar hacia el objetivo principal del proyecto: contribuir a la seguridad de los hogares mediante la detección y advertencia de posibles fugas de gas.
