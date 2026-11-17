# Lógica difusa y algoritmos genéticos

Prácticas de la materia de **Deep Learning** (segundo parcial) sobre **lógica difusa** y **algoritmos genéticos**, implementados desde cero con NumPy, sin librerías especializadas.

**Tecnologías:** Python, NumPy, pandas y Matplotlib.

## Lógica difusa

| # | Notebook | Qué hace |
|---|---|---|
| 01 | `01_Funciones_pertenencia_temperatura.ipynb` | Funciones de pertenencia triangulares para clasificar una temperatura en tres conjuntos difusos. |
| 02 | `02_Funciones_pertenencia_velocidad.ipynb` | Lo mismo aplicado a velocidad (km/h). |
| 03 | `03_Temperatura_y_humedad.ipynb` | Calcula los grados de pertenencia de temperatura y humedad para plantear reglas difusas que combinan ambas variables. |

## Algoritmos genéticos

Los tres usan selección por **torneo binario**, **cruce** y **mutación**, programados a mano.

| # | Notebook | Problema | Resultado en datos de prueba |
|---|---|---|---|
| 04 | `04_AG_Clasificacion_mamografia.ipynb` | Clasificar masas en mamografías como benignas o malignas. El cromosoma son los pesos y el sesgo de un clasificador logístico y el fitness es el F1-score. | Exactitud 81.9 %, F1 0.826 |
| 05 | `05_AG_Cancer_Wisconsin.ipynb` | El mismo enfoque con el dataset de cáncer de mama de Wisconsin (30 características). | Exactitud 99.1 %, F1 0.988 |
| 06 | `06_AG_Dieta_optima.ipynb` | Encontrar la dieta más barata que cumpla calorías (1,800 a 2,200 kcal), proteína, carbohidratos y grasa, usando penalizaciones. | Costo final: 179 unidades |

## Datos

En la carpeta `datos/`:
- `mammographic_masses.data`: Mammographic Mass dataset (UCI Machine Learning Repository).
- `wdbc.data`: Breast Cancer Wisconsin (Diagnostic) dataset (UCI Machine Learning Repository).

**Nota:** son ejercicios académicos para aprender los algoritmos, no herramientas de diagnóstico médico.
