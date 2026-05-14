# Hidden Markov Model (HMM) aplicado a Mantenimiento Predictivo

## Descripción del proyecto

Este proyecto implementa un Modelo Oculto de Markov (Hidden Markov Model - HMM) para simular un sistema de mantenimiento predictivo industrial.

El modelo permite representar el comportamiento de una máquina industrial mediante estados ocultos y observaciones visibles obtenidas a partir de sensores de vibración.

La simulación permite:

- Detectar desgaste progresivo.
- Inferir estados ocultos de la maquinaria.
- Generar alertas tempranas.
- Calcular métricas industriales.
- Estimar vida útil restante (RUL).

El proyecto fue desarrollado en Python y es compatible con Google Colab.

---

# Objetivo

Aplicar distribuciones de probabilidad y cadenas de Markov para implementar un Modelo Oculto de Markov que permita simular el comportamiento operativo de una máquina industrial y detectar posibles fallas mediante análisis de vibraciones.

---

# Modelo utilizado

El sistema utiliza un Hidden Markov Model compuesto por:

## Estados ocultos

- Estado Normal
- Estado de Desgaste
- Estado de Falla

## Observaciones

- Vibración Baja
- Vibración Media
- Vibración Alta

---

# Componentes probabilísticos

## Distribución inicial

```python
pi = [0.8, 0.15, 0.05]
Matriz de transición
A = [
    [0.85, 0.13, 0.02],
    [0.30, 0.50, 0.20],
    [0.05, 0.15, 0.80]
]
Matriz de emisión
B = [
    [0.80, 0.15, 0.05],
    [0.30, 0.50, 0.20],
    [0.10, 0.30, 0.60]
]
Tecnologías utilizadas
Python 3
NumPy
Matplotlib
Pandas
Google Colab
Funcionalidades principales

El sistema implementa:

Simulación de estados ocultos.
Generación de observaciones.
Algoritmo de Viterbi.
Dashboard de monitoreo.
Alertas automáticas.
Cálculo de:
MTBF
RUL
Riesgo financiero
Estructura del proyecto
📁 proyecto-hmm/
│
├── main.ipynb
├── main.py
├── README.md
├── requirements.txt
└── resultados/
    ├── dashboard.png
    └── simulacion.png
Instalación y ejecución
Opción 1: Google Colab
Abrir Google Colab.
Crear un nuevo notebook.
Copiar el código del proyecto.
Ejecutar todas las celdas.
Opción 2: Ejecución local
Instalar dependencias
pip install numpy matplotlib pandas
Ejecutar el programa
python main.py
Resultados esperados

El sistema genera:

Dashboard gráfico de vibraciones.
Estados ocultos simulados.
Alertas de mantenimiento.
Reporte de salud de la maquinaria.
Métricas predictivas industriales.
Ejemplo de salida

El programa muestra:

Estado actual inferido.
Tiempo medio entre fallas.
Vida útil restante.
Número de alertas.
Riesgo financiero.

Además, genera un gráfico de monitoreo industrial.

Aplicaciones reales

Este modelo puede aplicarse en:

Industria manufacturera.
Monitoreo de motores.
Sistemas industriales IoT.
Mantenimiento predictivo.
Análisis de vibraciones.
Autor

Jorge Paniagua

Licencia

Proyecto académico con fines educativos.
