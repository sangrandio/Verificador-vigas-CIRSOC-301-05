# Verificador de vigas de acero — CIRSOC 301-05

Herramienta interactiva para verificar vigas de acero (perfiles IPN) según el reglamento **CIRSOC 301-05**, con datos de catálogo oficiales CIRSOC/IRAM-IAS. Corre 100% en el navegador — un solo archivo HTML, sin instalación, sin conexión a internet, sin backend.

Desarrollada para uso interno de **Baleal Ingeniería** como herramienta rápida de chequeo en la revisión de anteproyectos estructurales.

## Qué hace

A partir de los datos de la viga (cargas, ancho de influencia, tipo de apoyo, perfil), calcula y muestra:

- Carga de servicio, momento último (Mu) y corte último (Qu)
- Clasificación de la sección (compacta / no compacta / esbelta) en ala y alma
- Verificación a flexión (fluencia y pandeo lateral-torsional), con % de material utilizado
- Verificación a corte, con % de material utilizado
- Verificación de flecha admisible
- Búsqueda automática del perfil IPN más liviano que verifica todas las condiciones
- Esquema de la viga con su deformada según el tipo de apoyo

## Cómo usarlo

Abrí [`verificador_vigas.html`](./verificador_vigas.html) con doble clic, o entrá directo por GitHub Pages: `https://<tu-usuario>.github.io/<nombre-repo>/verificador_vigas.html`

No requiere instalar nada ni tener conexión a internet una vez descargado.

## Alcance y limitaciones

- Solo perfiles **IPN** (catálogo CIRSOC/IRAM-IAS 80 a 600).
- Solo secciones **compactas** — si la sección clasifica como no compacta o esbelta, la herramienta lo indica y no calcula (requiere verificación manual, Cap. F3–F5 del CIRSOC 301-05).
- Pandeo lateral-torsional calculado con las fórmulas del Cap. F para perfiles doblemente simétricos, con J y Cw estimados por fórmula clásica de perfil abierto de pared delgada (el catálogo IPN no publica estos valores).
- Esta herramienta es una ayuda de cálculo rápido y **no reemplaza** la verificación profesional completa de un ingeniero estructural ni el uso de software de cálculo certificado.

## Stack

HTML + JavaScript vanilla. Sin frameworks, sin dependencias externas.

## Licencia

MIT — libre para usar, modificar y compartir.

## Autor

Baleal Ingeniería
