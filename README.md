# 🇨🇴 Trip Colombia 2026

Página interactiva de nuestro viaje a Colombia (Jaime & Ariel) · **26 nov – 6 dic 2026**
Cartagena → Medellín → Bogotá → Cartagena

🔗 **Ver la página:** https://jsansi.github.io/Trip-Colombia-2026/

## Qué tiene la página
- 🌞 Cuenta regresiva (durante el viaje muestra "Día X de 11")
- 🗺️ Ruta con las 4 paradas
- 📅 Itinerario día a día con 3 modos: ⭐ recomendado · 😌 tranquilo/resaca · 🎉 fiesta, y lo que hay que reservar marcado
- ✈️ Vuelos · 🏠 Alojamientos (solo zona)
- 🍽️ Dónde comer y platos típicos · 👗 Clima, dress code y outfits · 🎟️ Precios de entradas y covers
- 🧳 Checklist de maleta (se guarda en cada celular) · 💡 Tips

## Estructura
| Carpeta / archivo | Para qué sirve |
|---|---|
| `index.html` | La página del viaje (todo el contenido está en los datos al inicio del `<script>`) |
| `img/` | Fotos e imágenes para la página |
| `docs/` | Documentos **no sensibles** |
| `privado/` | ⚠️ Reservas, pasaportes, plan con info personal. **Nunca se sube a GitHub** (está en `.gitignore`) |
| `CLAUDE.md` | Reglas del proyecto para Claude Code |

## Cómo actualizar
Dejar la info nueva en `privado/` y pedirle a Claude Code que la agregue. Los cambios se publican solos en 1–2 minutos después del `git push`.
