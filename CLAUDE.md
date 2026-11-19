# Proyecto: Trip Colombia 2026

Página web del viaje de Jaime y Ariel a Colombia (26 nov – 6 dic 2026), publicada con GitHub Pages.

- Repo: https://github.com/jsansi/Trip-Colombia-2026 (público, rama `main`)
- Página: https://jsansi.github.io/Trip-Colombia-2026/
- `gh` está en `C:\Program Files\GitHub CLI\gh.exe` (puede no estar en el PATH de la sesión)

## Cómo trabajar con el usuario
- Jaime **no es programador**: explicar en español, paso a paso y en lenguaje simple ("for dummies").
- Él deja capturas, PDFs y links en `privado/` y avisa. Leerlos, extraer los datos y actualizar.
- Puede pedir usar Claude in Chrome para leer reservas (Airbnb, Gmail, aerolíneas) con su sesión: solo leer, nunca modificar.

## Reglas de privacidad (IMPORTANTE)
- `privado/` está en `.gitignore`: **nunca** subirlo ni copiar su contenido sensible a archivos versionados.
- La página es **pública**. NO publicar: códigos de reserva, números de boleto, pasaportes o documentos, apellidos completos, correos, teléfonos, direcciones exactas, nombres de edificios ni números de apartamento, asientos, ni información médica o alimentaria de los viajeros.
- SÍ se puede publicar (aprobado por Jaime): nombres "Jaime & Ariel", fechas, ciudades, **números de vuelo** y horarios, nombre del alojamiento + barrio.
- Antes de cada push, buscar en `index.html` términos sensibles (códigos, apellidos, direcciones).

## Dónde está cada cosa
- `index.html`: todo el contenido está en arrays JS al inicio del `<script>`: `CITY`, `DAYS` (cada día con `ev` fijos y `opts` {rec, chill, party}; `true` en la posición 3 = reservar/pendiente), `FLIGHTS`, `HOMES`, `FOOD`, `CLIMA`, `LOOKS`, `PRICES`, `CHECK`.
- `privado/datos-viaje.md`: datos crudos (vuelos con códigos, direcciones de Airbnb).
- `privado/plan-de-viaje.md`: plan completo (logística, salud, comida, tours, fiesta, finanzas, checklist).

## Respaldo de `privado/`
`privado/` es su **propio repositorio git** (privado en GitHub, aparte del público). Cuando cambie algo ahí: `cd privado && git add . && git commit && git push`. Nunca hacerlo público.

## Flujo de publicación
1. Editar `index.html` → verificar el JS (`node --check` sobre el contenido del `<script>`).
2. Revisar que no haya datos privados.
3. `git add index.html && git commit && git push` → Pages se actualiza en 1–2 min.
