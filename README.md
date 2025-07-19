# Análisis de Modelos de Regresión Lineal para Predicción de Precios de Hoteles

## 📌 Descripción del Proyecto

Este proyecto tiene como objetivo comparar diferentes modelos de **regresión lineal múltiple** para predecir el **precio (`Preco`) de hoteles**, utilizando variables explicativas como:
- `Estrelas`: Número de estrellas del hotel
- `ProximidadeTurismo`: Distancia o proximidad a zonas turísticas
- `Capacidade`: Capacidad del hotel (número de habitaciones o huéspedes)

Se han construido y evaluado **cuatro modelos** con distintas combinaciones de variables, y se ha seleccionado el **mejor modelo** en términos de ajuste y capacidad predictiva.

## 📁 Estructura del Proyecto
hotel_pricing_model/
- ├── master/ # Carpeta con los datos de entrada
- │ └── hotels.csv
- ├── README.md # Este archivo
- ├── LICENSE # Este archivo
- ├──Fijacion_de_precios_de_Habitaciones_de_hoteles.ipynb # Carpeta con los cuadernos de análisis


## 🧪 Modelos Entrenados

| Modelo | Variables Incluidas                          | R²    | Adj. R² | Comentarios                        |
|--------|----------------------------------------------|-------|---------|------------------------------------|
| 0      | `Estrelas`                                   | 0.161 | 0.160   | Muy básico                         |
| 1      | `Estrelas`, `ProximidadeTurismo`             | 0.650 | 0.649   | Mejora significativa               |
| 2      | `Estrelas`, `ProximidadeTurismo`, `Capacidade` | 0.923 | 0.923   | Mejor modelo (sin overfitting)     |
| 3      | `Estrelas`, `ProximidadeTurismo`, `Preco`    | 1.000 | 1.000   | Inválido (data leakage)            |

## 📈 Objetivos del Cuaderno

En este cuaderno se realiza el siguiente análisis:

1. **Carga y exploración de datos**
2. **Construcción de los modelos de regresión**
3. **Comparación de métricas (R², AIC, BIC, F-stat, etc.)**
4. **Validación de supuestos del modelo lineal**
   - Normalidad de residuos
   - Homocedasticidad
   - Linealidad
   - Ausencia de multicolinealidad
5. **Visualización de residuos y diagnóstico del modelo**
6. **Selección del modelo final**

## 📊 Visualizaciones Generadas

- Gráfico de residuos vs. valores ajustados
- Histograma y QQ-Plot de residuos
- Gráficos de residuos vs. variables explicativas
- Análisis de factores de inflación de varianza (VIF)
- Comparación de métricas entre modelos

## 📤 Exportación
El cuaderno permite exportar:

- Gráficos en carpetas (plots/)
- Informes PDF (opcionalmente con nbconvert)
- Resúmenes de modelos en tablas
  
## Si tienes dudas o quieres colaborar, puedes contactarme en:

* Correo: cmpmendoza12@gmail.com
* GitHub: [[w2k31984](https://github.com/w2k31984/)]
