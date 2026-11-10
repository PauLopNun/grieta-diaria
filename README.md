<div align="center">

# Grieta Diaria

### Un campeón de League of Legends al día. El mismo para todo el equipo.

*Cinco minutos en la Grieta y a seguir currando.*

<a href="https://paulopnun.github.io/grieta-diaria/"><img src="https://img.shields.io/badge/JUGAR%20AHORA-c8aa6e?style=for-the-badge&labelColor=010a13" alt="Jugar ahora" height="42"></a>

<br><br>

![Campeones](https://img.shields.io/badge/campeones-171-c8aa6e?style=flat-square&labelColor=0a1428)
![Modos](https://img.shields.io/badge/modos-7-c8aa6e?style=flat-square&labelColor=0a1428)
![Splash arts](https://img.shields.io/badge/splash%20arts-843-c8aa6e?style=flat-square&labelColor=0a1428)
![Voces](https://img.shields.io/badge/voces-342-c8aa6e?style=flat-square&labelColor=0a1428)
![Habilidades](https://img.shields.io/badge/habilidades-855-c8aa6e?style=flat-square&labelColor=0a1428)

<img src="docs/campeones.png" alt="Iconos de campeones" width="88%">

</div>

---

## Tecnologías

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=githubpages&logoColor=white)
<br>
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pillow](https://img.shields.io/badge/Pillow-WebP-0a1428?style=for-the-badge&logo=python&logoColor=c8aa6e)
![League of Legends](https://img.shields.io/badge/League%20of%20Legends-C28F2C?style=for-the-badge&logo=leagueoflegends&logoColor=white)
![Riot Games](https://img.shields.io/badge/Riot%20Games-D32936?style=for-the-badge&logo=riotgames&logoColor=white)
![Claude](https://img.shields.io/badge/Hecho%20con-Claude-D97757?style=for-the-badge&logo=claude&logoColor=white)

</div>

- **El juego:** HTML, CSS y JavaScript a pelo. Ni frameworks, ni librerías, ni compilación: una sola página.
- **Los recursos:** Python con Pillow, para bajar de CommunityDragon los iconos, las habilidades, los splash y las voces, y convertirlos a WebP y MP3.
- **El alojamiento:** GitHub Pages.

---

## Modos de juego

| Modo | Cómo se juega |
|---|---|
| **Clásico** | Escribe un campeón y compara 7 características: género, posición, especie, recurso, rango, región y año. Verde si coincide, amarillo si coincide en parte, rojo si no, y una flecha que indica si el campeón de hoy salió antes o después. |
| **Cita** | Escucha lo que dice el campeón al ser elegido o al ser bloqueado. A los 4 fallos se desbloquea la otra frase. |
| **Habilidad** | Un icono de habilidad, en gris y girado. A los 3 fallos recupera el color y a los 6 se endereza. **Extra:** ¿en qué tecla va? |
| **Emoji** | Cuatro emojis que describen al campeón. Cada fallo destapa uno. |
| **Splash** | Un trozo muy ampliado de un splash art. Cada fallo aleja la imagen. **Extra:** ¿qué aspecto es? |
| **Título** | El apodo oficial del campeón, como «la Espada de los Darkin». |
| **Libre** | Partidas ilimitadas tipo Clásico con un campeón al azar. |

Cada día a las **00:00 (hora de Madrid)** salen campeones nuevos en todos los modos. La elección sale de una semilla con la fecha, así que todo el mundo juega con los mismos.

<div align="center">
<img src="docs/captura.jpg" alt="Captura del juego en modo Clásico" width="80%">
</div>

---

## Lo que trae

- **Estadísticas por modo:** partidas, racha actual, mejor racha y media de intentos.
- **Cuenta atrás** hasta el campeón de mañana.
- **Copiar el resultado** con sus cuadraditos de colores, para pegarlo en el chat del equipo.
- **Fondo** con un splash difuminado distinto cada día, que nunca es la respuesta de ningún modo.
- **Sin cuentas:** los intentos y las estadísticas se guardan en el navegador de cada uno.

---

## Estructura

```
index.html          el juego entero (iconos de campeones y habilidades incrustados)
splash/<id>.webp    hasta 5 aspectos por campeón, apilados en una tira de 1280×720 cada uno
voz/<id>.json       frases de voz en MP3 (base64): "e" al elegir, "b" al bloquear
```

Para probarlo en local hace falta un servidor, porque las voces se cargan con `fetch`:

```bash
python -m http.server
# y abre http://localhost:8000
```

---

## Créditos

Imágenes, voces y datos de campeones: **Riot Games**, vía [CommunityDragon](https://www.communitydragon.org/).

<sub>*Grieta Diaria isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing Riot Games properties. Riot Games, and all associated properties are trademarks or registered trademarks of Riot Games, Inc.*</sub>

<div align="center">

**Hecho por diversión, sin ánimo de lucro.**

</div>
