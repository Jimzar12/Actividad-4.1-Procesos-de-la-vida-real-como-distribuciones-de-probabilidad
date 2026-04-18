# Análisis de precipitación diaria

Este proyecto modela la **cantidad de lluvia diaria (mm de precipitación)** en la ciudad de Chihuahua utilizando distribuciones de probabilidad.

Notebook: [Act-4.1.ipynb](./Act-4.1.ipynb)

---

## 1. Proceso seleccionado
Se analiza la cantidad de lluvia diaria durante un periodo de días consecutivos.

## 2. Atributo a medir
La variable medida es la **precipitación diaria en milímetros (mm)**.

## 3. Origen de los datos
Los datos pueden provenir de fuentes públicas como CONAGUA o plataformas como Kaggle.  
Para este análisis se usan entre 30 y 50 observaciones.

## 4. Histograma
El histograma muestra que la mayoría de los días tienen poca o nula lluvia, mientras que pocos días presentan valores altos.

Esto genera una distribución **asimétrica hacia la derecha**, sugiriendo modelos como:
- Exponencial  
- Gamma  

![Histograma](./histograma.png)

## 5. Ajuste de distribución
Se utilizó Python con la librería `fitter` para encontrar el mejor modelo.

**Resultado:** la distribución que mejor se ajusta es la **Gamma**.

## 6. Parámetros de la distribución
- **k (forma):** controla la forma  
- **θ (escala):** controla la dispersión  

Ejemplo:
- k ≈ 1.8  
- θ ≈ 4.2  

## 7. Reflexión
El modelo permite:
- Estimar lluvias intensas  
- Apoyar decisiones agrícolas o urbanas  
- Comparar comportamientos entre regiones o temporadas  

Las distribuciones de probabilidad ayudan a identificar patrones y tomar decisiones basadas en datos.