# Cuestionario de Evaluación: Comunicación por Sockets 📝

**Nombre del Estudiante:** Adriana Murcia 
**Fecha:** 11-03-2026

*Instrucciones: Responde a las siguientes preguntas basándote en la teoría de redes y en el análisis del código de nuestro proyecto. Sube este archivo con tus respuestas a tu repositorio como evidencia de trabajo.*

1. **¿Qué es una Dirección IP y para qué sirve en nuestro proyecto?**
   > Una Dirección IP es un número único que identifica a un dispositivo dentro de una red. Funciona como la “dirección” de una computadora o dispositivo para que otros puedan encontrarlo y comunicarse con él.
En nuestro proyecto, la IP sirve para que la computadora se conecte con la ESP32 a través de la red WiFi y puedan enviarse datos entre sí .

2. **¿Qué es un Puerto de red? (Menciona qué puerto estamos usando en el código de la ESP32).**
   > Un Puerto de red es un número que identifica un canal específico de comunicación dentro de un dispositivo conectado a la red. Permite que varios programas usen la red al mismo tiempo sin confundirse.
En nuestro proyecto, la ESP32 abre un puerto para escuchar conexiones desde la computadora. El puerto que usamos en el código es 80

3. **Define con tus propias palabras qué es un Servidor en informática.**
   > Un Servidor es un dispositivo o programa que espera conexiones de otros dispositivos y les proporciona información o servicios a través de una red.
Por ejemplo, puede enviar datos, guardar información o controlar dispositivos cuando lo solicita.

4. **¿Cuál es la diferencia entre un "Servidor" (Hardware/Software) y un "Servicio" (Service)?**
   > *Un Servidor es el sistema (computadora o programa) que recibe solicitudes de otros dispositivos.
Un Servicio es la función o tarea específica que el servidor ofrece.

5. **Investigación: ¿Cuál es la diferencia técnica entre un "Socket TCP" normal y un "WebSocket"?**
   > Un Socket TCP normal es una conexión directa entre dos dispositivos que envían y reciben datos continuamente usando el protocolo TCP. Se usa mucho en programas y aplicaciones personalizadas.

Un WebSocket es un protocolo que funciona sobre HTTP y permite una comunicación bidireccional en tiempo real entre un navegador web y un servidor.

6. **Analizando nuestro código: ¿Quién actúa como Servidor y quién actúa como Cliente? (Justifica tu respuesta mencionando qué funciones del código lo demuestran, ej. `bind()`, `connect()`).**
   > En nuestro proyecto, la ESP32 actúa como servidor porque abre un puerto y espera que alguien se conecte. Esto se demuestra con funciones como bind() y listen(), que preparan el dispositivo para recibir conexiones.

7. **En el código de la computadora (Python), importamos la librería `threading` (Hilos). ¿Qué pasaría con la ventana de Tkinter si no usáramos hilos para recibir los datos de la red?**
   > *Tu respuesta aquí*

8. **¿Por qué es necesario usar bloques `try...except` cuando trabajamos con conexiones de red e Internet?**
   > *Tu respuesta aquí*

9. **En la función de encender el LED en Python, enviamos el comando así: `sock.send(b'ON')`. ¿Qué significa esa letra `b` antes de las comillas y por qué no enviamos un texto normal?**
   > *Tu respuesta aquí*

10. **Describe brevemente el flujo de datos: ¿Qué camino recorre la información desde que giras el potenciómetro físicamente hasta que la barra se mueve en la pantalla de la computadora?**
    > *Tu respuesta aquí*
