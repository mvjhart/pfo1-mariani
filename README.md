# PFO1 - Landing de Portafolio

## Índice

* [Descripción](#descripción)
* [Tecnologías](#tecnologías)
* [Demo](#demo)
* [Decisiones de diseño](#decisiones-de-diseño)
* [Accesibilidad](#accesibilidad)
* [Uso de IA](#uso-de-ia)

## Descripción

Landing page desarrollada para la Primera Práctica Profesional Obligatoria (PFO1) de Frontend.

El proyecto presenta una simplificación de mi perfil como desarrolladora de software, mis habilidades, una sección de contacto y una sección Bonus desarrollada exclusivamente con HTML y CSS.

## Tecnologías

* HTML5
* CSS3
* Google Fonts - Inter
* Flexbox
* CSS Grid

## Demo

https://pfo1-mariani.vercel.app/

## Decisiones de diseño

La propuesta utiliza una estética basada en degradados, transparencias y una combinación de colores violeta, rosa, azul y amarillo.

Se utilizó CSS Grid y Flexbox para estructurar y distribuir las distintas secciones, junto con unidades y funciones flexibles como `clamp()`, `min()`, `vw` y `rem` para adaptar los tamaños de los elementos a diferentes tamaños de pantalla. Las media queries se utilizaron para incorporar ajustes específicos: un separador visual en el footer para pantallas pequeñas y el respeto de la preferencia `prefers-reduced-motion`.

La navegación entre las distintas páginas se realiza mediante enlaces HTML.

El formulario de contacto fue incluido como una interfaz de contacto, pero no se configuró para realizar envíos reales. Al tratarse de una PFO desarrollada únicamente con HTML y CSS, sin JavaScript ni un backend para procesar los datos, se decidió no agregar `method="post"` ni un `action` que no tendría un destino funcional. De esta manera, se evita simular una funcionalidad que el proyecto no puede procesar.

La sección Bonus, **"Excusatrón 3000"**, presenta una interacción demostrativa sin JavaScript. El modal se implementó utilizando la pseudoclase `:target`, aprovechando los enlaces internos de HTML para mostrar y ocultar el contenido. Si bien actualmente existe una alternativa declarativa mediante el elemento `<dialog>` y los atributos `command` y `commandfor`, esta última funcionalidad es relativamente reciente y todavía no cuenta con soporte completo entre navegadores. Se optó por utilizar `:target` para mantener una implementación sencilla y ampliamente compatible.

También se incorporaron transiciones y animaciones CSS para mejorar la interacción visual.

## Accesibilidad

Las imágenes utilizadas incluyen el atributo `alt`. En particular, si bien el ícono de advertencia del archivo `bonus.html` está oculto para lectores de pantalla mediante `aria-hidden`, ya que cumple una función puramente decorativa, se decidió mantener el atributo `alt` como respaldo textual ante un posible fallo de carga y para cumplir explícitamente con el requisito de la consigna.

Los formularios incluyen etiquetas `label` asociadas a sus respectivos controles mediante el atributo `for`, y se incorporaron estados `:focus-visible` para facilitar la navegación mediante teclado.

También se incorporó `prefers-reduced-motion` para respetar la preferencia del usuario de reducir las animaciones y transiciones.

## Uso de IA

Para el desarrollo de esta PFO se utilizó **ChatGPT (GPT-5.6 Luna)**, utilizando el **plan gratuito**.

La herramienta se utilizó como apoyo y consulta durante el proceso de desarrollo, principalmente para agilizar la resolución de dudas puntuales y revisar aspectos específicos de HTML y CSS. Entre otras cosas, se consultaron cuestiones relacionadas con accesibilidad, como `prefers-reduced-motion`, así como conceptos que ya conocía pero que necesitaba recordar o verificar rápidamente, por ejemplo el reseteo de estilos o la conversión de valores y unidades relativas a rangos para utilizar con `clamp()`.

También se utilizó como herramienta de consulta para verificar si existían características o actualizaciones recientes de HTML y CSS que pudieran ser relevantes para el desarrollo y que no hubiera tenido en cuenta.

Las respuestas y sugerencias obtenidas fueron revisadas y adaptadas de acuerdo con la visión y las decisiones propias del proyecto.

Mi experiencia previa con IA está principalmente vinculada al estudio y al apoyo durante el desarrollo de proyectos, por lo que en esta PFO se utilizó de la misma manera: como una herramienta de consulta y apoyo disponible durante el proceso, manteniendo el análisis, la toma de decisiones y la implementación bajo criterio propio.
