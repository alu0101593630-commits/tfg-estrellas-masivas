# TFG: Técnicas matemáticas en el estudio espectroscópico de estrellas masivas

**Autora:** Adriana García González  
**Tutor:** Sergio Simón Díaz (Instituto de Astrofísica de Canarias)  
**Titulación:** Grado en Matemáticas — Universidad de La Laguna  
**Curso:** 2025-2026

---

## Descripción

Este repositorio contiene el código y los datos generados en el Trabajo Fin de Grado, cuyo objetivo es desarrollar una metodología matemática para la normalización del continuo espectral y el ajuste de perfiles de líneas de absorción en una muestra de 159 estrellas masivas de tipo B y A temprana de la Vía Láctea.

Los espectros de alta resolución proceden del repositorio público SPECTRA del Instituto de Astrofísica de Canarias, obtenidos con el espectrógrafo HERMES del Telescopio Mercator (La Palma, España).

---

## Contenido del repositorio

### Notebooks

| Archivo | Descripción |
|--------|-------------|
| `Normal_cont_FINAL.ipynb` | Normalización del continuo espectral mediante el motor híbrido de sustitución iterativa basado en splines cúbicas |
| `Análisis_FINAL.ipynb` | Ajuste interactivo de perfiles de absorción (pseudo-Voigt y rotacional) sobre las líneas diagnósticas |
| `Compara_espectros.ipynb` | Visualización comparativa de espectros a lo largo de la secuencia espectral B |
| `Gráficas_clasif.ipynb` | Generación de las figuras de clasificación espectral del Capítulo 4 |

### Datos

Los ficheros `.csv` contienen los valores de anchura equivalente (EW) y anchura a media altura (FWHM) obtenidos para las cuatro líneas diagnósticas analizadas:

| Archivo | Línea |
|--------|-------|
| `linea_4387.csv` | He I λ4387 Å |
| `linea_4481.csv` | Mg II λ4481 Å |
| `linea_4860.csv` | Hβ λ4860 Å |
| `linea_8598.csv` | Paschen 14 λ8598 Å |

---

## Líneas diagnósticas analizadas

- **He I λ4387 Å** — diagnóstico de subtipo espectral (temperatura efectiva)
- **Mg II λ4481 Å** — diagnóstico de subtipo espectral (temperatura efectiva)
- **Hβ λ4860 Å** — diagnóstico de clase de luminosidad (gravedad superficial)
- **Paschen 14 λ8598 Å** — diagnóstico de clase de luminosidad en el infrarrojo cercano

---

## Requisitos

```python
numpy
scipy
astropy
pandas
matplotlib
```

---

## Uso

1. Descargar los espectros FITS desde el repositorio SPECTRA del IAC:  
   https://cloud.iac.es/index.php/s/kFYEk3xPqByX82F

2. Ejecutar `Normal_cont_FINAL.ipynb` para normalizar el continuo de cada espectro.

3. Ejecutar `Análisis_FINAL.ipynb` para ajustar las líneas de absorción de forma interactiva.

4. Ejecutar `Compara_espectros.ipynb` y `Gráficas_clasif.ipynb` para reproducir las figuras del trabajo.

---

## Licencia

Este repositorio es de acceso público con fines académicos.
