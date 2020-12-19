## Estadística Computacional con Python
--

### Objetivos
- Aprender cuándo utilizar programación dinámica y sus beneficios
- Entender las diferencias entre programas deterministas y estocásticos
- Aprender a utilizar programación estocástica
- Aprender a crear simulaciones computacionales válidas

### Programación Dinámica
El nombre programación dinámica se escogió para esconder a patrocinadores gubernamentales el hecho que en realidad estaba haciendo matemáticas. La frese programación dinámica es algo que ningún congresista puede oponerse.

- **Subestructura Óptima**. Una solución global óptima se puede encontrar al combinar soluciones óptimas de subproblemas locales.
- **Problemas empalmados**. Una solución que involucra resolver el mismo problema en varias ocasiones.

### Memoization
- La memorización es una técnica para guardar cómputos previos y evitar realizarlos nuevamente.
- Normalmente se utiliza un diccionario, donde las consultas se pueden hacer en O(1).
- Intercambia tiempo por espacio.

### Caminos aleatorios
- Es un tipo de simulación que elige aleatoriamente una decisión dentro de un conjunto de decisiones válidas.
- Se utiliza en muchos campos del conocimiento cuando los sistemas no son deterministas e incluyen elementos de aleatoriedad

## Programación Estocástica
- Un programa es determínistico si cuando se corre en el mismo input produce el mismo output
- Los programas determiniísticos son muy importantes, pero existen problemas que no pueden resolverse de esa manera
- La programación estocástica permite introducir aleatoriedad a nuestros programas para crear simulaciones que permiten resolver otro tipo de problemas