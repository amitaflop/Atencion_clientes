# Turnero de atención local

Aplicación de atención con una fila FIFO y cuatro mesas. El botón **Llamar siguiente** envía al primer cliente de la fila a la mesa libre que lleva más tiempo desocupada. Si todas están ocupadas, el botón queda desactivado. Al finalizar una atención, esa mesa queda disponible para el siguiente turno.

## Componentes

- API en Python con FastAPI y WebSocket para sincronizar cambios en tiempo real.
- Interfaz Angular.
- Estado en memoria: no usa base de datos. Reiniciar el servidor limpia los turnos.
- El frontend usa `localhost`; es para operar en la misma computadora.

## Cómo abrirlo

1. Extrae el ZIP.
2. Asegúrate de tener Python 3.10+ y Node.js 20+ instalados.
3. Haz doble clic en `start.bat` y espera a que se abra el navegador.

La primera vez se descargan las dependencias, así que requiere conexión a Internet durante la instalación inicial. Después, los turnos se procesan localmente. No necesitas abrir un editor de código.

## GitHub

GitHub guarda y comparte el código; no mantiene encendido el servidor local. Para operar, deja abierta la ventana del backend en la computadora donde atienden. No guardes contraseñas ni tokens en este proyecto.
