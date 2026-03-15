# Foco — Tema para Typora

Un tema de escritura diseñado para sesiones largas. Sin distracciones visuales, sin fatiga ocular. Solo el texto.

Disponible en modo claro y oscuro.

---

## Vista previa

| Modo claro | Modo oscuro |
|---|---|
| Fondo marfil cálido `#F5F1EB` | Fondo carbón cálido `#1A1916` |
| Texto marrón oscuro `#27211C` | Texto beige apagado `#DDD8CF` |
| Acento verde musgo `#4D7A65` | Acento verde musgo `#6BA88E` |

> Las capturas de pantalla se encuentran en la carpeta `/screenshots`.

---

## Filosofía de diseño

**Foco** nace de un principio simple: un buen tema de escritura debe desaparecer.

Cada decisión de diseño responde a criterios de ergonomía visual para uso diario:

- **Paleta cálida en ambos modos** — elimina la fatiga que genera el blanco frío o el negro puro en sesiones largas.
- **Contraste calibrado al 85%** — suficiente para leer con claridad, insuficiente para producir vibración visual (*halation*).
- **Ancho de línea limitado a 720px** — entre 60 y 75 caracteres por línea, el rango óptimo para el movimiento horizontal del ojo.
- **Interlineado 1.75** — más aire que el estándar web, mejor ritmo de lectura en bloques largos.
- **Tamaño base 17px** — el estándar de 16px viene de los años 90; las pantallas modernas exigen más.
- **Un solo color de acento** — verde musgo, usado con moderación. Nada compite con el texto.

---

## Fuentes

Foco utiliza exclusivamente:

| Rol | Fuente |
|---|---|
| Prosa y UI | [Segoe UI](https://learn.microsoft.com/en-us/typography/font-list/segoe-ui) |
| Código | [JetBrains Mono](https://www.jetbrains.com/lp/mono/) |

**Segoe UI** viene preinstalada en Windows. En macOS y Linux se recomienda instalarla manualmente o dejar que el sistema use su sans-serif de sistema como fallback.

**JetBrains Mono** es gratuita y de código abierto. Descarga en [jetbrains.com/lp/mono](https://www.jetbrains.com/lp/mono/) o instala vía tu gestor de paquetes.

---

## Instalación

### Método 1 — Manual

1. Descarga `foco-light.css` y/o `foco-dark.css` desde este repositorio.
2. Abre Typora y ve a `Preferencias → Apariencia → Abrir carpeta de temas`.
3. Copia los archivos `.css` en esa carpeta.
4. Reinicia Typora.
5. Ve a `Preferencias → Apariencia` y selecciona **Foco Light** o **Foco Dark** en el menú desplegable.

### Método 2 — Clonar el repositorio

```bash
# macOS
git clone https://github.com/tu-usuario/foco-typora ~/Library/Application\ Support/abnerworks.Typora/themes/foco

# Windows
git clone https://github.com/tu-usuario/foco-typora %APPDATA%\Typora\themes\foco

# Linux
git clone https://github.com/tu-usuario/foco-typora ~/.config/Typora/themes/foco
```

Luego reinicia Typora y selecciona el tema en preferencias.

---

## Estructura del repositorio

```
foco-typora/
├── foco-light.css
├── foco-dark.css
├── screenshots/
│   ├── light-preview.png
│   └── dark-preview.png
└── README.md
```

---

## Elementos estilizados

| Elemento | Decisión de diseño |
|---|---|
| `h1` | Peso ligero (300), borde inferior en acento apagado |
| `h2` | Peso normal (400), borde inferior sutil |
| `h5` | Versalitas + espaciado de letras, rol de etiqueta |
| Listas `ul` | Bullet `–` en lugar del disco estándar |
| `blockquote` | Borde izquierdo en acento, fondo levemente diferenciado |
| `code` inline | Fondo cálido, color acento, borde sutil |
| Bloque `pre` | Borde izquierdo en acento, fuente mono con ligaduras |
| `hr` | Línea delgada con decoración `· · ·` centrada |
| Tablas | Sin bordes agresivos, cabeceras en versalitas |
| Scrollbar | 6px, invisible por defecto, aparece en hover |
| Selección | Color derivado del acento, no el azul del sistema |
| Task lists | Checkbox personalizado con check en color acento |

---

## Personalización

Todas las variables de diseño están centralizadas en el bloque `:root` al inicio de cada archivo.

```css
:root {
  --bg-primary:    #F5F1EB;   /* Color de fondo */
  --text-primary:  #27211C;   /* Color de texto */
  --accent:        #4D7A65;   /* Color de acento */
  --max-width:     720px;     /* Ancho del área de escritura */
  --text-base:     17px;      /* Tamaño de fuente base */
  --line-height:   1.75;      /* Interlineado */
}
```

---

## Compatibilidad

Probado en **Typora 1.x**. No compatible con versiones anteriores a `0.11`.

| Sistema | Estado |
|---|---|
| Windows 10/11 | ✓ Recomendado (Segoe UI nativa) |
| macOS 12+ | ✓ Funcional (Segoe UI requiere instalación) |
| Linux | ✓ Funcional (Segoe UI requiere instalación) |

---

## Licencia

MIT — libre para usar, modificar y distribuir.

---

## Créditos

Diseñado con criterios de ergonomía visual para escritura de larga duración.  
Fuentes: [Segoe UI](https://learn.microsoft.com/en-us/typography/font-list/segoe-ui) (Microsoft) · [JetBrains Mono](https://www.jetbrains.com/lp/mono/) (JetBrains, OFL).
