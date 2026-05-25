# Clase Práctica 1 - Parpadeo de un LED

Este directorio contiene la primera práctica del curso de **ArduinoUno**. En ella se introduce el clásico programa "Blink" (parpadeo de un LED), que constituye el equivalente al "Hola mundo" en la programación de hardware.

## Contenido de la carpeta

- **`Práctica #01 Parpadeo de un LED.md`** : Archivo principal de la práctica. Incluye:
  - Explicación detallada del código (`setup()`, `loop()`, `digitalWrite()`, `delay()`).
  - Consideraciones sobre el uso de resistencias y efectos de variar los tiempos de espera.
  - Código completo para copiar y pegar.
  - Enlace a un simulador en Tinkercad.
  - **Preguntas teóricas** (5 preguntas sobre voltajes, configuración de pines, LED interno, frecuencia y limitaciones de `delay()`).
  - **Ejercicios prácticos** (5 ejercicios para modificar el código y analizar cambios en el comportamiento del LED).

## ¿De qué trata esta práctica?

Se conecta un LED (con su resistencia de 220 Ω) al pin digital 12 de una placa Arduino. El programa enciende el LED durante 300 ms, lo apaga durante otros 300 ms y repite el ciclo indefinidamente. El objetivo es verificar que la placa, el compilador y el montaje funcionan correctamente, además de comprender los conceptos básicos de salidas digitales y temporizaciones.

## Cómo utilizar este material

1. Lee el archivo `Práctica #01 Parpadeo de un LED.md` para entender el código y los fundamentos.
2. Responde las preguntas teóricas por escrito.
3. Realiza cada uno de los ejercicios prácticos modificando el código, ya sea en un Arduino real o en el simulador de Tinkercad (enlace incluido en el archivo).
4. Anota tus observaciones y cambios en el comportamiento del LED.

## Requisitos

- Conocimientos básicos de electrónica (LED, resistencia, protoboard).
- Entorno de desarrollo Arduino IDE o acceso a Tinkercad.
- Placa Arduino Uno (o compatible) y los componentes indicados en la práctica.
