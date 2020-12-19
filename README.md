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
- Los programas estocásticos se aprovechan de que las distribuciones probabilísticas de un problema se conocen o pueden ser estimadas

### Probabilidades
- La probabilidad es una medida de la certidubmbre asociada a un evento o suceso futuro y suele expresarse como un número entre 0 y 1
- Una probabilidad de 0 significa que un suceso jamás sucederá
- Una probabilidad de 1 significa que un suceso está garantizado de suceder en el futuro
- P(A) + P(-A) = 1
    - Ley del complemento
- P(A y B) = P(A) * P(B)
    - Ley multiplicativa
- P(A o B) = P(A) + P(B)
    - Mutuamente exclusivos
- P(A o B) = P(A) + P(B) - P(A y B) (No exclusivos)
    - Ley aditiva

## Inferencia Estadística
- Con las simulaciones podemos calcular las probabilidades de eventos complejos sabiendo las probabilidades de eventos simples
- ¿Qué pasa cuando no sabemos las probabilidades de los eventos simples?
- Las técnicas de la inferencia Estadística nos permiten inferir/concluir las propiedades de una población a partir de una muestra aleatoria.

El principio guía de la inferencia estadística es que una muestra aleatoria tiende a exhibir las mismas propiedades que la población de la cual fue extraída.

### Ley de los grandes números
- En pruebas independientes repetidas con la misma probabilidad p de un resultado, la fracción de desviaciones de p converge a cero conforme las cantidad de pruebas se acerca al infinito.


