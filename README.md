# Apx School - Piedra Papel ó Tijera solución

Esta es una solucion a este desafio PPT-Off

## Índice

- Resumen
  - [Desafio](#desafio)
  - [Captura de pantalla](#captura-de-pantalla)
  - [Enlaces](#https://preeminent-squirrel-24c83e.netlify.app)
  - [Mi proceso](#miproceso)
  - [Construido con](#JavaScript-HTML-CSS-TypeScript)
  - [Lo que aprendí](#Uso-de-TypeScript-LocalStorage-Manejo-de-eventos-Manejo-de-Estados)
  - [Desarrollo continuo](#Juego-Off-Line)
  - [Recursos útiles](#Vite-Project)
  - [Autor](#Cristian-Minni)
  - [Agradecimientos](#Agradezco-a-mi-amigo-Sergio-Luis)


## Overview

### El reto

Los usuarios deben poder:

- Elegir entre tres variables
- Una vez elegido toca elegir PC de forma tal que es random
- Si el Usuario gana se le otorga un punto y si pierde se le suma a la PC
- Diseño óptimo de la interfaz en función del tamaño de la pantalla de su dispositivo.
- La pagína debe realizar los cambios de estados.

### Captura de pantalla

![](C:\Users\usuario\OneDrive\Escritorio)



## Mi proceso


### Construido con

- HTML5 semántico
- Propiedades CSS personalizadas
- TypeScript
- Vanilla JavaScript
- Node

### Lo que aprendí

En este desafio se fortalecion el uso de estados y metodos en JavaScript ademas se trabajo en equipo junto a colaboradores realizando asi un optimo desempeño para resolver.

```html
<h1>Piedra Papel ó Tijeras</h1>
```
```css
:root {
  font-family: "Odibee Sans", sans-serif;
  font-weight: 400;
  font-size: 40px;
  font-style: normal;

  color: #333333;
  background-color: ghostwhite;

  font-synthesis: none;
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
```
``js
setState(stateData: StateData): void {
    if (supportStorage()) {
      localStorage.setItem("PPT-OFF", JSON.stringify(stateData));
    } else {
      this.data = stateData;
    }
    this.listeners.forEach((callback: Function): void => {
      callback(this.data);
    });
  },
```
