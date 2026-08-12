[README (1).md](https://github.com/user-attachments/files/30967200/README.1.md)
# Prueba Práctica — Unidad IV — Ingeniería de Requisitos (ISR-401)

**Estudiante:** Barrionuevo Carlos
**Asignatura:** Ingeniería de Requisitos (ISR-401)
**Docente:** Ing. Gleiston Guerrero, Mg.
**Caso:** Sistema de Gestión de Pedidos

## Estructura del repositorio

```
.
├── Archivo_Principal.tex     # Archivo principal LaTeX (carátula + P1-P10)
├── Archivo_Principal.pdf     # PDF compilado (versión de referencia)
├── diagrama_clases.png       # Diagrama de clases UML (P1)
├── Diagrama_Actividad.png    # Diagrama de actividades UML (P2)
├── Diagrama_Estados.png      # Máquina de estados UML (P3)
├── captura_evaluacion.png    # Captura del cuestionario (resumen + intento) del SGA
└── README.md                 # Este archivo
```

No se usa archivo `.bib`: el documento no incluye citas bibliográficas propias
(las referencias del enunciado pertenecen al documento de la prueba, no a
este entregable).

## Requisitos previos

- Distribución LaTeX con **TeX Live** (o equivalente, p. ej. MiKTeX).
- Compilador **pdflatex**.
- Paquete de idioma español para `babel`:
  - En TeX Live: `texlive-lang-spanish`
  - En MiKTeX se instala automáticamente al compilar (o vía el MiKTeX Console).
- Paquetes estándar (incluidos en cualquier instalación completa de TeX Live):
  `babel`, `amsmath`, `geometry`, `booktabs`, `array`, `longtable`,
  `enumitem`, `hyperref`, `graphicx`, `caption`.

## Instrucciones de compilación

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/cdxniel/Evaluaci-n-Pr-ctica-de-la-Unidad-IV.git
   cd Evaluaci-n-Pr-ctica-de-la-Unidad-IV
   ```
2. Compilar con `pdflatex`. **Debe ejecutarse dos veces** para que el índice
   de contenidos (`\tableofcontents`) y las referencias internas se generen
   correctamente:
   ```bash
   pdflatex -interaction=nonstopmode Archivo_Principal.tex
   pdflatex -interaction=nonstopmode Archivo_Principal.tex
   ```
3. El PDF resultante se genera como `Archivo_Principal.pdf` en la misma
   carpeta.

### Archivo principal

`Archivo_Principal.tex`

### Dependencias de archivos

`Archivo_Principal.tex` incluye las siguientes imágenes mediante
`\includegraphics`, por lo que deben estar presentes en la **misma carpeta**
al compilar (si falta alguna, la compilación fallará):

- `diagrama_clases.png`
- `Diagrama_Actividad.png`
- `Diagrama_Estados.png`
- `captura_evaluacion.png`

## Notas

- Si se desea recompilar desde cero, se recomienda eliminar antes los
  archivos auxiliares (`Archivo_Principal.aux`, `Archivo_Principal.toc`,
  `Archivo_Principal.out`, `Archivo_Principal.log`) para evitar advertencias
  de `rerunfilecheck`.
- Los nombres de archivo distinguen mayúsculas/minúsculas en sistemas
  Linux/macOS; respetar exactamente la capitalización indicada arriba.
