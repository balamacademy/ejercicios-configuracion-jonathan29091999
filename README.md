# Ejercicios Iniciales C++

Resuelve los siguientes ejercicios para familiarizarte con C++.

Puedes usar el siguiente código como plantilla para los ejercicios.
```cpp
#include <iostream>

int main(int argc, char **argv) {
    std::cout << "Hola, mundo!\n";
    return 0;
}
```

Recuerda compilar y ejecutar con la siguiente secuencia de comandos.

> Linux/MacOs
> ```bash
> g++ miprograma.cpp -o miprograma.o
> ```

> Windows
> ```bash
> g++ miprograma.cpp -o miprograma.exe
> ```

También puedes ejecutar el programa de python **evaluar.py**, el cual, junto con el archivo **conf_eval.json** probará tus programas para saber si estan correctos. 

```bash
python evaluar.py
```

:warning: Cada ejercicio cuenta con un ejemplo, con la entrada y la salida esperada. Las palabras "Entrada:" y "Salida:" no deben imprimirse en la consola. Revisa bien que la salida sea escriba exactamente con el formato que el texto de ejemplo muestra, si no el programa evaluador lo marcará como fallido.

- :heavy_check_mark: Ejemplo:
     ```
     Entrada: 22
     Salida: Categoría: Adulto
     ```
- ✖️: Ejemplo:
    ```
    Entrada: Ingrese su edad: 22
    Salida: Categoría: Adulto
    ```
En ningún programa se requiere que imprima un mensaje para solicitar los valores de entrada. 

## **Ejemplo:** única entrada

1. **Dime tu edad:**
   - Descripción: Ingresa tu edad y muestrala en pantalla.
   - Nombre de archivo: `edad.cpp`
   - Ejemplo:
     
    ```
     Entrada: 22
     Salida: Tu edad es: 22.
    ```
    **Solución:**

    ```cpp
    #include <iostream>

    int main(int argc, char **argv) {
        int edad;
        std::cin >> edad;
        std::cout << "Tu edad es: "<< edad << ".";
        return 0;
    }
    ```

## **Ejemplo:** multiples entradas

1. **Fecha de nacimiento:**
   - Descripción: Ingresa tu edad y el año actual muetrala el año de nacimiento.
   - Nombre de archivo: `nacimiento.cpp`
   - Ejemplo:
     
    ```
     Entrada: 22, 2023
     Salida: Naciste en el 2001.
    ```
    **Solución:**

    ```cpp
    #include <iostream>

    int main(int argc, char **argv) {
        int edad;
        int anio_actual;
        std::cin >> edad;
        std::cin >> anio_actual;
        std::cout << "Naciste en el "<< (anio_actual-edad) << ".";
        return 0;
    }
    ```

> :warning: **Únicamente sube al repositorio los archivos fuente solicitados, aquellos que terminan en ".cpp".** 

> :warning: **No los coloques dentro de carpetas.**

> :warning: **Respeta los nombre de archivo.**


# Ejercicios hechos en clase
1. **Hola Mundo**
   - Descripción: Imprime en pantalla la frase "Hola Mundo!"
   - Nombre de archivo: `holamundo.cpp`
   - Ejemplo:
     ```
     Entrada: NO HAY
     Salida: Hola Mundo!
     ```

1. **Imprimir valores**
   - Descripción: Crea las varibles nombre y edad, a nombre asigna el valor "Juan" y a edad el valor 34, imprimelos en esta frase "El nombre es Juan de edad 34"
   - Nombre de archivo: `imprimirvalores.cpp`
   - Ejemplo:
     ```
     Entrada: 
     Salida: El nombre es Juan de edad 34
     ```

1. **Ingresar valores**
   - Descripción: Solicita el nombre y edad de una persona y imprime el mensaje "El nombre es NOMBRE_INGRESADO de edad EDAD_INGRESADA"
   - Nombre de archivo: `ingresarvalores.cpp`
   - Ejemplo:
     ```
     Entrada: Juan, 34
     Salida: El nombre es Juan de edad 34
     ```
