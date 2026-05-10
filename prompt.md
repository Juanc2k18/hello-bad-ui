# Prompt: Bad UI — Controlador de Volumen Frustrante

Crea un único archivo `index.html` autocontenido usando únicamente:

- HTML semántico
- CSS puro
- Vanilla JavaScript

No uses frameworks ni dependencias externas.

El archivo debe poder abrirse directamente con doble clic en un navegador moderno.

---

## Objetivo

Desarrollar una **“Bad UI”** deliberadamente frustrante basada en un controlador de volumen para reproducir un sonido genérico.

La experiencia debe ser:

- Funcional
- Incómoda
- Burocrática
- Agotadora para el usuario
- Segura

---

## 1. Estructura HTML semántica

Usa HTML semántico y evita la “sopa de `div`s”.

La estructura debe incluir:

- `header` con un `h1` principal describiendo la interfaz.
- `nav` con botones o enlaces inútiles o redundantes.
- `main` como contenedor principal.
- Dentro de `main`, usar múltiples `section`.
- Una `section` para el reproductor de sonido.
- Una `section` para las confirmaciones y captcha ficticio.
- Una `section` para logs o mensajes burocráticos.
- `footer` con texto irónico o copyright falso.

Usa los siguientes elementos:

- `h1`
- `h2`
- `p`
- `button`
- `form`
- `label`
- `input`
- `ul`
- `li`

Todos los elementos interactivos importantes deben tener atributos `id` únicos para manipularlos desde JavaScript mediante el DOM.

Ejemplos de `id` esperados:

- `#playBtn`
- `#increaseBtn`
- `#captchaForm`
- `#volumeDisplay`
- `#systemLog`

---

## 2. Comportamiento general

La interfaz debe reproducir un sonido genérico usando exclusivamente **Web Audio API**.

No usar:

- Archivos `.mp3` externos
- Librerías
- Recursos externos
- Descargas

El sonido debe ser:

- Un tono sinusoidal simple en loop
- Seguro
- No agresivo

El volumen debe iniciar en `50%`.

Debe existir:

- Un botón **“Reproducir sonido”**
- Un botón **“Subir volumen”**
- Un indicador visual del volumen actual

---

## 3. Mecánica hostil

Cada vez que el usuario quiera subir el volumen:

1. Debe pasar por tres confirmaciones consecutivas.
2. Luego debe resolver un captcha ficticio.
3. Solo después el volumen aumenta `2%`.

Las confirmaciones deben ser exageradamente burocráticas.

Ejemplos:

- “¿Seguro que desea iniciar el procedimiento de incremento sonoro?”
- “Confirme que confirma la confirmación anterior.”
- “Última oportunidad para cancelar esta operación irreversible.”

El captcha debe implementarse dentro de un `form` usando:

- `label`
- `input`
- `button`

Ejemplos de captcha:

- Escribir una palabra absurda
- Resolver una suma innecesaria
- Copiar texto exacto

Si el usuario falla:

- Mostrar mensajes sarcásticos
- Resetear el proceso
- O disminuir el volumen

---

## 4. Degradación automática

Implementa un sistema de degradación automática usando estado en JavaScript.

Crear la variable:

```js
let volumeLevel = 50;
````

Cada `20` segundos:

* Disminuir automáticamente el volumen en `5%`
* Nunca bajar de `0%`
* Actualizar inmediatamente el DOM para reflejar el cambio visual del volumen

---

## 5. JavaScript y DOM

Usar **Vanilla JavaScript** estructurado y comentado.

Requisitos técnicos:

* Usar `querySelector`
* Usar `addEventListener`
* Usar `setInterval`
* Usar estado con variables `let`
* Actualizar el DOM dinámicamente

Ejemplos esperados:

* Escuchar eventos `click` en botones
* Actualizar texto del volumen
* Mostrar y ocultar secciones
* Insertar logs dinámicos en listas HTML

Todos los elementos importantes deben tener `id`.

---

## 6. CSS y diseño visual

Usar CSS puro dentro de una etiqueta `<style>`.

Definir variables globales en `:root`.

Ejemplo:

```css
:root {
  --color-bg: #111;
  --color-panel: #1e1e1e;
  --color-accent: #ff4444;
  --color-text: #f5f5f5;
  --color-warning: #ffaa00;
}
```

Usar propiedades como:

* `background`
* `color`
* `font-family`
* `padding`
* `margin`
* `border`
* `border-radius`
* `gap`

Usar Flexbox y Grid:

* `display: flex`
* `display: grid`

El diseño visual debe incluir:

* Estilo corporativo opresivo
* Paneles innecesarios
* Advertencias exageradas
* Botones incómodamente pequeños
* Jerarquía visual confusa
* Mensajes de error prominentes

Agregar:

* Animaciones molestas leves
* Efectos `hover` innecesarios
* Loaders falsos
* Delays artificiales

---

## 7. Experiencia Bad UI

La interfaz debe sentirse:

* Lenta
* Burocrática
* Frustrante
* Absurdamente compleja

Pero debe seguir siendo:

* Funcional
* Estable
* Entendible técnicamente

No incluir:

* Malware
* Permisos reales
* Fullscreen forzado
* Spam de ventanas
* Descargas
* Comportamiento peligroso

---

## 8. Resultado final

Entregar un único archivo `index.html` completamente funcional con:

* HTML semántico
* CSS organizado
* Vanilla JavaScript comentado
* Comportamiento hostil deliberado
* Experiencia de usuario frustrante pero segura
