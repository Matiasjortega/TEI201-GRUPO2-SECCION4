# Documentación de Software

## Contenido

### Diagramas de Flujo
Incluir diagramas de las funciones principales del sistema.
<img width="906" height="670" alt="image" src="https://github.com/user-attachments/assets/d5bee422-f448-43e2-b124-da2be0650366" />
usando el de relación de voltaje y ppm:
es de 0 a 5V, con la relación logaritmica, esto aplicando desde 200 ppm hasta 10000, su proposito es identificar las particulas por millon en el aire, retorna un voltaje especifico según las particulas por millon en el aire detectado por el componente, un ejemplo de su uso puede ser cuando se ocurre una fuga de gas dentro de una fabrica y se puede activar un sistema de seguridad segun lo ocurrido

**Formato:** PNG, PDF o draw.io



## Manual de Operación

Paso 1: conectar la alimentación del Arduino UNO y verificar que el sensor MQ-6, el LED y el buzzer estén correctamente conectados.

Paso 2: esperar 30 segundos para el calentamiento inicial del sensor. una vez finalizado este tiempo, el sistema comenzará a realizar mediciones automáticamente.
---

## Troubleshooting

### Problemas Comunes

*1. Alimentación incorrecta del módulo SIM800L*

Durante la implementación del módulo SIM800L se utilizó una fuente de alimentación con el voltaje adecuado, pero con una capacidad de corriente insuficiente. Esto provocó problemas en su funcionamiento, ya que el módulo necesita una corriente elevada, especialmente durante los picos de transmisión de datos. Una alimentación insuficiente puede ocasionar reinicios, pérdida de comunicación o fallas en el envío de mensajes SMS.

*Solución:* Utilizar una fuente externa que entregue el voltaje recomendado por el fabricante y que tenga capacidad para suministrar los picos de corriente requeridos por el módulo (que pueden acercarse a 2 A, según la versión). Verificar también que exista una conexión GND común entre el Arduino y el SIM800L.

*2. Condiciones ambientales inadecuadas para la calibración del sensor MQ-6*

Durante las pruebas no se contó con un ambiente suficientemente controlado o libre de posibles gases contaminantes para realizar una calibración de referencia confiable. La presencia de gases en el entorno, además de cambios de temperatura y humedad, puede modificar la resistencia y las lecturas del sensor, afectando la definición de los valores de referencia y los umbrales de activación.

*Solución:* Realizar la calibración en un ambiente controlado, con condiciones estables y siguiendo las recomendaciones de la hoja de datos del MQ-6. Permitir que el sensor alcance una estabilización adecuada antes de realizar las mediciones y ajustar los umbrales según las condiciones reales de operación.

*3. Conexión floja o deficiente del sensor MQ-6*

Una conexión suelta, inestable o con falso contacto entre el sensor MQ-6 y el Arduino puede provocar variaciones en la señal analógica de salida. Esto puede generar lecturas incorrectas, fluctuaciones o interrupciones en la medición. Como consecuencia, el voltaje leído por la entrada analógica puede no representar correctamente la respuesta del sensor ante la presencia de gas.

*Solución:* Revisar las conexiones del sensor, especialmente la alimentación (VCC), GND y la salida analógica (AO). Comprobar que los cables estén firmemente conectados y que no existan daños o contactos intermitentes. Repetir las mediciones después de asegurar las conexiones.
