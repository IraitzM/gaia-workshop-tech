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

### Sesión 3: De la Formulación a la Optimización Cuántica

Iremos construyendo poco a poco la noción de cómo aporta la cuántica al mundo de la optimización con el objetivo de comprender mejor comparativas como las del [QOBLIB](https://zib-aopt.github.io/QOBLIB/index.html) de [IBM](https://www.ibm.com/quantum/blog/qoblib).

| Cuaderno | Descripción | Colab |
|---|---|:---:|
| **`01-annealing-maxcut.ipynb`** | **Annealing y otros solvers (Max-Cut):** Mismo QUBO de la sesión anterior. Referencia exacta, recocido simulado con `neal`, evolución adiabática ideal con QuTiP, bifurcación simulada y Fujitsu Digital Annealer vía DADK. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/02-optimizacion-cuantica/notebooks/01-annealing-maxcut.ipynb) |
| **`02-qaoa-maxcut.ipynb`** | **QAOA desde cero (Max-Cut):** El mismo QUBO como circuito construido puerta a puerta. Funciones de *scheduling*, annealing digitalizado, optimización variacional con COBYLA y envío a Aer, IBM e IonQ. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/02-optimizacion-cuantica/notebooks/02-qaoa-maxcut.ipynb) |
| **`03-tsp-anexo.ipynb`** | **Anexo TSP:** Qué cambia cuando hay penalizaciones $P$ y restricciones *one-hot*. Reutiliza la cartera y el TSP de la sesión anterior. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/02-optimizacion-cuantica/notebooks/03-tsp-anexo.ipynb) |
| **`04-vqe-maxcut.ipynb`** | **VQE desde cero (Max-Cut):** El mismo QUBO con ansatz libre *hardware-efficient* (`EfficientSU2`). Principio variacional, optimización con COBYLA y cara a cara con QAOA. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/02-optimizacion-cuantica/notebooks/04-vqe-maxcut.ipynb) |
| **`05-vqe-ionq-simulator.ipynb`** | **VQE en IonQ (Max-Cut):** El circuito VQE óptimo muestreado en el `ionq_simulator`. Ansatz hardware-efficient, comparativa Aer frente a IonQ y bucle completo opcional. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/02-optimizacion-cuantica/notebooks/05-vqe-ionq-simulator.ipynb) |

### Sesión 4: Aprender con Qubits (Aprendizaje Cuántico)

El aprendizaje automático, machine learning o inteligencia artificial son conceptos que no son ajenos a la cuántica. En esta sesión exploraremos qué nos aporta la cuántica a todo esto.

| Cuaderno | Descripción | Colab |
|---|---|:---:|
| **`01-qsvm-kernels.ipynb`** | **Embedding, kernels y QSVM (iris):** Tres formas de meter números en qubits, kernel de fidelidad *compute-uncompute*, *target alignment* y QSVC con mapas Z y ZZ, también con sQUlearn. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/03-aprendizaje-cuantico/notebooks/01-qsvm-kernels.ipynb) |
| **`02-qnn-vqc.ipynb`** | **QNN y clasificador variacional (iris difícil):** El circuito entero como modelo, mapa YZ_CX y ansatz por capas de sQUlearn, observable medido y comparación contra el kernel fijo. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/03-aprendizaje-cuantico/notebooks/02-qnn-vqc.ipynb) |
| **`03-qrc-squlearn.ipynb`** | **Reservorio cuántico o QRC (lunas y onda):** Reservorio fijo sin entrenar y readout lineal clásico con sQUlearn, para clasificación y regresión con el mismo esquema. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/03-aprendizaje-cuantico/notebooks/03-qrc-squlearn.ipynb) |
| **`04-qsvm-ibm-hardware.ipynb`** | **QSVM en hardware real de IBM:** Versión mini del kernel del cuaderno 01 (264 circuitos en un único job de `SamplerV2`) para que quepa en una QPU, con comparación exacta, Aer e IBM y la factura en circuitos y shots. Requiere API key de IBM Quantum y el envío es opcional. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/03-aprendizaje-cuantico/notebooks/04-qsvm-ibm-hardware.ipynb) |
| **`05-falcondale-sdk-auto.ipynb`** | **QML automático con falcondale-sdk (cáncer de mama):** `Project` perfila y preprocesa el dataset, `assess()` juzga si merece la pena probar QML, la selección de rasgos QUBO recorta 30 rasgos a 4 y `evaluate("auto")` entrena el modelo recomendado (QSVC) frente a la línea de base clásica `svc`. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IraitzM/gaia-workshop-tech/blob/main/03-aprendizaje-cuantico/notebooks/05-falcondale-sdk-auto.ipynb) |
