# ¿Cómo se hace en Python?

**Buscador de herramientas de Python para estudiar y consultar durante las clases y los ejercicios.**

La idea nació de una necesidad muy concreta: **a veces sé lo que quiero hacer en Python, pero no recuerdo qué método, función u operador necesito**. En vez de memorizar todas las herramientas, ¿por qué no tener un buscador que permita encontrarlas escribiendo la acción?

Por ejemplo, escribo **«contar letras»**, **«sacar claves»**, **«añadir elemento»** o **«invertir lista»** y encuentro las opciones pertinentes, con explicaciones y ejemplos.

Este proyecto empezó así: **detecté un problema real en mi aprendizaje, pensé cómo resolverlo y desarrollé la solución con la ayuda de ChatGPT**. No es una aplicación creada por la IA de forma autónoma: la necesidad, el objetivo, los requisitos, el enfoque y las decisiones sobre su utilidad proceden de una persona que está aprendiendo a programar. ChatGPT ha colaborado en la implementación, la organización del contenido y las explicaciones.

## ¿Qué permite hacer?

- **Buscar por lo que quiero conseguir**, sin conocer de antemano el nombre de la herramienta.
- Filtrar por tipo de dato (`str`, `int`, `float`, `list`, `dict`, `tuple` y `set`), operación o clase de herramienta.
- Distinguir **métodos**, **funciones integradas** y **operadores**.
- Consultar la sintaxis, una explicación sencilla, los tipos que recibe, qué devuelve y si modifica el objeto original.
- Ver ejemplos de código con **resultados esperados**, errores habituales, herramientas relacionadas y enlaces a la documentación oficial.
- Comparar cómo se realiza una misma operación según el tipo de dato.
- Consultar conversiones habituales y una pequeña chuleta con conceptos básicos, `help()` y `dir()`.
- **Guardar favoritos** en el navegador y copiar ejemplos.

### Contenido actual (versión 0.2)

| Contenido | Cantidad |
| --- | ---: |
| Herramientas y operaciones | 109 |
| Comparaciones entre tipos | 19 |
| Ejemplos de conversión | 5 |

## Cómo utilizarlo

1. Descarga el archivo **`index.html`**.
2. Ábrelo con doble clic desde tu ordenador, en un navegador moderno.
3. Escribe lo que necesitas: `buscar elemento`, `contar apariciones`, `ordenar lista`...
4. Lee las herramientas encontradas, revisa el ejemplo y copia el código si te sirve.

**No necesita instalar Python, extensiones, servidores ni dependencias.** El buscador funciona sin conexión a internet. Los enlaces a la documentación externa sí requieren conexión.

**Atajos:** `/` lleva el cursor al buscador y `Esc` vacía el texto de búsqueda cuando el cursor está dentro.

## ¿Cómo está hecho?

- **HTML:** estructura de la aplicación.
- **CSS:** presentación y modo oscuro inspirado en un editor de código.
- **JavaScript:** búsqueda, filtros, comparaciones y favoritos.
- **JSON:** catálogo de herramientas con sus ejemplos, incorporado dentro de `index.html` para que funcione incluso al abrirlo como archivo local.
- **`localStorage`:** conserva los favoritos en ese navegador, cuando el navegador lo permite.

El archivo `catalogo_python.json` es una **copia separada del catálogo**, útil para consultar y ampliar los datos. **No es necesario para ejecutar la aplicación**: la versión actual ya incorpora el catálogo en `index.html`. Si se modifica el JSON externo, los cambios no aparecen automáticamente en la web; también habría que actualizar el catálogo incrustado en el HTML.

## Qué no hace todavía

- No ejecuta código Python: enseña ejemplos y resultados preparados.
- No utiliza IA ni conexión a una API para interpretar las búsquedas; utiliza palabras clave y coincidencias locales.
- No guarda un historial de búsquedas.
- No sustituye la comprensión del código ni la documentación oficial: sirve para localizar la herramienta adecuada y aprender a utilizarla.

## Origen y créditos

**Idea original, detección de la necesidad, definición de requisitos y dirección del proyecto:** su creador, estudiante de programación.

**Asistencia técnica:** ChatGPT (OpenAI), utilizado como apoyo para generar y organizar código, preparar el catálogo, revisar ejemplos y documentar la aplicación.

La colaboración es parte del sentido del proyecto: **aprender programación no consiste en memorizar todo ni en delegarlo todo, sino en identificar problemas, formular buenas preguntas, comprender las soluciones y saber adaptarlas**.

> No quería memorizar Python entero. Quería saber qué herramientas existen, encontrarlas en segundos y aprender a utilizarlas.

## Próximos pasos

El objetivo no es llenar la aplicación de funciones sin criterio. Antes de añadir más contenido, importa que el buscador **muestre primero las opciones realmente útiles** para cada consulta. Después se podrán añadir sinónimos, más casos prácticos y mejoras en el comparador.

---

**Proyecto educativo personal.** Python y los nombres de sus herramientas pertenecen a sus respectivos titulares. Los enlaces de referencia conducen a la documentación oficial de Python.
