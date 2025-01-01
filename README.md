# Curso de Bash Script para Principiantes

Este repositorio contiene ejemplos y ejercicios prácticos del curso de Bash Script para principiantes del canal Fazt. 

**¿Qué es Bash?**

Bash es un intérprete de comandos de línea utilizado para interactuar con sistemas operativos similares a Unix, como Linux y macOS. Los scripts de Bash son programas escritos en el lenguaje Bash que automatizan tareas.

**¿Por qué aprender Bash?**

* **Automatización de tareas:** Simplifica tareas repetitivas, como la administración de archivos, la gestión de servidores y la generación de informes.
* **Control del sistema:** Permite interactuar directamente con el sistema operativo, lo que es esencial para administradores de sistemas y desarrolladores.
* **Mejora la productividad:** Aumenta la eficiencia al automatizar tareas y reducir el tiempo dedicado a tareas manuales.

**Conceptos básicos:**

* **Variables:** Almacenan valores que pueden ser utilizados en el script.
  
  ```bash
  nombre="Juan"
  edad=30
  echo "Hola, mi nombre es $nombre y tengo $edad años."

* **Comentarios:** Se utilizan para documentar el código y mejorar su legibilidad.

  ```bash
  : '
  Este es un comentario
  que abarca varias líneas
  '
  #Este es un comentario de una sola linea
  
* **Operadores:** Se utilizan para realizar operaciones matemáticas, lógicas y de comparación.

  ```bash
  numero1=10
  numero2=5
  resultado=$((numero1 + numero2))
  echo "La suma es: $resultado"
  
* **Estructuras de control:** 
    * **Condicionales (if-else, elif):** Permiten ejecutar diferentes bloques de código según se cumplan o no ciertas condiciones.

      ```bash
      if [ $numero1 -gt $numero2 ]; then
        echo "$numero1 es mayor que $numero2"
      else
        echo "$numero2 es mayor o igual que $numero1"
      fi
      
    * **Bucles (for, while):** Permiten repetir un bloque de código varias veces.
 
      ```bash
      for i in {1..5}; do
        echo "Iteración $i"
      done
      
* **Manejo de archivos:** 
    * **Leer archivos:** Obtener el contenido de un archivo.

      ```bash
      contenido=$(cat archivo.txt)
      echo "$contenido"
    
    * **Escribir archivos:** Crear o modificar archivos.

      ```bash
      echo "Hola, mundo" > nuevo_archivo.txt  
      
    * **Agregar contenido a archivos:** Añadir información a un archivo existente.
    
      ```bash
      echo "Nueva línea" >> archivo.txt
      
**Ejemplo: Hola Mundo**

```bash
#!/bin/bash

echo "Hola Mundo"
