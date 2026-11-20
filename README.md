# Mi Solcito — Jardín Maternal (demo)

Landing de demostración para **Mi Solcito**, jardín maternal en Mendoza 435 Norte, San Juan, Argentina.

Sitio de una sola página (`index.html` autocontenido: CSS y JS inline), mobile first.

## Contenido

- Presentación del jardín y las cuatro salas por edad (lactarios, deambuladores, 2 y 3 años).
- Propuesta pedagógica y rutina diaria orientativa.
- **Pre-inscripción en línea**: nombre del niño/a, fecha de nacimiento (sugiere la sala según la edad), adulto responsable y teléfono. Al enviar muestra la confirmación y un botón que abre WhatsApp con los datos ya redactados.
- Cómo se asignan los cupos y cómo funciona la lista de espera.
- Cuotas y formas de pago (conceptos, sin montos).
- Reseñas: 5.0 de promedio sobre 22 reseñas de Google.
- Ubicación, mapa y coordinación de visitas.

## Desarrollo local

```bash
python3 -m http.server 8080
# http://localhost:8080
```

## Deploy

Contenedor nginx estático:

```bash
docker build -t misolcito .
docker run --rm -p 8080:80 misolcito
```

En EasyPanel: app `demo-misolcito` dentro del proyecto `clientes`, build por `Dockerfile`, dominio
`https://clientes-demo-misolcito.rddxeh.easypanel.host`.

El panel no redespliega solo con el push: hay que disparar el deploy del servicio después de cada cambio.

## Notas

- Sin emojis: todos los iconos son SVG inline.
- Fotografías de Unsplash (uso libre). El texto evita prometer resultados y no inventa montos de cuotas.
- Sitio de demostración con fines de presentación comercial.