Ejercicio 2.E.2 08 - Manga Volume

Lógica del programa
Para resolver este ejercicio del Bloque IV, me enfoqué en la representación textual de los objetos y la modularización mediante métodos auxiliares. Diseñé la clase `MangaVolume` definiendo tres atributos: `tituloSerie` (String), `numeroTomo` (int) y `cantidadPaginas` (int), acompañados de su respectivo constructor parametrizado.

Para organizar el comportamiento de la clase y aplicar el principio de encapsulamiento y modularización, implementé dos métodos:
1. Un método auxiliar privado llamado `esTomoExtenso()` que evalúa mediante una estructura condicional (`if/else`) si la `cantidadPaginas` supera las 300 páginas, retornando un valor booleano.
2. Un método público llamado `esEdicionEspecial()` que actúa como interfaz y reutiliza internamente al método privado anterior para definir si el tomo clasifica como edición especial.

Además, sobrescribí el método canónico `toString()` utilizando la anotación `@Override`. Esto me permitió personalizar la forma en que el objeto se representa como cadena de texto, concatenando los atributos y llamando implícitamente al método `esEdicionEspecial()`.

Dentro de la clase `Main`, implementé la siguiente lógica de prueba:
1. Instancié dos objetos de tipo `MangaVolume` ("Another" con 677 páginas y "Adabana" con 192 páginas).
2. Imprimí ambos objetos directamente pasando la instancia a la sentencia `System.out.println()`. Al hacerlo, comprobé cómo Java invoca automáticamente al método `toString()` sobrescrito, mostrando por consola la ficha técnica estructurada y el resultado dinámico del método booleano para cada caso.

Ejecución en consola
*(Arrastrá y soltá acá la captura de pantalla de tu IDE mostrando el código funcionando)*
<img width="1917" height="1018" alt="image" src="https://github.com/user-attachments/assets/8c12a4e3-8a9d-4aa2-beb7-85f66b1a963a" />
