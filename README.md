# 🛰️ Simuladores TIC · CURZA (UNCo)

Suite modular de experiencias educativas interactivas desarrolladas para aprender jugando: desde pilotaje de drones en cabina FPV y programación por bloques, hasta sistemas IoT con Arduino, laboratorios SIG/QGIS, ciberseguridad e inteligencia artificial.

> **100% Offline & Autocontenido:** Cada simulador corre en el navegador del dispositivo sin necesidad de conexión a internet ni dependencias externas.

---

## 📁 Estructura del Repositorio

El proyecto está organizado de manera modular por ejes temáticos bajo las mejores prácticas de desarrollo web:

```text
curza-stic-main/
├── index.html                   # Portal principal con acceso a todos los simuladores
├── index-codex.html             # Índice alternativo detallado con tags y buscador
├── package.json                 # Metadatos del proyecto y scripts
├── README.md                    # Documentación del proyecto
│
├── simuladores/                 # Módulos interactivos organizados por categoría
│   ├── dron/                    # Vuelo FPV, planificación, misiones, recursos y despiece
│   │   ├── modo-libre.html
│   │   ├── etapa-1.html ... etapa-6.html
│   │   └── dron-despiece.html
│   ├── robotica/                # Programación 3D de brazo robótico por bloques
│   │   └── brazo-bloques.html
│   ├── iot/                     # Banco Arduino, sensores y automatización de viveros
│   │   ├── arduino-banco.html
│   │   ├── arduino-despiece.html
│   │   ├── vivero.html
│   │   └── vivero-automatizado.html
│   ├── meteo/                   # Central meteorológica y estaciones inmersivas
│   │   ├── central-meteo.html
│   │   ├── estacion-meteorologica.html
│   │   └── estacion-meteorologica-gemini.html
│   ├── ofimatica/               # Fundamentos de planillas, fórmulas, datos y maquetación
│   │   ├── calc-1-formulas.html
│   │   ├── calc-2-datos.html
│   │   └── writer-maqueta.html
│   ├── sig-cad/                 # Laboratorios autónomos de teledetección, CAD y GDE
│   │   ├── sig-teledeteccion-autonomo.html
│   │   ├── cad-espacios-verdes-autonomo.html
│   │   ├── simulador-opencad-espacios-verdes.html
│   │   └── gde-circuito-organizacional-autonomo.html
│   ├── bi/                      # Business Intelligence (fuentes, métricas e informes)
│   │   ├── bi-1-fuentes.html
│   │   ├── bi-2-informes.html
│   │   └── bi-3-interactivo.html
│   ├── seguridad/               # Laboratorio de criptografía, 2FA, phishing y firmas
│   │   ├── segu-1-claves.html
│   │   ├── segu-2-cifrado.html
│   │   ├── segu-3-phishing.html
│   │   └── segu-4-firma-certificados.html
│   ├── bd/                      # Taller práctico de modelado de datos y consultas SQL
│   │   ├── bd-1-tablas.html
│   │   ├── bd-2-consultas.html
│   │   └── bd-3-relaciones.html
│   ├── ia/                      # Clasificador, auditoría de sesgos y generador de lenguaje
│   │   ├── ia-1-clasificador.html
│   │   ├── ia-2-sesgo.html
│   │   └── ia-3-generador.html
│   └── moodle/                  # Campus virtual simulado (roles estudiante, docente, admin)
│       ├── moodle-1-estudiante.html
│       ├── moodle-2-docente.html
│       └── moodle-3-admin.html
│
├── sig-teledeteccion-ii/         # Laboratorio SIG II con escenas Sentinel-2 y Landsat
├── resoluciones-ejercicios/     # Material guiado y resoluciones
├── resoluciones-ejercicios-cad/ # Resoluciones paso a paso CAD
└── resoluciones-ejercicios-qgis/# Guías, videos y subtítulos de ejercicios QGIS
```

---

## 🚀 Cómo Ejecutar

### Opción 1: Abrir directamente (Sin instalar nada)
Hacé doble clic en [`index.html`](file:///c:/Users/Ramoncito/Downloads/Dulce/curza-stic-main/index.html) desde el explorador de archivos. Todo funcionará localmente sin necesidad de servidor web.

### Opción 2: Con servidor local de desarrollo
Si tenés Node.js instalado:

```bash
npm start
```

Esto levantará un servidor local rápido para navegar el proyecto.

---

## 🛡️ Directivas y Calidad de Código
Este repositorio implementa directivas de ingeniería estricta y gobernanza:
- **`AGENTS.md` / `.agentrules`**: Directivas operativas de inmutabilidad, no destructividad y zonas protegidas.
- **GitNexus**: Análisis de impacto estructural antes de cada refactorización o cambio crítico.
