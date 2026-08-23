<div align="center">

# Curso teórico práctico sobre inversión geofísica en Python

### Del dato observado al modelo del subsuelo

**Gravimetría · Magnetometría · MT 1D · FWI · SimPEG · Aprendizaje profundo guiado por física**

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![SimPEG](https://img.shields.io/badge/SimPEG-0.25.2-23395B)](https://simpeg.xyz/)
[![Course](https://img.shields.io/badge/curso-teórico--práctico-19A7CE)](#ruta-científica)
[![YouTube](https://img.shields.io/badge/ver-clases_en_YouTube-FF0000?logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=gAqL1yqmJJw&list=PLBrkSquHNyNM)

</div>

<p align="center"><em>Un laboratorio reproducible para explorar la relación</em></p>

$$
\mathbf{d} = \mathcal{F}(\mathbf{m}) + \boldsymbol{\varepsilon}
$$

<p align="center"><em>y reconstruir modelos físicos con ajuste de datos, regularización y aprendizaje profundo.</em></p>

![Mapa visual del curso](docs/assets/course-map.png)

## Qué encontrarás

Este repositorio reúne los materiales del **Curso teórico práctico sobre inversión geofísica en Python**, dirigido a la comunidad científica. Integra fundamentos del problema inverso con ejercicios guiados, casos sintéticos y datos reales.

El curso fue dirigido por **Ana Mantilla, Javier Torres y León Suárez**, con **PhD Henry Arguello Fuentes** como investigador principal. Fue organizado por los grupos de investigación **HDSP, GIGBA y CPS** en el marco del **Contrato No. 045-2025**, financiado por el Ministerio de Ciencia, Tecnología e Innovación (MINCIENCIAS) y la **Agencia Nacional de Hidrocarburos (ANH)**.

### Desarrollo del material

Los materiales de este repositorio, incluyendo los **códigos, notebooks y ejercicios prácticos**, fueron desarrollados por:

- **Adrián Pérez-Montejo**, Geólogo
- **Kevin Tarazona**, BSc (c)

La autoría anterior corresponde al desarrollo del material disponible en este repositorio. Las personas encargadas de la dirección y dictado del curso se reconocen en la sección institucional correspondiente.

## Ruta científica

| Sesión | Eje | Del dato al modelo | Material | Video |
|:--:|---|---|:--:|:--:|
| 01 | Fundamentos | No unicidad, sensibilidad, incertidumbre y regularización | [Abrir](materials/session-01/) | [▶ Ver sesión](https://www.youtube.com/watch?v=gAqL1yqmJJw&list=PLBrkSquHNyNM&index=1) |
| 02 | Gravimetría 3D | Anomalía residual → contraste de densidad | [Abrir](materials/session-02/) | [▶ Ver sesión](https://www.youtube.com/watch?v=Yf4zvhu8cIk&list=PLBrkSquHNyNM&index=2) |
| 03 | Magnetometría 3D | Anomalía TMI → susceptibilidad magnética | [Abrir](materials/session-03/) | *No publicado* |
| 04 | MT 1D guiada por física | Impedancia Z<sub>xy</sub> → resistividad por capas | [Abrir](materials/session-04/) | [▶ Ver sesión](https://www.youtube.com/watch?v=SriI-fnhWYc&list=PLBrkSquHNyNM&index=3) |
| 05 | FWI: fundamentos | Registros sísmicos → modelo de velocidad | [Abrir](materials/session-05/) | [▶ Ver sesión](https://www.youtube.com/watch?v=zWDQ6DE8mWs&list=PLBrkSquHNyNM&index=4) |
| 06 | FWI: entrenamiento | *Shots* y pesos preentrenados → velocidad de onda P | [Abrir](materials/session-06/) | [▶ Ver sesión](https://www.youtube.com/watch?v=zzUrBL7tILg&list=PLBrkSquHNyNM&index=5) |
| 07 | Reto integrador MT 1D | Datos sintéticos → inversión profunda no supervisada | [Abrir](materials/session-07/) | *No publicado* |

> **Disponibilidad de videos:** la playlist pública contiene actualmente las grabaciones de las sesiones 1, 2, 4, 5 y 6. Esta tabla puede actualizarse cuando se publiquen las sesiones restantes.

## Arquitectura conceptual

<p align="center">
  <img src="docs/assets/architecture-conceptual.svg" width="100%" alt="Animación futurista de la arquitectura de inversión geofísica guiada por física e inteligencia artificial">
</p>

La inversión se plantea como un **ciclo iterativo y auditable**: los datos observados y la hipótesis física alimentan el operador directo; la discrepancia entre datos predichos y observados se combina con regularización y conocimiento previo; el modelo se actualiza hasta alcanzar convergencia, y finalmente se evalúan resolución, incertidumbre y coherencia geológica.

## Clases grabadas

<div align="center">

### ▶️ [Ver la lista de reproducción completa en YouTube](https://www.youtube.com/watch?v=gAqL1yqmJJw&list=PLBrkSquHNyNM)

[![Modelos 3D del subsuelo e inteligencia artificial: vista previa de las clases](docs/assets/youtube-course-preview.png)](https://www.youtube.com/watch?v=zWDQ6DE8mWs&list=PLBrkSquHNyNM&index=4&t=112s)

*Revisa las sesiones en orden y utiliza los notebooks de este repositorio como laboratorio práctico.*

</div>

## Inicio rápido

```bash
git clone https://github.com/Anagabrielamantilla/inversion-geofisica-python.git
cd inversion-geofisica-python
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
jupyter lab
