# Tesis: Análisis de Algoritmos de Machine Learning para Predicción de Aceleraciones Sísmicas Máximas en México

## Objetivos
El propósito principal de esta tesis fue evaluar y optimizar algoritmos de machine learning para predecir aceleraciones sísmicas máximas en México. Esto incluye:
- Comparar el desempeño de distintos algoritmos.
- Identificar el modelo que mejor representa los datos sísmicos del país.
- Proponer soluciones aplicables para mejorar la preparación frente a eventos sísmicos.

## Metodología
1. **Recopilación de datos**:
   - Se utilizaron registros sísmicos provenientes de diversas instituciones, como el Instituto de Ingeniería UNAM y el CIRES, con un total de 2710 registros.
2. **Preprocesamiento**:
   - Transformación de escalas de magnitud sísmica a una escala unificada (`Mw`).
   - Análisis estadístico y normalización de datos.
3. **Implementación de modelos**:
   - Algoritmos lineales: Regresión lineal, regresión de cresta.
   - Métodos de conjunto: Bosques aleatorios, XGBoost.
   - Reducción de dimensionalidad: PCA y PLS.
4. **Evaluación**:
   - Métricas como el error cuadrático medio (MSE) y el coeficiente de determinación (`R^2`) fueron utilizadas para medir el desempeño.

## Resultados
- El modelo **XGBoost** mostró un desempeño superior con una precisión del **75.8%** en la predicción de aceleraciones sísmicas.
- Se realizaron simulaciones para evaluar escenarios hipotéticos de sismos en México, mostrando resultados coherentes con los datos históricos.

## Cómo utilizar este repositorio
1. **Clonar el repositorio**:
   ```
   git clone https://github.com/JOchoa51/tesis_geofisica.git
   ```
2. **Instalar las dependencias**:
   Instala los paquetes necesarios desde `requirements.txt`:
   ```
   pip install -r requirements.txt
   ```
3. **Estructura del proyecto**:
   - ``Datos y resultados/``: Contiene datos de entrada y resultados finales
   - ``Modelos entrenados/``: Modelos entrenados en formato `.pkl`, listos para usar.
   - ``Modelos con Vs30/``: Modelos entrenados en formato `.pkl`, listos para usar, especiales para simulación de eventos.

4. **Entrenamiento del modelo**:
   Ejecuta el Jupyter Notebook llamado `FINAL_Resultados.ipynb` y sigue la estructura del archivo.

## Requisitos
- Python 3.8+
- Librerías: `xgboost`, `pandas`, `numpy`, `matplotlib`, `scikit-learn`.

## Créditos
Este trabajo fue realizado por **Jesús Ochoa Contreras** como parte del programa de Ingeniería Geofísica en la UNAM. Para dudas o colaboración, contáctame en: **ochoacontrerasjesus8@gmail.com**.

## Licencia
Este repositorio está bajo la Licencia MIT. Si utilizas este trabajo, por favor da el crédito correspondiente.

¡Gracias por tu interés!
