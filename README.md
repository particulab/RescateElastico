# Rescate Elástico

**Rescate Elástico** es un minijuego educativo de física desarrollado como parte del proyecto **EulerGames**.

El objetivo del juego es calcular la compresión necesaria de un resorte para lanzar una cápsula de suministros hacia una plataforma de rescate. El jugador debe leer los datos físicos, hacer sus cálculos y probar su respuesta dentro de la simulación.

El juego corre directamente en navegador y está hecho con **HTML, CSS, JavaScript y Canvas**, sin librerías externas.

---

## Objetivo educativo

El juego busca que el estudiante relacione dos fenómenos físicos:

1. **Energía potencial elástica**
2. **Movimiento parabólico**

La cápsula es impulsada por un resorte comprimido. Al liberarse, la energía almacenada en el resorte se transforma en velocidad de salida. Después, la cápsula sigue una trayectoria parabólica bajo la acción de la gravedad.

El estudiante debe calcular la compresión adecuada del resorte para que la cápsula caiga dentro de la zona segura de la plataforma.

---

## Mecánica del juego

En cada ronda se muestran datos físicos como:

* masa de la cápsula;
* constante del resorte;
* ángulo de lanzamiento;
* altura de salida;
* distancia horizontal a la plataforma;
* altura de la plataforma;
* zona segura de aterrizaje;
* gravedad.

El jugador ajusta la compresión del resorte y lanza la cápsula.

Antes del intento no se muestran fórmulas ni soluciones. El estudiante debe realizar el cálculo por su cuenta.

Después del lanzamiento, el juego muestra retroalimentación física, incluyendo información como:

* velocidad de salida;
* tiempo de empuje del resorte;
* tiempo de vuelo;
* si faltó o sobró energía;
* distancia de error respecto al objetivo.

---

## Controles

### Teclado

* `←` disminuye la compresión en 0.10 m.
* `→` aumenta la compresión en 0.10 m.
* `↓` disminuye la compresión en 0.01 m.
* `↑` aumenta la compresión en 0.01 m.
* `Enter` lanza la cápsula.
* `R` continúa a la siguiente ronda después del intento.

### Botones en pantalla

* `− 0.10 m`
* `+ 0.10 m`
* `− 0.01 m`
* `+ 0.01 m`
* `Lanzar`
* `Continuar`
* `Sonido`

---

## Modelo físico

El juego usa un modelo físico simplificado pero coherente.

Durante la primera fase, la cápsula es empujada por el resorte mientras este se descomprime. Después, al llegar a la boca del lanzador, inicia el vuelo parabólico.

La simulación considera:

* resorte ideal;
* conversión de energía elástica en energía cinética;
* gravedad constante;
* movimiento parabólico sin resistencia del aire;
* tiempo de animación equivalente al tiempo físico de la simulación.

La trayectoria se muestra únicamente después del lanzamiento. También se dibujan marcas de tiempo sobre la trayectoria para visualizar cómo cambia la rapidez de la cápsula durante el vuelo.

---

## Condiciones de victoria

El jugador gana si la cápsula cae dentro de la zona segura de la plataforma.

El jugador pierde si:

* la cápsula cae antes de la plataforma;
* la cápsula se pasa de la plataforma;
* no alcanza la altura necesaria;
* toca el suelo antes de llegar al objetivo.

---

## Aleatorización

Cada ronda genera valores físicos distintos dentro de intervalos controlados.

El juego asegura que las rondas sean resolubles. Para lograrlo, internamente genera una compresión correcta oculta y construye una situación física compatible con esa solución.

El jugador no ve esa respuesta. Solo ve los datos físicos necesarios para calcularla.

---

## Características principales

* Juego educativo basado en cálculo real.
* Una sola variable de control: compresión del resorte.
* Datos físicos visibles.
* Sin fórmulas antes del intento.
* Retroalimentación física después del lanzamiento.
* Rondas aleatorias resolubles.
* Animación en tiempo real.
* Movimiento de la cápsula durante la descompresión del resorte.
* Trayectoria parabólica con marcas de tiempo.
* Interfaz clara y distribuida.
* Sonido opcional.
* Controles por teclado y botones.
* Código en un solo archivo `index.html`.
* Sin librerías externas.

---

## Cómo ejecutar el juego

1. Descarga o clona este repositorio.
2. Abre el archivo `index.html` en cualquier navegador moderno.
3. Lee los datos físicos de la ronda.
4. Calcula la compresión del resorte.
5. Ajusta la compresión en el juego.
6. Presiona **Lanzar**.

No se requiere instalación ni servidor.

---

## Tecnologías utilizadas

* HTML
* CSS
* JavaScript
* Canvas API

---

## Filosofía de EulerGames

**EulerGames** es una colección de minijuegos educativos de física y matemáticas.

La idea no es que el estudiante solo observe una simulación ni que gane por reflejos. Cada juego busca que el estudiante:

1. lea datos;
2. piense el fenómeno;
3. calcule en su libreta;
4. tome una decisión;
5. pruebe su respuesta;
6. reciba retroalimentación física.

El juego debe sentirse como un reto, no como una calculadora disfrazada.

---

## Estado del proyecto

Versión inicial funcional.

El juego ya incluye la mecánica principal, generación de rondas, controles, animación, retroalimentación y visualización de trayectoria.

Posibles mejoras futuras:

* agregar eficiencia del lanzador;
* incluir resistencia del aire;
* permitir modificar el ángulo;
* añadir obstáculos;
* crear niveles de dificultad;
* guardar estadísticas del jugador;
* mejorar efectos visuales y sonoros.

---

## Autor

Proyecto desarrollado como parte de **EulerGames**, una iniciativa de minijuegos educativos para aprender física y matemáticas mediante retos interactivos en navegador.
