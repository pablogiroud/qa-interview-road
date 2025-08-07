# Clases de equivalencias

## Resumen:

Las clases de equivalencia en testing son una técnica de pruebas de software que divide los datos de entrada en grupos o categorías, llamados clases de equivalencia, donde se espera que el sistema los trate de manera similar. En lugar de probar cada valor de entrada individualmente, se selecciona un representante de cada clase para las pruebas, reduciendo así el número de casos de prueba necesarios. 
¿Cómo funciona?

1. Identificar las condiciones de entrada:
Se determinan las restricciones o reglas que afectan a los datos de entrada del sistema. 
2. Definir las clases de equivalencia:
Se agrupan los valores de entrada en clases donde se espera que el sistema se comporte de la misma manera. Estas clases pueden ser:
Válidas: Valores que el sistema debe manejar correctamente. 
Inválidas: Valores que deben ser rechazados o generar un mensaje de error. 
3. Seleccionar casos de prueba:
Se elige un valor representativo de cada clase de equivalencia para crear los casos de prueba. 
Ejemplo:Imagina una función que acepta edades entre 18 y 65. Las clases de equivalencia podrían ser: 
    1. Válida: Edades entre 18 y 65 (ej: 25, 40, 60).
    2. Inválida: Edades menores a 18 (ej: 10).
    3. Inválida: Edades mayores a 65 (ej: 70).
    - En este caso, en lugar de probar con 100 edades diferentes, se probarían 3 (una por cada clase).
  
4. Ventajas y desventajas:
    1. Ventajas:
Reduce el número de casos de prueba: Permite probar un rango amplio de valores con menos casos. 
Aumenta la eficiencia de las pruebas: Permite centrarse en los casos más representativos. 
Mejora la cobertura de las pruebas: Asegura que se prueben diferentes tipos de datos de entrada. 
    2. Desventajas:
Requiere experiencia: Definir las clases de equivalencia requiere un buen entendimiento del sistema.
Puede no detectar errores en los límites: Es posible que no se detecten problemas en los bordes de las clases. 
5. En resumen: Las clases de equivalencia son una técnica de pruebas eficiente para reducir el esfuerzo de prueba, manteniendo una buena cobertura del sistema, especialmente en áreas con rangos de entrada amplios. 


## Extendido:

Testing gird: https://testgrid.io/blog/equivalence-partitioning-testing/#:~:text=El%20Particionamiento%20de%20Equivalencia%20o,una%20cobertura%20de%20prueba%20adecuada.