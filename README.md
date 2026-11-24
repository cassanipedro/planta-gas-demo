# Planta de Gas Aguada Norte · gemelo digital (demo)

Demo interactiva de una planta de tratamiento de gas y su yacimiento, estilo recorrida en dron.
Sobre una única foto aérea 4K generada con IA, una cámara virtual vuela entre las áreas de la planta.
Cada área muestra indicadores en vivo, que son simulados, y fichas de estado por equipo.

## Cómo verla

Abrí `index.html` en el navegador, siempre junto a la carpeta `img/`. Si querés servirla localmente:

```
python -m http.server 8765
```

y entrá a http://localhost:8765.

## Qué tiene

- **11 áreas** que siguen el camino del gas:
  - pad de pozos
  - slug catcher
  - separación de entrada
  - aminas (CO₂)
  - deshidratación con TEG
  - punto de rocío
  - turbocompresión
  - medición fiscal
  - energía y sala de control
  - condensado
  - antorcha
- **38 equipos** con ficha: estado, índice de salud, indicadores en tiempo real con tendencia, ficha técnica e historial.
- **Vuelo en dron** (botón ▶): recorrido automático con HUD de dron (REC, altura, velocidad, rumbo, GPS) que se detiene en los equipos con alertas.
- **Navegación**:
  - clic en un área o en los botones de abajo;
  - arrastrar para moverse y rueda para hacer zoom;
  - ← → para pasar de área y Esc para volver;
  - minimapa arriba a la derecha.
- **Escena viva**:
  - llama de antorcha animada con humo;
  - vapor en la regeneradora de aminas;
  - gases calientes y refracción sobre las chimeneas de las turbinas;
  - ventiladores girando;
  - sombras de nubes, balizas y polvo en suspensión.
- **Alta resolución**: la zona de la planta usa mosaicos con upscale ×2. El zoom se limita a la resolución real de la foto para que no se pixele.
- Se adapta a celular.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | Versión actual: planta realista, cámara continua tipo dron |
| `version-maqueta.html` | Versión anterior: estilo maqueta, una imagen por área |
| `version-petroleo.html` | Primera versión: yacimiento de petróleo |
| `img/planta/` | Foto aérea 4K, miniatura y mosaicos de alta resolución |
| `img/gas/`, `img/v1-petroleo/` | Imágenes de las versiones anteriores |

Todo el contenido es genérico: nombres, TAGs y valores son ficticios.
