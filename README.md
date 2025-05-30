# Reto 04 - Visualización de Datos con Shiny

Este repositorio contiene una aplicación interactiva desarrollada con **Shiny en R** para analizar el comportamiento de compra de los clientes de un supermercado, segmentar sus perfiles mediante clustering y visualizar diferentes resultados de modelos y recomendaciones.

---

💻 Cómo descargar el proyecto en tu equipo

Si quieres probar el proyecto en tu propio ordenador, puedes clonar este repositorio desde GitHub. 
### 👉 Pasos:

1. Abre una terminal o consola (por ejemplo, Git Bash en Windows).
2. Ejecuta el siguiente comando para clonar el repositorio:

```
git clone https://github.com/javierllorenteMon/VisuShinyApp
```

---

## 🌟 Funcionalidades destacadas

### ▶️ Estructura de la interfaz
La aplicación está organizada en **cuatro pestañas principales**:

1. **Análisis Exploratorio**: permite visualizar información agregada de los datos de compra con diferentes tipos de gráficos.
2. **Clusterización**: muestra cómo se han segmentado los clientes, incluyendo centroides, productos preferidos y representaciones 3D.
3. **Modelos**: compara distintos algoritmos de recomendación con métricas y visualizaciones como curvas ROC o errores.
4. **Objetivos**: resume los resultados obtenidos en distintos objetivos del reto, incluyendo recomendaciones por cliente.

### ⚙️ Filtros interactivos con `sidebarLayout`

En la pestaña de **Análisis Exploratorio**, se ha implementado un `sidebarLayout` que permite:

- Filtrar por rango de fechas.
- Seleccionar días de la semana (excluyendo domingos).
- Elegir una categoría de producto general.
- Definir un mínimo de unidades vendidas.
- Aplicar o resetear los filtros mediante botones.

Estos filtros afectan a varios gráficos de forma reactiva, permitiendo una exploración personalizada de los datos.

### 📊 Visualizaciones interactivas

- Gráficos con `ggplot2` y `plotly` para mejorar la experiencia de usuario.
- Tabla de centroides exportable a CSV/Excel.
- Representaciones 3D de clusters.
- Radar plot (en pruebas) para comparar comportamientos por cluster.

### 🔬 Análisis de Clusters y Modelos

- Segmentación mediante `k-means` y visualización de centroides.
- Método del codo para estimar el número óptimo de clusters.
- Evaluación de algoritmos de recomendación mediante RMSE, MAE, MSE y curva ROC.
