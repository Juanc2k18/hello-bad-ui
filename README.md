# Bad UI: Controlador de Volumen Burocrático

## Descripción

Este proyecto consiste en una interfaz web deliberadamente frustrante para controlar el volumen de un sonido genérico producido por el código. La aplicación está hecha en un único archivo `index.html`, usando únicamente HTML semántico, CSS puro y Vanilla JavaScript, sin frameworks ni dependencias externas.

## Diseño de la interfaz

La página usa una estructura HTML semántica con `header`, `nav`, `main`, varias `section` y `footer`.

El diseño visual tiene un estilo corporativo opresivo, con paneles oscuros, advertencias exageradas, botones pequeños, mensajes administrativos y una jerarquía visual intencionalmente confusa.

También se incluyen animaciones leves, loaders falsos y mensajes sarcásticos para reforzar la sensación de trámite innecesario.

## Funcionamiento

La interfaz reproduce un tono sinusoidal simple mediante la Web Audio API, sin usar archivos de audio externos.

El volumen inicia en 50%. El usuario puede presionar el botón **Reproducir sonido** para activar el tono.

Para subir el volumen, el usuario debe:

1. Pasar tres confirmaciones consecutivas.
2. Resolver un captcha ficticio.
3. Esperar pequeños retrasos artificiales.

Si completa el proceso correctamente, el volumen solo aumenta 2%. Si falla el captcha, el proceso se reinicia y el volumen puede disminuir.

Además, cada 20 segundos el sistema reduce automáticamente el volumen en 5%, sin bajar de 0%.

## Razonamiento detrás de la idea

La idea principal fue exagerar acciones simples hasta convertirlas en procesos absurdamente complejos. Subir el volumen, que normalmente debería ser una acción inmediata, se transforma en un trámite lleno de confirmaciones, reglas innecesarias y castigos menores. Como inspiración, se tomó el ejemplo tratado en clase.

La interfaz sigue siendo funcional y segura, pero intencionalmente mala desde el punto de vista de experiencia de usuario. Esto permite mostrar cómo decisiones de diseño pequeñas pueden afectar negativamente la usabilidad de una aplicación.

## Tecnologías usadas

- HTML semántico
- CSS puro
- Vanilla JavaScript
- Web Audio API
## Cómo usarlo

Abrir el archivo `index.html` directamente en un navegador moderno haciendo doble clic sobre él.
