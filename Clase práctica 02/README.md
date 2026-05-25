# Clase Práctica 2 - Introducción a Variables y Secuencias con LEDs

Este directorio contiene la segunda práctica del curso de **ArduinoUno**. Se introducen las variables para almacenar pines y tiempos, y se programan diferentes secuencias de encendido y apagado de LEDs, incluyendo efectos de acumulación, semáforos y control de un LED RGB.

## Contenido de la carpeta

La carpeta `clase practica 2` incluye cuatro archivos, cada uno con una variante del uso de variables y estructuras de control para manejar múltiples LEDs.

- **`Práctica #02 - P1 _ prendido y apagado de leds ordenados - Declaración de Variables.md`**  
  Enciende y apaga tres LEDs (rojo, amarillo, verde) de forma secuencial individual. Cada LED permanece encendido 300 ms y apagado 300 ms antes de pasar al siguiente. Se utiliza la declaración de variables (`const int` e `int`) para asignar los pines. Incluye preguntas teóricas sobre constantes y retardos, y ejercicios como invertir el orden, añadir un cuarto LED o usar bucles `for`.

- **`Práctica #02 - P2 _ Encendido y apagado de leds - Declaración de Variables.md`**  
  Enciende los LEDs de forma acumulativa (verde → verde+amarillo → verde+amarillo+rojo) y luego los apaga de forma decremental (rojo → amarillo → verde). Cada paso dura 1 segundo. Introduce variables para los tiempos (`espera1s`, `espera2s`). Las preguntas abordan la simetría de la secuencia, ventajas de usar variables y cálculos de duración. Los ejercicios incluyen cambiar el orden, asimetría en los retardos, añadir un cuarto LED, eliminar el último delay y reemplazar por bucles.

- **`Práctica #02 - P3 _ Semáforo - Declaración de Variables.md`**  
  Simula un semáforo estándar: verde 2 s, amarillo 1 s, rojo 2 s. Utiliza variables para pines y tiempos. Explica la secuencia típica y la posibilidad de añadir una luz peatonal. Las preguntas teóricas tratan sobre el orden de las fases, tiempos reales de semáforo y la utilidad de las variables. Los ejercicios proponen intercambiar tiempos, añadir un LED peatonal, hacer parpadear el amarillo antes del verde, sincronizar dos semáforos opuestos y reestructurar con máquina de estados (switch-case).

- **`Práctica #02 - P4 _ led RGB- Declaración de Variables.md`**  
  Controla un LED RGB de cátodo común para mostrar siete colores (azul, verde, cian, rojo, magenta, amarillo, blanco), cada uno durante 1 segundo. Explica la diferencia entre cátodo común y ánodo común, y la necesidad de resistencias individuales. Las preguntas abordan la lógica de encendido, generación de colores secundarios y el uso de PWM. Los ejercicios incluyen cambiar el orden de los colores, añadir un LED blanco extra, usar `analogWrite` para intensidades, reducir el tiempo de espera para efecto de persistencia visual e invertir la lógica para ánodo común.

## Propósito de la práctica

Aprender a:
- Declarar variables y constantes para pines y retardos.
- Realizar secuencias temporales con `delay()`.
- Controlar múltiples LEDs de forma individual, acumulativa o alternada.
- Simular comportamientos reales como semáforos.
- Generar colores mediante un LED RGB combinando salidas digitales.
- Modificar y optimizar el código usando bucles y arrays.

## Cómo usar estos archivos

1. Lee cada archivo en orden (P1, P2, P3, P4) para seguir una progresión lógica.
2. Responde las preguntas teóricas por escrito.
3. Realiza los ejercicios prácticos modificando el código en el simulador de Tinkercad (enlace incluido en cada archivo) o en un Arduino real.
4. Anota las observaciones y cambios en el comportamiento de los LEDs.

## Requisitos

- Arduino Uno (o compatible) o acceso a Tinkercad.
- LEDs individuales (rojo, amarillo, verde, azul) y resistencias de 220 Ω.
- Un LED RGB (de cátodo o ánodo común) y tres resistencias de 220 Ω.
- Cables y protoboard.
