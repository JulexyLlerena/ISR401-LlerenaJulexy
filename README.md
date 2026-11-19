# ISR-401 · EV-PRAC-01 — Transcripción fiel (caso FRÍOVAC)

Repositorio personal de Llerena Abril Angelina Julexy.

`EV-PRAC-01/main.tex` es la guía-rúbrica del docente con la transcripción fiel de la prueba escrita a mano el 18 de noviembre de 2026, debajo de cada tarea respondida (T1 y T2). Las fotografías de las hojas están en `EV-PRAC-01/evidencias/` (`hoja-01.jpg` a `hoja-04.jpg`) y se incluyen en el anexo del PDF. El documento se elaboró y compiló en Overleaf.

## Estructura

```
ISR401-LlerenaJulexy/
├── README.md
└── EV-PRAC-01/
    ├── main.tex          archivo principal
    ├── referencias.bib   referencias de la guía (natbib, estilo unsrtnat)
    ├── main.pdf          PDF compilado
    ├── figuras/          logoband.png (logo de la portada)
    └── evidencias/       hoja-01.jpg, hoja-02.jpg, hoja-03.jpg, hoja-04.jpg
```

## Cómo compilar en Overleaf

Configuración que debe tener el proyecto:

| Opción de Overleaf (Menú) | Valor |
|---|---|
| Compiler | pdfLaTeX |
| Main document | main.tex |
| TeX Live version | 2024 o la más reciente |

No se necesita instalar nada: todos los paquetes (inputenc, fontenc, helvet, geometry, graphicx, array, tabularx, longtable, pdflscape, colortbl, xcolor, enumitem, fancyhdr, lastpage, tcolorbox, amsmath, natbib, url, needspace, caption, hyperref) vienen incluidos en Overleaf.

### Pasos

1. En este repositorio de GitHub, pulsar el botón verde **Code → Download ZIP** y descomprimir el archivo.
2. Entrar a la carpeta `EV-PRAC-01` y comprimir su contenido (`main.tex`, `referencias.bib` y las carpetas `figuras` y `evidencias`) en un nuevo archivo `.zip`.
3. En Overleaf: **New Project → Upload Project** y subir ese `.zip`.
4. Abrir **Menú** (arriba a la izquierda) y comprobar que **Compiler** sea `pdfLaTeX` y **Main document** sea `main.tex`.
5. Pulsar **Recompilar**. Overleaf genera el PDF con la bibliografía: ejecuta pdfLaTeX y BibTeX automáticamente (estilo `unsrtnat`, definido en `main.tex`).

### Si algo falla

- **`File 'figuras/logoband.png' not found`:** la carpeta `figuras` debe quedar al mismo nivel que `main.tex`, con los nombres en minúsculas.
- **No se encuentran las imágenes del anexo:** la carpeta `evidencias` debe quedar al mismo nivel que `main.tex` y contener `hoja-01.jpg` a `hoja-04.jpg`.
- **Las referencias salen como [?]:** pulsar Recompilar otra vez, o en la flecha junto a Recompilar elegir **Recompile from scratch**.
- **Error con XeLaTeX o LuaLaTeX:** cambiar Compiler a `pdfLaTeX` en el Menú.

## Compilar en una computadora (alternativa)

Con TeX Live 2024 o posterior (o MiKTeX), desde la carpeta del repositorio clonado:

```
cd EV-PRAC-01
pdflatex main
bibtex main
pdflatex main
pdflatex main
```
