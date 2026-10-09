Portafolio interactivo · Grupo Roca Primaria

Una experiencia 3D para explorar las soluciones digitales y los servicios de Grupo Roca Primaria. Diseñada para demostraciones con clientes, combina un mapa interactivo con presentaciones por solución y control opcional mediante la cámara.

## Acceder al portafolio

[**Abrir el portafolio interactivo**](https://rocaprimaria01.github.io/Introduccion-Roca-Primaria/Portafolio_Roca_Primaria_Premium.html)

Cuando se publique `index.html` en la raíz del repositorio, también se podrá acceder desde:

https://rocaprimaria01.github.io/Introduccion-Roca-Primaria/

## Qué incluye

- **34 soluciones** distribuidas en cinco líneas de servicio: sistemas de calidad en planta, tableros e indicadores, solución de problemas y entrenamiento, salud ocupacional y servicios, y cómo trabajamos.
- **Tres vistas 3D:** ADN, Centralizado y Árbol.
- **Presentaciones de tres diapositivas por solución:** Explicación, Objetivo y Entradas y salidas.
- Selección por clic o por permanencia del cursor durante **1,5 segundos**, con un indicador circular.
- Control opcional con gestos de la mano mediante la cámara.
- Creación de ideas o proyectos y personalización de imágenes, guardadas en el navegador.
- Diseño adaptable a computadora, tablet y celular, con fondo integrado y paneles translúcidos.

## Cómo utilizarlo

### Explorar el mapa

| Acción | Control |
| --- | --- |
| Girar el mapa | Arrastrar con el ratón o el dedo |
| Acercar o alejar | Rueda del ratón o gesto de pellizco en pantalla táctil |
| Abrir una solución | Hacer clic o mantener el cursor sobre ella durante 1,5 segundos |
| Cambiar de vista | Botones ADN, Centralizado y Árbol |
| Cambiar de vista con el teclado | `1`: ADN · `2`: Centralizado · `3`: Árbol |
| Alternar imágenes y puntos | Botón de imágenes/puntos |
| Cambiar el efecto de selección | Botón de efecto |
| Agregar una idea o proyecto | Botón `+` |

Durante la selección por permanencia, el mapa se pausa para mantener estable el objetivo. También se suspende el trabajo de animación 3D mientras está abierto el panel de descripción.

### Leer las diapositivas

Cada solución tiene tres secciones:

1. **Explicación:** descripción del artefacto o servicio.
2. **Objetivo:** propósito que busca atender.
3. **Entradas y salidas:** información requerida y resultados descritos para esa solución.

Usa **Anterior**, **Siguiente**, las pestañas o las flechas `←` y `→` del teclado. En pantalla táctil puedes deslizar horizontalmente sobre el contenido.

La navegación es cíclica: después de la tercera diapositiva vuelves a la primera; desde la primera puedes retroceder a la tercera.

Para cerrar, usa la **X**, pulsa `Esc` o haz clic fuera del panel. La X, las flechas y las pestañas también admiten selección por permanencia durante **1,5 segundos**. Para repetir una acción sobre el mismo control, retira el cursor y vuelve a colocarlo encima.

### Usar la cámara

1. Abre el sitio publicado mediante HTTPS.
2. Pulsa el botón de la mano **✋** y permite el acceso a la cámara.
3. Espera a que cargue el modelo y muestra una mano frente a la cámara.
4. Mueve el cursor con la mano o utiliza los gestos siguientes.

| Gesto | Acción |
| --- | --- |
| Mantener el cursor sobre un punto o control compatible | Seleccionar después de 1,5 segundos |
| Pellizco rápido entre pulgar e índice | Seleccionar un punto o botón |
| Mantener el pellizco y mover la mano | Girar el mapa |
| Mantener el pellizco y acercar o alejar la mano | Ajustar el zoom |

El cursor permanece por encima de las diapositivas para permitir su navegación y cierre. Para detener la cámara, pulsa nuevamente **✋** o cierra su ventana con la **X**.

Una iluminación uniforme y una mano visible facilitan el seguimiento. La fluidez depende del dispositivo, la cámara y la capacidad de procesamiento disponible. El control convencional con ratón o pantalla táctil sigue disponible.

## Publicar en GitHub Pages

Este proyecto es una página HTML estática. No necesita un servidor de aplicación ni un proceso de compilación.

1. Sube la versión más reciente del portafolio a la raíz del repositorio con el nombre **`index.html`**, en minúsculas.
2. En GitHub, entra a **Settings → Pages**.
3. En **Build and deployment**, elige **Deploy from a branch**.
4. Selecciona la rama **`main`** y la carpeta **`/ (root)`**; guarda la configuración.
5. Espera a que finalice la publicación y abre la dirección que muestra GitHub Pages.

Si mantienes únicamente `Portafolio_Roca_Primaria_Premium.html`, utiliza el enlace completo que termina en ese nombre. La dirección principal necesita `index.html` para abrir el portafolio directamente.

Si conservas ambos archivos, actualiza los dos al publicar cambios para evitar versiones distintas. Conserva `Portafolio_Roca_Primaria_Premium.html` mientras utilices enlaces o códigos QR que apunten a ese nombre.

## Archivos

| Archivo | Uso |
| --- | --- |
| `index.html` | Página de inicio para GitHub Pages |
| `Portafolio_Roca_Primaria_Premium.html` | Portafolio accesible mediante su nombre completo |
| `README.md` | Descripción e instrucciones del proyecto |
| `QR_Roca_Primaria.png` — opcional | Código QR para compartir o incorporar a presentaciones |
| `QR_Roca_Primaria.svg` — opcional | Versión vectorial del QR para impresión |

El fondo y las imágenes incluidas están integrados en el HTML. No necesitan una carpeta de imágenes aparte.

## Requisitos y almacenamiento

- Navegador actualizado con soporte para WebGL. Puedes probarlo en Chrome o Edge.
- Conexión a internet para cargar Three.js, las fuentes y, al activar la cámara, MediaPipe y su modelo de seguimiento.
- Cámara y permiso de acceso únicamente si deseas utilizar el control por gestos.
- Las ideas, imágenes personalizadas y preferencias se guardan mediante `localStorage` en el navegador utilizado. No se sincronizan entre dispositivos ni se publican en GitHub.
- Borrar los datos del sitio elimina esas personalizaciones. Abrir la página local y abrirla desde GitHub Pages puede mostrar datos guardados diferentes.
- Las nuevas ideas incluyen la descripción capturada; sus objetivos, entradas y salidas quedan por definir. Las 34 soluciones iniciales tienen contenido preparado para las tres diapositivas.

El seguimiento de la mano se ejecuta en el navegador. La implementación no incluye grabación ni envío del video a un servidor propio; sí descarga las bibliotecas y el modelo necesarios para realizar el seguimiento.

## Solución de problemas

| Problema | Qué revisar |
| --- | --- |
| Aparece un error 404 | Confirma que `index.html` esté en la raíz de la rama publicada, o usa el enlace con el nombre completo del archivo |
| Se muestra una versión anterior | Comprueba que la publicación terminó y recarga con `Ctrl + F5` |
| No aparece el mapa 3D | Revisa la conexión a internet, la compatibilidad con WebGL y posibles bloqueos de las bibliotecas externas |
| La cámara no inicia | Abre la versión HTTPS, revisa los permisos y comprueba que la cámara esté disponible |
| El seguimiento responde lento | Mejora la iluminación y cierra otras aplicaciones que utilicen intensivamente la cámara o los gráficos |
| La selección por permanencia no se completa | Mantén el cursor sobre el mismo objetivo; cambiar de objetivo reinicia el contador |
| No aparecen las ideas guardadas en otro dispositivo | El almacenamiento es local a cada navegador y dirección del sitio |

## Tecnologías

HTML, CSS y JavaScript; Three.js para el mapa 3D; MediaPipe Hand Landmarker para el seguimiento de la mano; y GitHub Pages para la publicación estática.

---

**Grupo Roca Primaria · Ingeniería, tecnología y personas.**
