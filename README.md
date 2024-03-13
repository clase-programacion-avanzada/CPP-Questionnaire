# Preguntas teóricas de C++ 

A continuación encontrará una compilación de preguntas teóricas para prepararse para el exámen. Junto a una breve explicación de la respuesta correcta: 

1. **Una estructura de datos es un arreglo, en donde cada uno de los campos de la estructura tiene un índice que lo identifica.**
    - [ ] Falso
    - [ ] Verdadero
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **Verdadero**.
    </details>

2. **Un apuntador es una variable que solamente puede contener una dirección de memoria.**
    - [ ] Falso
    - [ ] Verdadero
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **Verdadero**.
    </details>

3. **Hay dos formas de enviar parámetros a una función, que se conocen como paso de parámetros por valor y paso de parámetros por referencia.**
    - [ ] Falso
    - [ ] Verdadero
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **Verdadero**.
    </details>

4. **Un arreglo es un apuntador a la primera casilla de los datos que contiene, y se puede mover a cualquier otra casilla, es decir que se puede poner a apuntar a cualquier casilla dentro del arreglo.**
    - [ ] Falso
    - [ ] Verdadero
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **Falso**.
    </details>

5. **Si se tiene la dirección de memoria de una variable, se puede modificar el dato que contiene esa variable a través de su dirección.**
    - [ ] Falso
    - [ ] Verdadero
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **Falso**.
    </details>

6. **¿Cuál es la forma correcta de declarar un puntero a una estructura llamada Persona?**
    - [ ] struct Persona *p;
    - [ ] struct p Persona;
    - [ ] Persona p;
    - [ ] Persona *p;
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **struct Persona *p;**.
    </details>

7. **¿Qué operador se utiliza para acceder al valor almacenado en una variable de tipo puntero?**
    - [ ] &
    - [ ] *
    - [ ] $
    - [ ] #
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **\***.
    </details>

8. **Para pasar un parámetro por referencia a una función, se puede hacer de dos formas:**
    - [ ] Pasando el apuntador a la variable que es parámetro de la función y pasando el alias (o referencia) de la variable
    - [ ] Pasando una copia del dato que contiene la variable y pasando la dirección de memoria de la variable
    - [ ] Pasando un apuntador a la variable y creando memoria dinámica dentro de la función
    - [ ] Pasando una copia de la estructura que contiene el parámetro y pasando una des referenciación del parámetro que se quiere modificar
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **Pasando el apuntador a la variable que es parámetro de la función y pasando el alias (o referencia) de la variable**.
    </details>

9. **La instrucción new, para memoria dinámica:**
    - [ ] Elimina la memoria creada dinámicamente, del apuntador que se pasa como parámetro
    - [ ] Crea un apuntador a null (NULL o nullptr), con la memoria reservada
    - [ ] Permite crear memoria de forma dinámica, retornando el dato que contiene la memoria. Si no hay dato, retorna NULL o nullptr
    - [ ] Busca un espacio en memoria para el tipo de dato indicado, reserva ese espacio y retorna su dirección
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **Busca un espacio en memoria para el tipo de dato indicado, reserva ese espacio y retorna su dirección**.
    </details>

10. **Si tenemos un apuntador llamado ap que apunta a una estructura que contiene los campos a y b, la siguiente es una forma de asignar 5 al campo a:**
    - [ ] `ap.a = 5;`
    - [ ] `&ap.a = 5;`
    - [ ] `*ap->a = 5;`
    - [ ] `ap->a = 5;`
    <details>
      <summary>Ver respuesta</summary>
      La respuesta correcta es **ap->a = 5;**.
    </details>

11. **Encuentre los errores en la siguiente declaración de punteros:**

    ```cpp
    int x, *p, &y;
    char* b = "Cadena larga";
    char* c = "C";
    void *r = &x;
    ```

    - [ ] Es incorrecta la declaración de &y.
    - [ ] No se puede declarar un puntero de tipo void. Al atributo *b no se le puede asignar un valor.
    - [ ] Es incorrecta la declaración de &y y no se puede declarar un puntero de tipo void.
    - [ ] El código no tiene errores.

<details>
  <summary>Ver respuesta</summary>
  La opción correcta es la **3**. La declaración `int x, *p, &y;` es incorrecta ya que "&y" intenta declarar una referencia, lo cual no es válido en este contexto. Además, la línea `void *r = &x;` es correcta y no contiene errores.
</details>

12. **Un arreglo unidimensional se puede indexar con la aritmética de punteros.**

    - [ ] Verdadero.
    - [ ] Falso.

<details>
  <summary>Ver respuesta</summary>
  La respuesta correcta es **Verdadero**. En C y C++, un arreglo unidimensional puede ser tratado como un puntero al primer elemento del arreglo, lo que permite utilizar la aritmética de punteros para acceder a sus elementos.
</details>

13.  **¿Cuál de las siguientes líneas genera errores de compilación?**

    ```cpp
    1. float val1 = 5.f;
    2. float val2 = 5.75F;
    3. float val3 = 3f;
    4. float val4 = 2;
    5. double val5 = 3e3L;
    ```

    - [ ] Línea 1
    - [ ] Línea 2
    - [ ] Línea 3
    - [ ] Línea 1 y 3
    - [ ] Línea 4

<details>
  <summary>Ver respuesta</summary>
  La opción correcta es la **4**. La línea 1 (`float val1 = 5.f;`) es correcta y no genera errores de compilación. La línea 3 (`float val3 = 3f;`) genera un error de compilación debido al sufijo "f" utilizado incorrectamente. Las demás líneas tampoco generan errores de compilación.
</details>



14. **Según el siguiente código, ¿la asignación de la línea 3 y 4 apunta a la misma posición de memoria?**

    ```cpp
    1 int b[5];
    2 int *bPtr;
    3 bPtr = &b[0];
    4 bPtr = b;
    ```

    - [ ] Verdadero
    - [ ] Falso

<details>
  <summary>Ver respuesta</summary>
  La respuesta correcta es **Falso**.
</details>


15.    **Una estructura (struct) en C++ puede estar compuesta de funciones además de variables.**

       - [ ] Falso
       - [ ] Verdadero

<details>
  <summary>Ver respuesta</summary>
  La respuesta correcta es **Falso**.
</details>

16.   **Una vez que un arreglo dinámico ha sido creado en C++ con una cierta cantidad de elementos, no puede redimensionarse para contener más o menos elementos.**

- [ ] Falso
- [ ] Verdadero

<details>
  <summary>Ver respuesta</summary>
  La respuesta correcta es **Falso**.
</details>

17.    **Una cadena de caracteres representada como un arreglo de caracteres termina con un carácter nulo (10), que indica el final de la cadena**
      - [ ] Falso
      - [ ] Verdadero

<details>
  <summary>Ver respuesta</summary>
  La respuesta correcta es **Verdadero**.
</details>

1.    **En C++, tanto los archivos binarios como los de texto se pueden abrir utilizando objetos de las clases ifstream (para lectura) y ofstream (para escritura), pero es necesario especificar el modo (binario o texto) en el que se abrirá el archivo**.

      - [ ] Falso
      - [ ] Verdadero

<details>
  <summary>Ver respuesta</summary>
  La respuesta correcta es **Verdadero**.
</details>

19.   **Un arreglo unidimensional no puede contener valores tipo struct**

      - [ ] Falso
      - [ ] Verdadero

<details>
  <summary>Ver respuesta</summary>
  La respuesta correcta es **Falso**.
</details>
