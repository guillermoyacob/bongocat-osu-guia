# Guía en español para Bongo cat para OSU! 🇦🇷

*bongocat-osu de Kuroni versión 1.5.3*

## ⌨️ Teclas para STD

* **`Z` y `X`** → Mueven la manito izquierda cuando jugás

* **`C`** → Bongo se pone lentes cuando dibujás

* **`V`** → Bongo saluda

## ⚙️ Configuración para que funcione

### A) En Bongo Cat para OSU!

En el archivo de configuración de Bongo (`config.json`) tenés que cambiar esto:

1. **Uso de tableta gráfica:**

   Si querés que Bongo use una tableta en vez de un mouse hacé esto (si no, salteate este paso). Tenés que cambiar el modo de mouse verdadero (`true`) por falso (`false`), te quedaría así:

   ```
   "mouse": false,
   ```

   De esa manera el gatito Bongo cambia el mouse por la tableta

2. **Fondo para Stream (Chroma Key):**

   Si lo vas a usar para hacer stream seguramente vas a querer quitarle el fondo y que te quede solo Bongo jugando en la mesa, sin fondo. Para eso se cambia esta línea en la configuración, dentro de donde dice `decoration`:

   ```
   "rgb": [0, 255, 0],
   ```

   Ese es el color de fondo, que si lo escribís así corresponde al verde (el que se usa para *chroma key*). Ese verde es el que reconoce OBS para que lo filtre (o lo borre y lo deje transparente, para que se entienda)

> **Aclaración extra:** No te preocupes por el borde de la ventana del programa Bongo Cat para OSU!, porque OBS no toma los bordes

### B) Si querés usarlo en OBS

Tenés que ir a **Añadir fuente** y elegís **Captura de juego**. Esa fuente va a ser Bongo, ponele de nombre `Bongo cat`. Dentro de esa ventana elegís:

1. **Capturar una ventana específica**

2. Elegís ahí la del programa de Bongo

3. Seleccionás la opción: **Coincidir con el título, de lo contrario buscar ventana del mismo ejecutable**

4. Solo dejás tildadas las casillas **Captura de cursor** y **Utilice compatibilidad anti trampas**

5. Tasa de captura elegís **Normal (recomendada)**

6. Espacio de color elegís **sRGB**

**Configuración del Filtro Verde:**

> Después das botón derecho sobre esa fuente que acabás de crear y configurar, elegís **Filtros** y en la ventana de filtros le agregás un filtro de efecto de **Chroma** de color verde (eso se hace en donde dice *Tipo de clave de color*, ahí tiene que decir **Verde**)

### C) En OSU! Lazer

Tenés que desactivar las siguientes opciones (**control + o** para abrir el panel de opciones):

En la sección de **Entrada:**

1. **Ratón de precisión:** Desactivado

2. **Limitar el cursor del ratón a la ventana:** Nunca

Eso te libera el puntero para que lo puedan usar otros programas, si no Bongo no mueve la manito derecha

### D) Otras cosas para tener en cuenta

* **No ejecutar Bongo como administrador:** Si no, OBS no puede acceder al programa de Bongo

* **Si Bongo se congela:** Si Bongo se llega a congelar en algún momento podés probar cambiando de ventanas, seleccionar la de Bongo y volver

Espero que esta guía les sirva!

**guiyee_ar** 🇦🇷
