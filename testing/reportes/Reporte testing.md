# Reportes de Testing

## Formato del Reporte Principal

### `reporte_testing_usuarios_v3.pdf`

**Estructura sugerida:**

1. **Introducción**
   - Objetivo del testing: mostrar el funcionamiento del objeto, en este caso sera conectado al pc, para mostrar la lectura de datos,
en la sección de testing se encuentra un video de la prueba con baterias.
   - Metodología utilizada: En primer lugar, se coneta el Arduino al pc, luego de esto se esperan 30 segundos, después se ve que el Arduino este tomando datos de forma correcta, posteriormente se aplica gas al sensor, cuando el sensor se activa, se prende la luz led y el buzzer, para finalizar se deja de darle gas al detector y se espera a que se apaguen la luz led y el buzzer para desconectar el aruino.

2. **Descripción de Participantes**
   - Perfil de usuario: El problema puede afectar a cualquier persona que viva en una casa donde se utilicen artefactos a gas. Sin embargo, hay situaciones en las que puede ser más difícil darse cuenta de una fuga, por ejemplo cuando una persona vive sola, está durmiendo, está en otra habitación o tiene dificultades para percibir olores.
   - Cantidad y demografía: Además, las fugas detectadas y reparadas mediante patrullajes aumentaron de 1.835 en 2020 a 3.197 en 2021. Esto representa un aumento importante y muestra que las fugas siguen siendo un problema que necesita atención.
La SEC también registró 357 reclamos relacionados específicamente con fugas de gas durante 2021. Este número corresponde a reclamos y no significa que sean fugas de gas, pero sirve para mostrar que este tipo de situaciones sí llega a ser reportado.
Nuestro proyecto se enfoca en un contexto urbano como Santiago, donde viven millones de personas y existe una gran cantidad de viviendas y edificio. De los cuales aproximadamente un 87% utiliza gas para cocinar.
Esto hace que el problema sea relevante para muchas personas. Además, en edificios una emergencia puede afectar no solamente a un departamento, sino también a otras personas que viven en el mismo lugar.
Realizamos una encuesta y obtuvimos 114 respuestas. De ellas, 107 personas, equivalentes al 93,9%, dijeron vivir en un hogar donde se utiliza gas.
Entre los artefactos que tenían en sus hogares, los más comunes fueron la cocina, con 82,2%, el calefón, con 56,1%, la estufa, con 43,0%, el horno, con 35,5%, y la parrilla, con 28,0%.
Cuando preguntamos qué tan seguras se sentían de poder detectar una fuga a tiempo, solamente un 20,2% respondió que se sentía muy seguro. Un 50,9% dijo sentirse algo seguro y un 28,1% poco seguro.
También encontramos que un 14,9% dijo que le resulta difícil detectar el olor o que no lo puede percibir bien.
Finalmente, un 97,4% consideró útil o muy útil tener una alerta visual. Además, 86 personas la calificaron como muy útil.

3. **Protocolo Aplicado**
   - Paso 1: conectar el Arduino UNO al pc.
   - Paso 2: Esperar 30 segundos para que empiece a detectar datos
   - Paso 3: Aplicar gas al sensor MQ-6
   - Paso 4: Esperar a que se activen la luz led y el buzzer
   - Paso 5: al activarse la led y el buzzer, se le deja de dar gas al sensor y se espera a que se apaguen
   - Paso 6: desconectar el Arduino UNO y dar por finalizado el testing
   - Preguntas realizadas: ¿Detectara de forma correcta el gas el sensor? ¿Las conexiones en el dispositivo estarán correctas? ¿Las baterías funcionaran con nuestro producto? ¿Sera mejor disminuir el intervalo en el que el sensor detecta valores para disminuir el consumo de las baterias?

4. **Resultados Cuantitativos**
Como se menciono con anterioridad, se hizo una encuesta para ver que tan grande es el problema.
Con respecto a los valores que detecta el sensor: Usamos el codigo analogRead() para la conversión de Voltaje (0V a 5V) a un valor fijo (0 a 1023), bajo la funcion siguiendo regla de tres, la función para identificar el voltaje es: f(x) = x*5V/1023, donde x es el valor entregado por analogRead(), como sigue una relación lineal la conversión es directa.
El valor del voltaje se procesa, para identificar las ppm entregadas por el arduino, podemos aplicar una interppara aproximar la función de ppm a voltaje, podemos evaluar la resistencia interna del sensor donde la ecuación divisora del voltaje presenta Vrl = Vc(Rl/(Rs+Rl)),
 Vrl = Vol salida que mide arduino
Vc = Voltaje alimentación circuito
Rl = Resistencia de carga (4700 amperes)
Rs = Resistencia sensible al gas
al despejar la ecuación:
Rs = Rl((Vc/Vrl)- 1),
al agregar una resistencia de referencia (R0) mediante un proceso de calibración con una concentración conocida de gas, podemos identificar:
log(Rs/R0) = m*log(ppm) + b,
Despejando:
ppm = 10^((log(Rs/R0)-b)/m)

6. **Resultados Cualitativos**
Nuestro principal problema fue no poder agregar la función de SMS al prototipo, ya que por temas de especificaciones no contábamos con las herramientas necesarias para usarlo.
7. **Validación de Impacto ODS**
Principalmente nuestr produco solo emitia una luz roja, lo cual puede no ser muy util en un caso de emergencias, especialmente si la persona se ecneuntra en otro lugar donde no se vea la luz, por lo que si aportaba a la ODS 3 y a la ODS 11, pero no era muy eficaz. Nuestro prototipo actual, no solo muestra una luz roja, tambien hace un ruido molesto para que el usuario sepa que esta en peligro, no es necesario que este cerca. Esto aumenta el aporte en las ODS 3 y ODS 11, ya que genera un ambiente aun mas seguro
8. **Conclusiones**
   - Fortalezas del prototipo: El prototipo es comodo de usar, puede ser transladado a cualquier lugar de la casa sin ningun problema. Tambien el ruido que genera es momesto, lo que hace facil escucharlo.
   - Limitaciones identificadas: No se pudo conectar al usuario por SMS al haber una fuga de gas. También el principal problema es que el objeto debe de estar siempre conectado y no sabemos si puede estar conectado a corriente. Las baterías son recargables, así que pueden recargarse al acabar su uso.
   - Recomendaciones para mejoras futuras
Buscar la manera de implementar SMS, tambien investigar si puede estar conectado mediante enchufe.


