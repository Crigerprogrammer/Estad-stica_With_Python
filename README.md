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

### Falacia del apostador
- La falacia del apostador señala que después de un evento extremo, ocurrirán eventos menos extremos para nivelar la media
- La regresión a la media señala que después de un evento aleatorio extremo, el siguiente evento probablemente será menos extremo.

### Media
- Es una medida de tendencia central
- Comúnmente es conocida como el promedio
- La media de una población se denota con el simbolo u . La media de una muestra se denota con X

### Varianza
- La varianza mide qué tan propagados se encuentran un conjunto de valores aleatorios de su media.
- Mientras que la media nos da una idea de dónde se encuentran los valores, la varianza nos dice que tan dispersos se encuentran.
- La varianza siempre debe entenderse con respecto a la media

### Desviación estándar
- La desviación estándar es la raíz cuadrada de la varianza.
- Nos permite entender, también, la propagación y se debe entender siempre relacionado a la media.
- La ventaja sobre la varianza es que la desviación estándar está en las mismas unidades que la media.

### Distribución normal
- Es una de las distribuciones más recurrentes en cualquier ámbito
- Se define completamente por su media y su desviación estándar
- Permite calcular intervalos de confianza con la regla empírica.

### Regla empírica
- También conocida como la regla 68-95-99.7
- Señala cuál es la dispersión de los datos en una distribución normal a uno, dos y tres sigmas
- Permite calcular probabilidades con la densidad de la distribución normal

### Simulaciones de Montecarlo
- Permite crear simulaciones para predecir el resultado de un problema
- Permite convertir problemas determinísticos en problemas estocásticos
- Es utilizado en una gran diversidad de áreas, desde la ingeniería hasta la biología y el derecho.

## Muestreo

- Hay ocasiones en la que no tenemos acceso a toda la población que queremos explorar
- Uno de los grandes descubrimientos de la estadística es que las muestras aleatorias tienden a mostrar las mismas propiedades de la población objetivo
- El tipo de muestreo que hemos hecho hasta ahora es muestreo probabilistíco 
- En un muestreo aleatorio cualquier miembro de la población tiene la misma probabilidad de ser escogido
- En un muestreo estratitificado tomamos en consideración las características de la población para partirla en subgrupos y luego tomamos muestras de cada subgrupo.
    - Incrementala probabilidad de que el muestreo sea representativo de la población

### Teorema del límite central
- Es uno de los teoremas más importantes de la estadística
- Establece que muestras aleatorias de cualquier distribución van a tener una distribución normal
- Permite entender cualquier distribución como la distribución normal de sus medias y eso nos permite aplicar todo lo que sabemos de distribuciones normales

### Datos experimentales
- Es la aplicación del método científico
- Es necesario comenzar con una teoría o hipótesis sobre el resultado al que se quiere llegar
- Basado en la hipótesis se debe crear un experimento para validad o falsear la hipótesis
- Se valida o falsea una hipótesis midiendo la diferencia entre las mediciones experimentales y aquellas mediciones predichas por la hipótesis

### Regresión Lineal
- Permite aproximar una función a un conjunto de datos obtenidos de manera experimental
- No necesariamente permite aproximar funciones lineales, sino que sus variantes permiten aproximar cualquier función polinómica

### Conclusiones
- La programación dinámica permite optimizar problemas que tienen subestructura óptima y subproblemas empalmados
- Las computadoras pueden resolver problemas determinísticos y estocásticos
- Podemos generar simulaciones computacionales para responder preguntas del mundo real
- La inferencia estadística nos permite tener confianza de que nuestras simulaciones arrojan resultados válidos