# VitalSysTech — logotipo

## Concepto
Un trazado de pulso atraviesa una circunferencia y la desborda por ambos lados.
El círculo aporta masa y hace de contenedor; la línea que lo rebasa es el
argumento de la marca: **la señal no se detiene en el límite del sistema**.
Hospital, laboratorio y domicilio como un solo continuo.

## Bloque de marca VST

El monograma **VST** lleva la V en azul marino, la S en celeste y la T en morado,
con el nombre completo debajo en dorado. Es el bloque que aparece en la barra de
navegación y en el pie de la web.

| | Claro | Oscuro |
|---|---|---|
| V | `#1B3B6F` | `#4C82CE` |
| S | `#4FC3E8` | `#5CCBEE` |
| T | `#34216B` | `#8E79D4` |
| Nombre | `#A8842B` | `#D6B65E` |

Sobre fondo oscuro los tres tonos van aclarados: con los originales, la V y la T
se funden con el panel. Archivos: `lockup-vst-claro.svg` y `lockup-vst-oscuro.svg`.

**Tipografía del monograma:** IBM Plex Mono Bold. Los remates cortados de la V,
la S escuadrada y el travesaño de la T dan carácter de instrumento, y pertenece
a la misma superfamilia que el texto de la web. Se descartaron las tipografías
de ciencia ficción: envejecen mal y en un sector que vende fiabilidad juegan en
contra. El nombre va en Plex Mono Medium muy traqueado, como una etiqueta de
equipo, separado por un filete dorado que da estructura al conjunto.

**Sistema de dos marcas.** El bloque VST se usa donde hay sitio para el nombre;
el símbolo del pulso queda para favicon y avatares, porque a 16 px tres letras
no se leen. Ambos comparten ahora la misma tríada —aro en el azul de la V,
trazo en el celeste de la S—, así que se reconocen como la misma empresa.

Regenerar el bloque: `python3 generar-lockup.py` (necesita las tipografías
IBM Plex Mono Bold y Medium).

## Qué archivo usar

| Uso | Archivo |
|---|---|
| Web, firmas, documentos | `logo-horizontal.svg` |
| Sobre fondo oscuro | `logo-horizontal-dark.svg` |
| Espacio vertical estrecho | `logo-apilado.svg` / `logo-apilado-dark.svg` |
| Una sola tinta (sellos, bordado, fax) | `logo-horizontal-mono.svg` |
| Sobre foto o color intenso | `logo-horizontal-blanco.svg` |
| Avatar de LinkedIn, WhatsApp Business, app | `icono-violeta.svg` · `icono-512.png` |
| Pestaña del navegador | `favicon.svg` (ya embebido en el HTML) |
| Icono de pantalla de inicio | `icono-192.png` |

## Reglas de uso

**Área de respeto.** Deje libre alrededor del logotipo al menos la altura del
círculo de la marca. Nada debe invadir ese margen.

**Tamaño mínimo.** El logotipo horizontal no baja de 120 px de ancho en pantalla
ni de 30 mm impreso. Por debajo, use solo la marca. Por debajo de 24 px, use el
favicon: la circunferencia se cierra visualmente y deja de leerse.

**No haga esto.** No cambie los colores, no aplique sombras ni degradados, no
deforme la proporción, no encierre el logotipo horizontal en una caja, no
sustituya la tipografía y no separe la marca del logotipo con más espacio del
definido.

## Color

| | Hex | Uso |
|---|---|---|
| Violeta | `#34216B` | Circunferencia y logotipo |
| Magenta | `#E0577F` | Trazado del pulso |
| Tinta | `#17122E` | Logotipo sobre fondo claro |
| Lila | `#C9BEE8` | Circunferencia sobre fondo oscuro |
| Panel | `#0D0920` | Fondo del favicon y del icono oscuro |

## Tipografía
IBM Plex Sans SemiBold, **trazada en curvas**. Los archivos no dependen de que
la fuente esté instalada: se ven igual en cualquier equipo. IBM Plex es de
código abierto (licencia SIL OFL), así que puede usarse comercialmente sin coste.

## Regenerar
`python3 generar-logo.py` (necesita `fonttools`, `cairosvg` y `plex.ttf`).

## Sobre Canva
Estos SVG se importan en Canva con *Subir archivo* y quedan vectoriales. Se
entrega en SVG y no como diseño de Canva porque el vector escala sin pérdida,
sirve de favicon, pesa unos pocos kilobytes y es de su propiedad sin depender
de una cuenta ajena.
