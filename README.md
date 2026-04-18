# SISTEMA-DE-CALIFICACIONES-DE-ESTUDIANTES

en el sistema de calificación de estudiante usaré de ejemplo a cuatro estudiantes Luis Luna sol y Luca la cual mostraré el mínimo de cada uno quién aprobaron y quién no aprobaron basándome en cuatro calificaciones que depende de cada quien

# Ejemplo del sistema en funcionamiento 

![image alt](https://github.com/vdalvin71-netizen/SISTEMA-DE-CALIFICACIONES-DE-ESTUDIANTES/blob/8e8f02cfb8c234c907b3751cb218452fd2758a2f/WhatsApp%20Image%202026-04-18%20at%207.46.20%20AM.jpeg2.jpeg)


![image alt](https://github.com/vdalvin71-netizen/SISTEMA-DE-CALIFICACIONES-DE-ESTUDIANTES/blob/447ac37392a3cedc5ade11d71d6dadcd97bd7ff2/WhatsApp%20Image%202026-04-18%20at%207.46.19%20AM.jpeg)


# Esplicacion mas profunda

​1. Preparación y Variables
​Primero, definimos los "contenedores" donde guardaremos la información. Como el ejercicio pide un máximo de 20 estudiantes, creamos:
​Un arreglo de strings para los nombres: nombres[20].
​Un arreglo de números decimales para los promedios: promedios[20].
​Variables para las estadísticas (suma total, nota más alta, nota más baja, y los contadores de aprobados/reprobados).
​2. El Ciclo Principal (Captura de Datos)
​Usamos un ciclo for que se repite según la cantidad de estudiantes que hayas indicado. Dentro de este ciclo sucede lo siguiente:
​Lectura del Nombre: Se pide el nombre y se guarda en su posición correspondiente del arreglo.Usamos getline para que, si escribes un nombre y un apellido, el programa no se confunda con el espacio.
​Segundo Ciclo (Las 4 Notas): Dentro de cada estudiante, hay otro ciclo for que corre 4 veces. Aquí es donde ocurre la validación: usamos un do-while que "obliga" al usuario a ingresar un número entre 0 y 100. Si pones un 105, el programa te dará error y te pedirá la nota otra vez.
​Búsqueda de Máximos y Mínimos: Cada vez que ingresas una nota, el programa la compara con la notaMasAlta y notaMasBaja que tenemos guardadas para actualizarlas si es necesario.
​3. Cálculos por Estudiante
​Una vez que se terminan de pedir las 4 notas de un alumno:
​Se calcula su promedio individual (suma de sus notas / 4).
​Ese promedio se guarda en el arreglo promedios[i].
​Se suma ese promedio a una variable global para luego sacar el promedio de todo el curso.
​Se verifica si el promedio es mayor o igual a 70 para sumarlo a la cuenta de "Aprobados" o "Reprobados".
​4. Mostrar Resultados
​Al final, el programa recorre el arreglo de nombres y el de promedios simultáneamente para mostrarte la lista limpia. Luego imprime las estadísticas finales que fue acumulando durante todo el proceso.
