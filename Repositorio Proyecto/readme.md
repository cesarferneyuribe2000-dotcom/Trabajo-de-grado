# Simulación de Emisiones Vehiculares - AMB

Este repositorio contiene el código desarrollado para la simulación de emisiones del parque automotor del Área Metropolitana de Bucaramanga (AMB), como parte del trabajo de grado:

**Formulación de estrategias de movilidad sostenible para el AMB basadas en la simulación de escenarios de emisiones**

## Descripción

El proyecto utiliza Python y el modelo COPERT para estimar las emisiones de:

- CO
- CO₂
- PM₂.₅

El análisis considera la evolución histórica y proyectada del parque automotor, así como diferentes escenarios de penetración de vehículos eléctricos para el periodo 2025–2030.

## Metodología

El flujo general del código comprende:

1. Procesamiento de información del parque automotor.
2. Estimación de tasas de crecimiento por categoría vehicular.
3. Proyección del parque automotor hasta 2030.
4. Modelación de la permanencia vehicular mediante una distribución Weibull.
5. Configuración de las categorías vehiculares en COPERT.
6. Estimación de emisiones para el escenario tendencial.
7. Simulación de escenarios de penetración de vehículos eléctricos.
8. Cálculo de las emisiones evitadas.
9. Generación de tablas y figuras para el análisis de resultados.

## Categorías vehiculares

El análisis considera las siguientes categorías:

- Automóvil
- Camioneta
- Bus
- Buseta
- Microbús
- Motocicleta

## Escenarios de vehículos eléctricos

Se evaluaron tres niveles de penetración de vehículos eléctricos para 2030:

| Escenario | Penetración EV |
|---|---:|
| EV 0.01% | 0.01% |
| EV 0.05% | 0.05% |
| EV 0.1% | 0.1% |

Estos escenarios se utilizan como escenarios analíticos de baja penetración para evaluar el efecto de la electrificación sobre las emisiones directas del transporte.

## Requisitos

Python 3.x

Principales librerías utilizadas:

```text
pandas
numpy
matplotlib
scipy
openpyxl