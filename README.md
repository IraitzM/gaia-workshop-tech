# GAIA Workshop

Repositorio de materiales, diapositivas y cuadernos prácticos para la formación tecnológica de **GAIA**, orientada a computación cuántica práctica y formulación de problemas de optimización combinatoria.

## 📚 Cuadernos interactivos (Notebooks)

Puedes abrir y ejecutar directamente cualquiera de los cuadernos en Google Colab haciendo clic en sus insignias correspondientes:

### Sesión 2: Del Portátil a la QPU

#### Bloque 2.1: Acceso y Envío a QPUs Reales y Emuladores

| Cuaderno | Descripción | Colab |
|---|---|:---:|
| **`01-ibm-submission.ipynb`** | Creación, simulación y envío de circuitos cuánticos a procesadores superconductores de **IBM Quantum**. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/01-del-portatil-a-la-qpu/notebooks/01-ibm-submission.ipynb) |
| **`02-iqm-ionq-submission.ipynb`** | Configuración y envío de trabajos a plataformas cuánticas comerciales (**IQM Resonance** e **IonQ Cloud**). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/01-del-portatil-a-la-qpu/notebooks/02-iqm-ionq-submission.ipynb) |
| **`03-aquila-submission.ipynb`** | Simulación analógica de Hamiltonianos (AHS) y problema del conjunto independiente máximo (MIS) en **QuEra Aquila** (átomos neutros vía AWS Braket). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/01-del-portatil-a-la-qpu/notebooks/03-aquila-submission.ipynb) |

#### Bloque 2.2: Formulación QUBO y Optimización Combinatoria

| Cuaderno | Descripción | Colab |
|---|---|:---:|
| **`04-qubo-portfolio-optimization.ipynb`** | **Optimización de Carteras (Finanzas):** Selección óptima de activos (Markowitz) con `PyQUBO`, balanceando retorno, riesgo de covarianza y restricciones de presupuesto mediante penalizaciones cuadráticas. Resolución con `dimod.ExactSolver` y `neal.SimulatedAnnealingSampler`. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/01-del-portatil-a-la-qpu/notebooks/04-qubo-portfolio-optimization.ipynb) |
| **`05-qubo-max-cut.ipynb`** | **Corte Máximo en Grafos (Max-Cut):** Particionado de nodos en dos conjuntos disjuntos. Deducción analítica de la matriz $Q$, simetría de espín $Z_2$, estados fundamentales degenerados y visualización con NetworkX y Matplotlib. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/01-del-portatil-a-la-qpu/notebooks/05-qubo-max-cut.ipynb) |
| **`06-qubo-tsp.ipynb`** | **Viajante de Comercio (Logística - TSP 4 Nodos):** Ruta cíclica óptima entre ciudades ($A, B, C, D$). Matriz de variables $x_{v, t}$ ($16$ variables binarias), restricciones *One-Hot*, multiplicadores de Lagrange, resolución con cálculo exacto y Neal, y reducción por *Gauge Fixing*. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/01-del-portatil-a-la-qpu/notebooks/06-qubo-tsp.ipynb) |
