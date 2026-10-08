# Turnero de atención local

Aplicación de atención con una fila FIFO y cuatro mesas. El botón **Llamar siguiente** envía al primer cliente de la fila a la mesa libre que lleva más tiempo desocupada. Si todas están ocupadas, el botón queda desactivado. Al finalizar una atención, esa mesa queda disponible para el siguiente turno.

## Componentes

- API en Python con FastAPI y WebSocket para sincronizar cambios en tiempo real.
- Interfaz Angular.
- Estado en memoria: no usa base de datos. Reiniciar el servidor limpia los turnos.
- El frontend usa `localhost`; es para operar en la misma computadora.

## Inicio (cuando Python esté instalado)

Abre una terminal en esta carpeta y ejecuta `start.bat`. La primera vez instala dependencias y abre el navegador. Requiere Python 3.10+ y Node.js 20+ con npm. También puedes iniciar por separado: `backend\start-backend.bat` y `frontend\start-frontend.bat`.

## GitHub

Subir este código a GitHub guarda y comparte el proyecto; no mantiene encendido el servidor local. Para operar, el backend debe estar ejecutándose en la computadora donde se atiende. No incluyas contraseñas ni tokens en archivos del proyecto.
