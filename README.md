# entregatarea3
Todos los programas solicitados en la tarea 3 QM2515

El primero: Cree un programa para calcular el pH de una solución dada la concentración de
iones H+, los pasos detallando que se hizo son:

En primer lugar, se utiliza la función input() para solicitar al usuario que introduzca la concentración de iones H+. La función float() se utiliza para convertir el valor ingresado por el usuario en un número de punto flotante y se guarda en la variable conc_H.

Luego, se utiliza la función math.log() para calcular el logaritmo en base 10 de conc_H. El resultado no se guarda en ninguna variable, por lo que esta operación no tiene ningún efecto en el programa.

A continuación, se utiliza nuevamente la función math.log() para calcular el logaritmo en base 10 de conc_H y se le asigna a la variable pH. Esto se hace para obtener el valor negativo del logaritmo y así obtener el pH de la solución.

Finalmente, se imprime el valor de pH utilizando la función print().

Este programa sigue el procedimiento estándar para calcular el pH utilizando la fórmula pH = -log[H+], donde [H+] es la concentración de iones H+. Se utilizan las funciones input(), float() y math.log() para realizar los cálculos necesarios.

El segundo; Cree un programa que me permita calcular los moles de cualquier compuesto, los pasos detallando que se hizo son: 

En primer lugar, se utiliza la función input() para solicitar al usuario que ingrese la cantidad del compuesto en gramos o mililitros. El valor ingresado se convierte a un número de punto flotante utilizando float() y se guarda en la variable Gcomp.

Luego, se utiliza la función input() nuevamente para solicitar al usuario que indique si la cantidad ingresada es en gramos o mililitros. La función lower() se utiliza para convertir la respuesta del usuario a minúsculas y así evitar problemas de capitalización. El resultado se guarda en la variable escala.

A continuación, se utiliza una estructura condicional if-elif para determinar qué cálculos realizar en función de si la escala es "g" (gramos) o "ml" (mililitros).

Si la escala es "g", se solicita al usuario que ingrese el peso molecular del compuesto en gramos por mol utilizando la función float(input()). Luego, se calcula el número de moles utilizando la fórmula moles = (Gcomp * (1 / Peso_A)) y el resultado se guarda en la variable moles. Finalmente, se imprime el valor de moles.

Si la escala es "ml", se solicita al usuario que ingrese la densidad del compuesto en gramos por mililitro y el peso molecular del compuesto en gramos por mol. Luego, se calcula el número de moles utilizando la fórmula moles = (Gcomp * Densidad * (1 / Peso_A)) y el resultado se guarda en la variable moles. Finalmente, se imprime el valor de moles.

Este programa permite calcular los moles de un compuesto utilizando las cantidades en gramos o mililitros proporcionadas por el usuario. Se utilizan estructuras condicionales y fórmulas matemáticas básicas para realizar los cálculos necesarios.

El tercero: Cree un programa que me permita calcular la concentración de cualquier compuesto
(moles/litros), los pasos detallando que se hizo son: 

En primer lugar, se utiliza la función input() para solicitar al usuario que ingrese la cantidad del compuesto en gramos o mililitros. El valor ingresado se convierte a un número de punto flotante utilizando float() y se guarda en la variable Gcomp.

Luego, se utiliza la función input() nuevamente para solicitar al usuario que indique si la cantidad ingresada es en gramos o mililitros. La función lower() se utiliza para convertir la respuesta del usuario a minúsculas y así evitar problemas de capitalización. El resultado se guarda en la variable escala.

A continuación, se utiliza una estructura condicional if-elif para determinar qué cálculos realizar en función de si la escala es "g" (gramos) o "ml" (mililitros).

Si la escala es "g", se solicita al usuario que ingrese el peso molecular del compuesto en gramos por mol utilizando la función float(input()). Luego, se calcula el número de moles utilizando la fórmula moles = (Gcomp * (1 / Peso_A)) y el resultado se guarda en la variable moles.

Si la escala es "ml", se solicita al usuario que ingrese la densidad del compuesto en gramos por mililitro y el peso molecular del compuesto en gramos por mol. Luego, se calcula el número de moles utilizando la fórmula moles = (Gcomp * Densidad * (1 / Peso_A)) y el resultado se guarda en la variable moles.

Después, se utiliza la función input() para solicitar al usuario que ingrese el volumen en litros. El valor ingresado se convierte a un número de punto flotante y se guarda en la variable Volumen.

Finalmente, se calcula la molaridad dividiendo la cantidad de moles (Gcomp) entre el volumen (Volumen) y se guarda en la variable Molaridad. Luego, se imprime el valor de Molaridad.

Este programa permite calcular la concentración de un compuesto en moles por litro utilizando las cantidades en gramos o mililitros proporcionadas por el usuario. Se utilizan estructuras condicionales y fórmulas matemáticas básicas para realizar los cálculos necesarios.

El cuarto: Cree un programa que me permita calcular el rendimiento teórico de una reacción a
partir de los rendimientos reales y teóricos, los pasos detallando que se hizo son: 

En primer lugar, se utiliza la función input() para solicitar al usuario que ingrese la masa experimental en gramos. El valor ingresado se convierte a un número de punto flotante utilizando float() y se guarda en la variable Mexperi.

Luego, se utiliza la función input() nuevamente para solicitar al usuario que ingrese la masa teórica en gramos. El valor ingresado se convierte a un número de punto flotante y se guarda en la variable Mteori.

A continuación, se calcula el porcentaje de rendimiento utilizando la fórmula (Mexperi / Mteori) * 100 y el resultado se guarda en la variable Rendimiento.

Finalmente, se imprime el valor de Rendimiento, que representa el porcentaje de rendimiento de la reacción.

Este programa te permite calcular fácilmente el porcentaje de rendimiento de una reacción comparando los rendimientos experimental y teórico.

El Quinto: Determinar el pH de una solución tampón a partir de la concentración de un ácido
débil y su base conjugada, los pasos detallando que se hizo son:

Cacid = float(input("Concentración (mol/L) del Ácido Débil:")) - Se le pide al usuario que ingrese la concentración del ácido débil en moles por litro. El valor ingresado se convierte a un número de punto flotante y se guarda en la variable Cacid.

Cbasc = float(input("Concentración (mol/L) de Base Conjugada:")) - Se le pide al usuario que ingrese la concentración de la base conjugada en moles por litro. El valor ingresado se convierte a un número de punto flotante y se guarda en la variable Cbasc.

pKa = float(input("pKA Ácido Débil: ")) - Se le pide al usuario que ingrese el valor pKa del ácido débil. El valor ingresado se convierte a un número de punto flotante y se guarda en la variable pKa.

import math - Se importa el módulo math, que proporciona funciones matemáticas avanzadas.

math.log(Cacid/Cbasc, 10) - Se calcula el logaritmo en base 10 de la división entre las concentraciones del ácido débil y la base conjugada utilizando la función log() del módulo math. Sin embargo, este cálculo no se guarda en ninguna variable.

pH = - pKa + math.log(Cacid/Cbasc, 10) - Se calcula el pH de la solución tampón utilizando la fórmula pH = -pKa + log(Cacid/Cbasc). El resultado se guarda en la variable pH.

print(pH) - Se imprime el valor de pH, que representa el pH de la solución tampón.

Este programa te permite determinar el pH de una solución tampón a partir de las concentraciones de un ácido débil y su base conjugada, utilizando el valor pKa del ácido débil y la fórmula correspondiente.

El Sexto: Cree un programa prediga si un compuesto será soluble o insoluble (use el kps), los pasos detallando que se hizo son:

Primero, se solicita al usuario que ingrese el valor de Kps, la concentración del Ion 1 en solución y la concentración del Ion 2 en solución. Luego, se calcula el producto de las concentraciones de los iones (Prod_I). Finalmente, se utiliza una estructura condicional (if-else) para comparar el producto con Kps y determinar si el compuesto es soluble o insoluble.

El Septimo: Con base a todo lo anterior cree su propio módulo de Python, yo decidi que fuese hallar los moles a partir de una muestra de ml y sabiendo su concentracion Molar, los pasos detallando que se hizo son:

def calcular_moles_ml(Mlcomp, Molaridad):: Esta línea define la función calcular_moles_ml con dos parámetros: Mlcomp y Molaridad.

print("Los moles ml son:", float(Mlcomp) * (1/1000) * float(Molaridad)): Esta línea realiza el cálculo de los moles usando los valores de Mlcomp y Molaridad. Los valores se convierten en números decimales utilizando la función float(). Luego, se multiplica el valor de Mlcomp por 1/1000 para convertirlo a litros y se multiplica por Molaridad para obtener los moles. El resultado se imprime en la consola junto con un mensaje.

Entonces, al llamar a esta función con valores específicos para Mlcomp y Molaridad, obtendrás el número de moles correspondiente al compuesto.

El Octavo: Cree un programa para calcular el seno y el coseno de un ángulo (No usar el módulo math) – Compare su resultado con el del módulo math (¿dan el mismo resultado?), los pasos detallando que se hizo son:

Primero, se define una función llamada calcular_seno(angulo) que toma como argumento el ángulo en grados. Dentro de esta función, se convierte el ángulo a radianes multiplicándolo por (3.14159 / 180), que es la conversión estándar de grados a radianes.

A continuación, se inicializan las variables resultado y termino a 0 y n a 1.

Luego, se utiliza un bucle while para calcular los términos de la serie de Taylor del seno hasta que el valor absoluto del término sea menor que 0.000001. En cada iteración del bucle, se suma el valor del término al resultado y se actualiza el valor del término multiplicándolo por -1 * (radianes ** 2) / ((2 * n) * (2 * n + 1)), donde ** representa la operación de exponente. Además, se incrementa el valor de n en 1 en cada iteración.

Finalmente, se retorna el resultado del cálculo del seno.

La función calcular_coseno(angulo) sigue un proceso similar al calcular el coseno en lugar del seno.

Después de definir las funciones, se solicita al usuario ingresar un ángulo en grados utilizando la función float(input("Ingrese el ángulo en grados: "))

Luego, se llama a las funciones calcular_seno(angulo) y calcular_coseno(angulo) para obtener los valores del seno y el coseno del ángulo ingresado.

Por último, se imprime en pantalla el resultado utilizando la función print.

En resumen, este código utiliza la serie de Taylor para calcular el seno y el coseno de un ángulo dado utilizando un bucle while y fórmulas matemáticas específicas para cada función trigonométrica.

Y si, si dan el mismo resultado que con el modulo math

El Noveno: Ahora cree un programa que le permita decir cuando el seno y el coseno de un ángulo sean iguales, los pasos detallando que se hizo son:

El código comienza definiendo una función llamada verificar_igualdad_seno_coseno que toma un parámetro angulo. Dentro de esta función, se convierte el ángulo de grados a radianes utilizando la función math.radians(). Los cálculos de seno y coseno se realizan utilizando las funciones math.sin() y math.cos() respectivamente, y se almacenan en las variables seno y coseno.

Luego, se compara si el valor redondeado del seno hasta 6 decimales es igual al valor redondeado del coseno hasta 6 decimales utilizando la función round(). Si la condición es verdadera, es decir, si el seno y el coseno son iguales, la función devuelve True. De lo contrario, devuelve False.

Después de definir la función, se solicita al usuario ingresar un ángulo en grados utilizando la función input() y se guarda en la variable angulo después de convertirlo a un número de punto flotante utilizando la función float().

A continuación, se llama a la función verificar_igualdad_seno_coseno() pasando el valor del ángulo como argumento. Si la función devuelve True, se imprime un mensaje indicando que el seno y el coseno del ángulo son iguales. Si devuelve False, se imprime un mensaje indicando que no son iguales.

En resumen, este código verifica si el seno y el coseno de un ángulo son iguales al convertir el ángulo a radianes y luego comparar los valores redondeados del seno y el coseno hasta 6 decimales.
