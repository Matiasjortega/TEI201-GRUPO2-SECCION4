# Iteración 1 - Concepto Inicial

## Información General

**Fecha:** [25/10/2025]  
**Versión:** v1.0  
**Estado:** Prototipo alpha - Prueba de concepto  
**Avance asociado:** Planificación inicial / Avance #1

---

## Descripción

Primera versión del prototipo, enfocada en validar el funcionamiento del sistema de detección de fugas de gas mediante un sensor MQ-6.

**Objetivo de esta iteración:**
- Validar la lectura del sensor MQ-6
- Calibrar el sensor de detección de gas 
- Visualizar el prototipo de forma fisica

---

## Componentes Utilizados

### Hardware
- Microcontrolador: ATmega328P 
- Sensores:
  - MQ-6
- Actuadores:
  - Luz led
- Otros: 
  - Protoboard
  - Cable USB tipo B
  - Baterias
  - Cables Dupont
  
### Software
- IDE: Arduino IDE 2.3.6
- Versión código: v1.0

---

## Fotos del Prototipo

Incluir en esta carpeta:
- `Imagen prototipo 3.jpeg`

---

## Resultados de Testing Inicial

### Funcionalidad Lograda
✅ Lectura del sensor de gas 
✅ calibración del sensor para detectar gas en una escala mas pequeña
❌ Al detectar gas que el usuario reciba un SMS
❌ Prototipado 3D completo
### Problemas Identificados

1. **Problema 1:**
   - Descripción: Mensaje SMS al detectar gas
   - Causa probable: No contamos con las herramientas para el chip de SMS]
   - Solución propuesta: Conseguir el adaptador y adaptar el código para que funciona

2. **Problema 2:**
   - Descripción: Prototipado 3D completo
   - Causa probable: Falta de conocimiento en el uso de fusion 360
   - Solución propuesta: Profundizar mas en fusion 360 y mejorar el modelo

---

## Aprendizajes

### Técnicos
- Calibrar de forma correcta el arduino 
- Calibrar correctamente el sensor MQ-6
### De Diseño
- Se requiere un orden para colocar los objetos dentro del modelo

---

## Plan para Iteración 2

### Mejoras Planificadas

**Hardware:**
-Mejorar la organizacion del circuito

**Software:**
- Implementar SMS

**Diseño:**
- Mejorar modelado 3D
- Definir la distribucion de los componentes

---

## Archivos en esta Carpeta

- `Imagen prototipo 3.jpeg`
- `Codigo_V1`
