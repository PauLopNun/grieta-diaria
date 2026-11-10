<div align="center">

# ⚔️ Grieta Diaria

**Un campeón de League of Legends al día. El mismo para todo el equipo.**
Cinco minutos en la Grieta y a seguir currando.

[**▶ Jugar**](https://paulopnun.github.io/grieta-diaria/)

</div>

---

## Modos de juego

| Modo | Cómo se juega |
|---|---|
| **Clásico** | Escribe cualquier campeón y compara 7 características: género, posición, especie, recurso, rango, región y año de salida. 🟩 coincide, 🟨 coincide en parte, 🟥 no coincide, y una flecha te dice si el campeón de hoy salió antes o después. |
| **Cita** | Escucha la frase que dice el campeón al ser elegido o al ser bloqueado. A los 4 fallos se desbloquea la otra frase. |
| **Habilidad** | Un icono de habilidad, en gris y girado. A los 3 fallos recupera el color y a los 6 se endereza. Extra: adivina en qué tecla va (Pasiva, Q, W, E o R). |
| **Emoji** | Cuatro emojis que describen al campeón. Cada fallo destapa uno más. |
| **Splash** | Un trozo muy ampliado de un splash art. Cada fallo aleja la imagen. Extra: adivina qué aspecto es. |
| **Título** | El apodo oficial del campeón, como «la Espada de los Darkin». |
| **Libre** | Partidas ilimitadas tipo Clásico con un campeón al azar. No cuenta para las rachas. |

Cada día a las **00:00 (hora de Madrid)** salen campeones nuevos en todos los modos. La elección va por una semilla de la fecha, así que todo el mundo tiene los mismos.

## Lo que trae

- **171 campeones** con sus iconos y sus 855 habilidades.
- **843 splash arts**, hasta 5 aspectos por campeón, que van rotando.
- **342 frases de voz** en castellano.
- **Estadísticas por modo:** partidas, racha actual, mejor racha y media de intentos.
- **Cuenta atrás** hasta el campeón de mañana.
- **Botón para copiar el resultado** con sus cuadraditos de colores y pegarlo en el chat del equipo.

Los intentos y las estadísticas se guardan en el navegador de cada uno. No hay cuentas ni servidor.

## Cómo está hecho

Una sola página HTML, con su CSS y JavaScript, sin librerías ni compilación. Los iconos van incrustados en la propia página; los splash (`splash/`) y las voces (`voz/`) se cargan al vuelo.

```
index.html        el juego entero
splash/<id>.webp  hasta 5 aspectos por campeón, apilados en una tira de 1280×720 cada uno
voz/<id>.json     frases de voz en MP3 (base64): "e" al elegir, "b" al bloquear
```

Para probarlo en local hace falta un servidor, porque las voces se cargan con `fetch`:

```bash
python -m http.server
```

## Créditos

Las imágenes, voces y datos de campeones son de **Riot Games**, sacados de [CommunityDragon](https://www.communitydragon.org/).

*Grieta Diaria isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing Riot Games properties. Riot Games, and all associated properties are trademarks or registered trademarks of Riot Games, Inc.*

Proyecto hecho por diversión, sin ánimo de lucro.
