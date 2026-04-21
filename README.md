# Carteles accesibles

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-blue)
![Jekyll](https://img.shields.io/badge/Jekyll-Static%20Site-red)
![Markdown](https://img.shields.io/badge/Markdown-Content-lightgrey)
![SCSS](https://img.shields.io/badge/SCSS-Styling-pink)

## Resumen

Sitio web orientado a mejorar la accesibilidad de materiales visuales mediante la publicación de texto alternativo para carteles elaborados a mano en el ámbito educativo.

Los textos se generan inicialmente mediante herramientas de inteligencia artificial y luego se corrigen y estandarizan de forma manual.

Estos contenidos pueden ser leídos por lectores de pantalla, como TalkBack o VoiceOver, accediendo al sitio web a través del escaneo de un código QR vinculado a cada cartel.

El resultado es una plataforma centralizada de textos alternativos asociados a imágenes reales.

De esta manera, las personas que no pueden acceder al contenido visual pueden utilizar un dispositivo móvil para escanear el QR y acceder a una versión textual accesible.

**Herramientas:** GitHub Pages, Jekyll, Markdown, SCSS

## Contexto

Proyecto desarrollado en el marco de iniciativas de accesibilidad digital promovidas por la Dirección de Accesibilidad de la Facultad de Informática, UNLP.

## Descripción

Este proyecto reúne textos alternativos de carteles producidos por estudiantes del Ingreso 2026 de la Facultad de Informática, UNLP.

El flujo de trabajo consiste en:

1. Capturar una imagen del cartel.
2. Generar automáticamente un texto alternativo mediante IA.
3. Revisar y corregir manualmente el contenido.
4. Publicarlo en el sitio web.
5. Generar un código QR que enlace a dicha publicación.

## Estandarización

Se buscó mantener una estructura jerárquica consistente de encabezados en todo el proyecto:

- Un único encabezado H1 por documento.
- Uso consistente de encabezados H2 para secciones principales.

Dado que las descripciones textuales son el eje central del proyecto, se priorizó su jerarquía de la siguiente manera:

- H1: Título del cartel
- H2: Texto transcripto, Descripción de imágenes, Descripción general
- **Negrita**: subtítulos o elementos organizativos dentro del contenido
- [Corchetes]: indicación de contexto o ubicación dentro del cartel

## Estructura de un cartel

```markdown
# Título del cartel

## Descripción de imagen

Texto

## Texto transcripto

[Columna izquierda]

Texto

[Columna derecha]

Texto

## Descripción general

Texto
```

## Estructura del proyecto

```shell
carteles-accesibles
├── assets
│   ├── css
│   │   └── style.scss
│   └── icons
│       ├── favicon.svg
│       └── logo.svg
├── _carteles
│   ├── cartel-01.md
│   ├── cartel-02.md
│   ├── cartel-03.md
│   ├── ...
├── carteles
│   └── index.md
├── _config.yml
├── contacto.md
├── _includes
│   └── head.html
├── index.md
└── README.md
```

