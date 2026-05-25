# Clase Práctica 3 - Control de Voltaje, Pulsadores y Estructuras de Control

Este directorio contiene la tercera práctica del curso de **ArduinoUno**. Se introducen las entradas analógicas (potenciómetro), las salidas PWM, la lectura de pulsadores y las estructuras condicionales (`if`) y bucles (`while`) para controlar el flujo del programa.

## Contenido de la carpeta

La carpeta `clase practica 3` incluye cuatro archivos, cada uno aborda un concepto diferente de control y temporización.

- **`Práctica #03 - P1 _ Control de Distribución de voltaje - Declaración de Variables.md`**  
  Lee un potenciómetro conectado a A0 y controla dos LEDs (verde en pin 5, rojo en pin 3) de forma complementaria: cuando el potenciómetro aumenta, el verde aumenta su brillo y el rojo disminuye. Utiliza `analogRead()` (0‑1023) y `analogWrite()` (0‑255) con escalado. Explica PWM, resistencias de 220 Ω y distribución inversa de voltaje. Incluye preguntas sobre rangos, pines no‑PWM y comportamiento en posición media. Los ejercicios proponen cambiar las fórmulas de escalado, intercambiar LEDs, añadir un tercer LED con el promedio y usar otros pines PWM.

- **`Práctica #03 - P2 _ LED con Pulsador - IF.md`**  
  Ejecuta una secuencia de encendido/apagado de tres LEDs (verde, amarillo, rojo) solo cuando se presiona un pulsador. Introduce la lectura digital (`digitalRead`), la configuración de un pin como `INPUT` y la estructura condicional `if`. Los LEDs se encienden en orden (verde → amarillo → rojo) y se apagan en orden inverso, con retardos de 500 ms. Las preguntas abordan la necesidad de resistencias pull‑down, el propósito de `if` y qué ocurre si se omite `pinMode`. Los ejercicios incluyen invertir la secuencia, añadir un cuarto LED, cambiar la lógica del pulsador (que ejecute cuando NO está presionado), eliminar el apagado o añadir un delay final.

- **`Práctica #03 - P3 LED con Pulsador - IF.md`**  
  Implementa un interruptor tipo “toggle” (cambia de estado cada vez que se presiona) usando un pulsador y un LED. Introduce variables de tipo `bool` y la inversión lógica (`estado = !estado`). Explica el problema del rebote (bouncing) y comenta una posible solución con `delay(50)`. Las preguntas teóricas cubren el funcionamiento de `bool`, el operador `!`, el rebote y la configuración de pines. Los ejercicios: agregar antirrebote con distintos delays, hacer que el LED parpadee 3 veces al presionar, usar resistencia pull‑up interna (`INPUT_PULLUP`), añadir un segundo LED invertido y reemplazar el LED por un servomotor.

- **`Práctica #03 - P4 _ LED con Pulsador - While.md`**  
  Otra versión del interruptor toggle, pero utilizando bucles `while` para esperar activamente a que el pulsador sea presionado y luego soltado. El código lee el estado actual del LED con `digitalRead` (válido incluso en pines de salida) y escribe el valor opuesto. Incluye `Serial.begin(9600)` (aunque no se use, se deja para depuración). Las preguntas comparan `if` vs `while`, explican la necesidad de dos bucles, el efecto del rebote y la validez de leer un pin de salida. Los ejercicios: añadir pequeños delays para antirrebote, eliminar el segundo `while` (produce múltiples cambios), controlar dos LEDs intercambiando estados, reemplazar los `while` por un `if` con flanco, y usar un LED RGB que recorra una secuencia de colores con cada pulsación.

## Propósito de la práctica

Aprender a:
- Leer señales analógicas (potenciómetro) y convertirlas a PWM para controlar brillo de LEDs.
- Usar estructuras condicionales (`if`) y bucles (`while`) para responder a entradas digitales (pulsadores).
- Diferenciar entre ejecución secuencial bloqueante (`delay`, bucles vacíos) y detección de flancos.
- Implementar interruptores tipo toggle y secuencias condicionadas.
- Conectar correctamente pulsadores con resistencias pull‑down o pull‑up.

## Cómo usar estos archivos

1. Lee los archivos en orden (P1 a P4) para progresar desde analógico/PWM hasta pulsadores y estructuras de control.
2. Responde las preguntas teóricas por escrito.
3. Realiza los ejercicios prácticos modificando el código en el simulador de Tinkercad (enlace incluido en cada archivo) o en un Arduino real.
4. Anota las observaciones y cambios en el comportamiento del circuito.

## Requisitos

- Arduino Uno (o compatible) o acceso a Tinkercad.
- Potenciómetro (10 kΩ).
- LEDs (rojo, verde, amarillo, azul, RGB) y resistencias de 220 Ω.
- Pulsadores y resistencias de 10 kΩ (para pull‑down).
- Cables y protoboard.
