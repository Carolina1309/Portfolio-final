# DESIGN.md — Guía de diseño

## Estilo
**Minimalista con personalidad.** Mucho espacio en blanco, pocas decoraciones y detalles en rosa. Las secciones alternan fondo claro (rosa muy suave) y oscuro (bordó) para separar visualmente el contenido.

## Paleta de colores
Paleta de Coolors en degradé, del bordó oscuro al rosa pálido.

| Variable | Color | Uso |
|---|---|---|
| `--oscuro` | `#590D22` | Header, secciones oscuras, texto sobre fondo claro |
| `--principal` | `#800F2F` | Títulos en fondo claro, botón principal, footer |
| `--secundario` | `#A4133C` | Subtítulos, etiquetas, texto de tecnologías |
| `--intenso` | `#C9184A` | Hover del botón principal |
| `--vibrante` | `#FF4D6D` | Hover de los enlaces de contacto |
| `--acento` | `#FF758F` | Líneas bajo títulos, bordes, marco de la foto |
| `--rosa-medio` | `#FF8FA3` | Hover del menú |
| `--rosa-suave` | `#FFB3C1` | Subtítulos y labels sobre fondo oscuro |
| `--rosa-palido` | `#FFCCD5` | Insignias y etiquetas de tecnologías |
| `--rosa-claro` | `#FFF0F3` | Fondo de secciones claras y texto sobre fondo oscuro |

Alternancia de secciones:
- Sobre mí → clara
- Skills → oscura
- Proyectos → clara
- Contacto → oscura
- Footer → principal (bordó)

## Tipografías (Google Fonts)
- **Títulos:** Playfair Display (600, 700), serif elegante.
- **Textos:** Poppins (300–600), sans-serif moderna.

## Componentes
- **Botones:** forma de píldora (`border-radius: 50px`). Principal relleno bordó (`--principal`); secundario con borde.
- **Chips de skills:** píldoras con borde rosa (`--acento`); al pasar el mouse se rellenan.
- **Tarjetas de proyecto:** fondo blanco, esquinas redondeadas (12px), sombra suave, línea rosa bajo la imagen, se elevan al hover.
- **Foto de perfil:** esquinas redondeadas con un marco rosa desplazado detrás.

## Responsive
- **> 900px:** grillas de 2 columnas.
- **≤ 900px (tablet):** todo en 1 columna, contenido de "Sobre mí" centrado.
- **≤ 600px (celular):** header con el menú debajo del logo, tipografías más chicas.
