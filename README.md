# ID Camper v3.2

PWA independiente para:
- extraer localmente un identificador numérico desde una URL de un área;
- buscar áreas por nombre/localidad;
- ordenar por puntuación, opiniones, distancia o nombre.

## Importante
ID Camper no es una aplicación oficial ni está afiliada a Park4Night.

La búsqueda utiliza un pequeño servicio intermedio (Cloudflare Worker) para evitar depender de un proxy CORS público. El Worker consulta la interfaz actual observada en proyectos públicos recientes (`https://park4night.com/api/places/around`). Esa interfaz no está documentada oficialmente por Park4Night y puede cambiar.

## Configuración
Antes de publicar `index.html`, cambia `CONFIG.API_BASE` por la URL del Worker, por ejemplo:
`https://idcamper-api.tu-subdominio.workers.dev`

El Worker está en la carpeta `worker/` del paquete separado `ID_Camper_v3.2_Worker.zip`.
