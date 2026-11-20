# Temas de temporada · Mochis

La página cambia sola según la fecha (decoración, colores, guirnalda de arriba, frase del día e imagen de cabecera).

| Fechas | Clave | Tema |
|---|---|---|
| 1 al 6 de enero | `reyes` | Año Nuevo y Reyes Magos |
| 7 al 31 de enero | `invierno` | Café calientito, frío (no lo pediste: puse algo suave) |
| Febrero | `candelaria` | Día de la Candelaria: tamales, velas |
| Marzo | `primavera` | Flores amarillas |
| Abril | `vacaciones` | Semana Santa y playa |
| Mayo | `mamas` | Día de las Madres |
| Junio | `papas` | Día del Padre |
| Julio y agosto | `verano` | Verano (agosto no lo mencionaste: seguí con verano) |
| Septiembre | `independencia` | Fiestas patrias |
| Octubre | `muertos` | Día de Muertos |
| Noviembre y diciembre | `navidad` | Navidad |

## Probar un tema antes de tiempo
Agrega `?tema=clave` al link. Ejemplo: `https://dlaluz007-sketch.github.io/mochis/?tema=muertos`

## Forzar un tema (por ejemplo si Semana Santa cae en marzo)
En `menu.json`, dentro de `"config"`, agrega `"tema": "vacaciones"`. Quítalo para volver al modo automático.

## Imágenes de cabecera (opcional)
Cada tema busca su imagen en la carpeta `temas/` con el nombre de su clave: `temas/muertos.jpg`, `temas/mamas.jpg`, etc.
Si el archivo no existe, se muestra el logo normal con la decoración.
Ya incluí `temas/navidad.jpg` (tu banner "¡Mañana! Ofrecemos:"). Como dice "Mañana", solo aparece cuando se ve el menú de mañana.
Las demás imágenes deben ir SIN esa frase (así se ven siempre). Tamaño sugerido: horizontal, unos 1200 x 700 px.

### Ideas de prompts (estilo de sus banners de Navidad)
Base: "Banner horizontal en estilo ilustración kawaii cálida. Tres gatitos chef con gorro de cocina y delantal (uno naranja llamado Aslan, uno crema llamado Mochi, uno atigrado llamado Chencho) junto al logo redondo de Mochis, café para todo el día, aprobado por Aslan. Sin texto, salvo el logo. Escena:"
- **reyes:** rosca de reyes, coronas y estrellas doradas, los gatitos con capa de rey.
- **invierno:** tazas de café humeantes, bufandas y cobijitas, luces cálidas.
- **candelaria:** tamales, atole, velas pequeñas, un niño Dios en su cunita.
- **primavera:** flores amarillas, mariposas, abejitas, pasto verde.
- **vacaciones:** los gatitos con short, tabla de surf, balón de playa y salvavidas, mar y sol.
- **mamas:** flores, lazos rosas y un cartel con lazo que diga "Para mamá".
- **papas:** los gatitos con tazas de "El mejor papá del mundo", corbatas, trofeo.
- **verano:** sol, sandía, helados, palmeras, gafas de sol.
- **independencia:** bandera, banderines verde-blanco-rojo, gatitos con bigote y sombrero de charro, antojitos mexicanos.
- **muertos:** catrinas, flores de cempasúchil, papel picado, velitas, pan de muerto.

## Frases
Las frases de cada tema están en `index.html` (busca `frases:`). Cambian una por día. Puedes editarlas libremente.
Son frases originales, no citas de personas famosas.
