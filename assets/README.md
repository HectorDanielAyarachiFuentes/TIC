# Assets del Portal CURZA-STIC

Esta carpeta contiene todos los recursos visuales y vectoriales utilizados en el portal interactivo de simuladores **CURZA STIC**.

## 🎨 Iconografía SVG (`assets/icons/`)

Todos los emojis y glifos antiguos fueron reemplazados por **iconos vectoriales SVG de alta definición** provenientes del paquete profesional [`lucide-static`](https://lucide.dev) (v1.52.0).

### Características Técnicas:
- **Formato**: SVG 24x24 estándar, trazo `stroke-width="2"`, bordes redondeados (`stroke-linecap="round" stroke-linejoin="round"`).
- **Herencia de Color Dinámico**: Utilizan `stroke="currentColor"`, lo que permite que cada icono herede automáticamente la paleta de colores de su respectiva categoría (`--c-dron`, `--c-robot`, `--c-iot`, `--c-ia`, etc.) y se adapte al modo oscuro sin artifacts ni desfases de contraste.
- **Rendimiento Offline y Cero Latencia**: Los iconos de la interfaz principal (`index.html`) están embebidos directamente como SVGs inline (`class="ico-svg"`), garantizando que el portal funcione 100% offline, incluso abriendo el archivo localmente con `file:///` sin problemas de CORS ni solicitudes de red.
- **Colección Disponible**: 72 iconos SVG listos para usar en nuevos simuladores, módulos y controles de interfaz (incluyendo controles del visor: `maximize-2`, `minimize-2`, `external-link`, `x`, `eye`, `expand`, `shrink`).

### Cómo agregar nuevos iconos:
1. Instalar o consultar el paquete:
   ```bash
   npm i -D lucide-static
   ```
2. Copiar el archivo `.svg` deseado desde `node_modules/lucide-static/icons/<nombre>.svg` hacia `assets/icons/`.
3. Para usarlo en una tarjeta o sección:
   ```html
   <span class="card-ico">
     <svg class="ico-svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
       <!-- paths del icono -->
     </svg>
   </span>
   ```
