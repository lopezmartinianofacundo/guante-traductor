# Proyecto de reconocimiento de Lengua de Señas Argentina (LSA)

## Descripción

Este proyecto busca desarrollar un sistema capaz de reconocer letras y señas de la Lengua de Señas Argentina (LSA) mediante sensores de flexión (Flex Sensors) y un sensor MPU6050 (acelerómetro y giroscopio) para determinar la orientación y el movimiento de la mano.

El sistema analiza la posición de los dedos y la orientación de la mano para identificar la seña realizada y mostrar la letra correspondiente.

El proyecto utiliza sensores flex para determinar la posición de los dedos y un MPU6050 para obtener información sobre la orientación de la mano, permitiendo identificar diferentes letras y señas de la LSA.

Actualmente el proyecto se encuentra en fase de desarrollo y validación del prototipo utilizando potenciómetros para simular los sensores flex antes de implementar el hardware definitivo.

El circuito electrónico y el diseño de la PCB fueron desarrollados en KiCad.

## Objetivo del proyecto

El objetivo principal del proyecto es aprender sobre la Lengua de Señas Argentina (LSA) y explorar distintas técnicas para el reconocimiento de señas mediante sensores y sistemas electrónicos.

A través de este desarrollo se busca adquirir experiencia en programación de microcontroladores, procesamiento de datos provenientes de sensores, diseño de circuitos electrónicos y diseño de PCB.


## Componentes principales

### Microcontrolador

* ESP32-S2

### Sensores

* MPU6050 (Acelerómetro y Giroscopio)
* 5 Sensores Flex (versión final)
* 5 Potenciómetros (prototipo y simulación)

## Funcionamiento

Cada dedo dispone de un sensor encargado de medir su nivel de flexión.

El MPU6050 proporciona información sobre la orientación de la mano mediante los ángulos de inclinación Pitch y Roll.

El microcontrolador procesa estos datos y los compara con patrones previamente definidos para determinar qué letra o seña se está realizando.

## Estado actual del proyecto

Actualmente se está trabajando en:

* Lectura de los sensores simulados mediante potenciómetros.
* Lectura del MPU6050.
* Cálculo de Pitch y Roll.
* Desarrollo inicial del algoritmo de reconocimiento de letras.
* Diseño del circuito electrónico.
* Diseño de PCB en KiCad.
* Pruebas en simulación mediante Wokwi.

## Mejoras futuras

* Incorporación de sensores flex reales.
* Reconocimiento de una mayor cantidad de letras y señas.
* Mejora de la precisión del reconocimiento.
* Implementación de métodos de calibración.
* Evaluación de nuevas técnicas para el reconocimiento de señas.

## Tecnologías utilizadas

* ESP32-S2
* Arduino IDE
* MPU6050
* KiCad
* Wokwi
* GitHub
