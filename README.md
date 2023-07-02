# Practica 2 - PdM

**Tabla de contenidos**

[TOCM]

[TOC]
- 
## Objetivo:
Implementar un módulo de software para trabajar con retardos no bloqueantes. 

### Consigna:
Implementar un programa que utilice retardos no bloqueantes y  haga titilar en forma periódica e independiente los tres leds de la placa NUCLEO-F429ZI de la siguiente manera:
- LED1: 100 ms. 
- LED2: 500 ms.
- LED3: 1000 ms.

### Funciones implementadas:
	void delayInit( delay_t * delay, tick_t duration );
	bool_t delayRead( delay_t * delay );
	void delayWrite( delay_t * delay, tick_t duration );

### Variables implementadas:
	typedef uint32_t tick_t; // Qué biblioteca se debe incluir para que esto compile?
	typedef bool bool_t;	  // Qué biblioteca se debe incluir para que esto compile?
	typedef struct{
	   tick_t startTime;
	   tick_t duration;
	   bool_t running;
	} delay_t;
