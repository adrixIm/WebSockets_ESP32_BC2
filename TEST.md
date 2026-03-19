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
   > Si no se usaran hilos, la ventana de Tkinter se bloquearía o se congelaría mientras el programa espera recibir datos de la red. Esto haría que la interfaz deje de responder (no se podría hacer clic ni cerrar la ventana), ya que todo el proceso estaría ocupando el mismo flujo de ejecución.

8. **¿Por qué es necesario usar bloques `try...except` cuando trabajamos con conexiones de red e Internet?**
   > Es necesario usar bloques try...except porque las conexiones de red pueden fallar en cualquier momento (por ejemplo, pérdida de conexión, errores del servidor o datos incorrectos). Estos bloques permiten manejar los errores sin que el programa se cierre inesperadamente, mostrando mensajes adecuados y manteniendo la aplicación funcionando correctamente.

9. **En la función de encender el LED en Python, enviamos el comando así: `sock.send(b'ON')`. ¿Qué significa esa letra `b` antes de las comillas y por qué no enviamos un texto normal?**
   > La letra b antes de las comillas indica que el mensaje está en formato de bytes. Esto es necesario porque las conexiones de red (sockets) solo pueden enviar y recibir datos en forma de bytes, no como texto normal (strings). Por eso no se envía un texto común, sino su representación en bytes para que pueda ser interpretado correctamente por el dispositivo receptor.

10. **Describe brevemente el flujo de datos: ¿Qué camino recorre la información desde que giras el potenciómetro físicamente hasta que
11. la barra se mueve en la pantalla de la computadora?**
  > Cuando giras el potenciómetro, este cambia su resistencia y genera una variación en el voltaje. Ese valor es leído por el microcontrolador (por ejemplo, Arduino), que lo convierte en un dato digital. Luego, ese dato se envía a través de la red (usando sockets) hacia la computadora. En la computadora, el programa en Python recibe la información, la procesa y actualiza la interfaz gráfica de Tkinter, haciendo que la barra se mueva según el valor recibido.









    > *Tu respuesta aquí*
