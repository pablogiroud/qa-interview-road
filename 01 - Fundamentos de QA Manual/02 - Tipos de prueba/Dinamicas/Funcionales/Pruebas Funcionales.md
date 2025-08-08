# Pruebas Funcionales

La prueba funcional es un tipo de prueba de software que verifica que cada función de una aplicación se comporte de acuerdo con los requisitos especificados y cumpla con las expectativas del usuario. Se centra en probar la funcionalidad del sistema desde la perspectiva del usuario, asegurando que las entradas correctas produzcan las salidas esperadas.

En resumen, las pruebas funcionales aseguran que el software haga lo que debe hacer según lo definido en los requisitos.

---

## ¿Qué se prueba?

Las pruebas funcionales evalúan las características y funcionalidades específicas de una aplicación, como la entrada de datos, la navegación, la generación de informes y la lógica del negocio.

**Enfoque principal:**  
Generalmente, las pruebas funcionales utilizan un enfoque de **caja negra**, donde el tester no necesita conocer la estructura interna del sistema, solo su comportamiento externo. Se suministran entradas y se observa la salida, comparándola con lo esperado.

---

## Técnicas funcionales

Las técnicas funcionales ayudan a diseñar casos de prueba efectivos para validar el comportamiento del software. Las principales son:

### 1. Caja Negra

- **Descripción:** El tester no conoce la estructura interna del sistema. Se enfoca en las entradas y salidas.
- **Ejemplos de técnicas:**
  - Partición de equivalencia
  - Análisis de valores límite
  - Tablas de decisión
  - Transición de estados
  - Pruebas de casos de uso

### 2. Caja Blanca

- **Descripción:** El tester tiene acceso al código fuente y diseña pruebas basadas en la lógica interna y los caminos del programa.
- **Ejemplos de técnicas:**
  - Cobertura de sentencias
  - Cobertura de decisiones/ramas
  - Cobertura de condiciones
  - Caminos independientes

### 3. Caja Gris

- **Descripción:** Combinación de caja negra y caja blanca. El tester tiene acceso parcial al diseño o código, lo que permite diseñar pruebas más efectivas.
- **Ejemplo de uso:** Pruebas de integración donde se conoce la arquitectura, pero se prueban funcionalidades desde la perspectiva del usuario.

---

## Tipos de pruebas funcionales

Las pruebas funcionales pueden clasificarse en varios tipos según el objetivo y el nivel de prueba:

- **Pruebas unitarias:** Verifican el funcionamiento correcto de las unidades más pequeñas del código (funciones, métodos, clases).
- **Pruebas de integración:** Evalúan la interacción entre diferentes módulos o componentes del sistema.
- **Pruebas de sistema:** Validan el comportamiento del sistema completo, asegurando que todos los componentes funcionen juntos correctamente.
- **Pruebas de aceptación:** Confirman que el sistema cumple con los requisitos y expectativas del usuario final.
- **Pruebas de humo:** Pruebas básicas para verificar que las funciones principales del sistema operan correctamente tras un cambio.
- **Pruebas de regresión:** Aseguran que nuevas modificaciones no hayan afectado funcionalidades existentes.
- **Pruebas exploratorias:** El tester explora la aplicación para identificar defectos no cubiertos por casos de prueba formales.

> **Nota:** Las técnicas de caja negra, caja blanca y caja gris pueden aplicarse en diferentes tipos de pruebas funcionales según el contexto y el objetivo de la prueba.

---

## Importancia

Las pruebas funcionales son cruciales para asegurar la calidad del software, ya que ayudan a identificar errores y problemas de funcionalidad antes de que el software sea lanzado al usuario final.

---

## Herramientas

Existen diversas herramientas para automatizar pruebas funcionales, como:
- Selenium
- UFT
- Katalon Studio
- TestComplete

---