# Experimento A/B en Página de Inicio (Landing Page)

Análisis estadístico de un experimento A/B realizado sobre una página de inicio, con el objetivo de determinar qué versión (**A** o **B**) genera mejores resultados de negocio y respaldar la decisión con datos.

## 📋 Descripción del proyecto

El dataset contiene información de **40,000 usuarios** expuestos a dos versiones de una landing page. Se analiza:

1. 🔍 Exploración y validación de los datos
2. 💰 Comparación del **gasto promedio** por usuario entre la página A y B
3. 🎯 Comparación de la **tasa de conversión** entre la página A y B
4. 🌐 Relación entre la **fuente de tráfico** y la conversión
5. 👤 Relación entre el **tipo de usuario** y la conversión
6. 📈 Visualización de resultados
7. 🧩 Insight ejecutivo para stakeholders con la recomendación final

Se aplican pruebas estadísticas (t-test, chi-cuadrado, prueba z de proporciones) para sustentar las conclusiones.

## 📁 Estructura del proyecto

```
.
├── S9_Version_Student_Proyecto_Landing_Experiment_V2.ipynb   # Notebook principal
├── landing_experiment.csv                                     # Datos del experimento
└── README.md
```

## 📊 Datos

El archivo `landing_experiment.csv` contiene las siguientes columnas:

| Columna          | Descripción                                              |
|------------------|-----------------------------------------------------------|
| `user_id`        | Identificador único del usuario                          |
| `date`           | Fecha de la visita                                        |
| `landing`        | Versión de la página mostrada (`A` o `B`)                |
| `region`         | Región del usuario                                         |
| `dispositivo`    | Tipo de dispositivo (Mobile, etc.)                        |
| `traffic_source` | Fuente de tráfico (Email, Organic, Ads, etc.)             |
| `user_type`      | Tipo de usuario (Nuevo, Recurrente)                       |
| `converted`      | Si el usuario convirtió (1) o no (0)                      |
| `gasto`          | Gasto realizado por el usuario                            |

## ⚙️ Requisitos

- Python 3.10 o superior
- Las siguientes librerías:

```
pandas
numpy
scipy
statsmodels
matplotlib
seaborn
```

## 🚀 Instalación y ejecución

1. **Clona este repositorio**
   ```bash
   git clone <url-de-tu-repositorio>
   cd <nombre-del-repositorio>
   ```

2. **(Opcional pero recomendado) crea un entorno virtual**
   ```bash
   python -m venv venv
   venv\Scripts\activate      # Windows
   source venv/bin/activate   # macOS/Linux
   ```

3. **Instala las dependencias**
   ```bash
   python -m pip install pandas numpy scipy statsmodels matplotlib seaborn jupyterlab
   ```

4. **Verifica que el archivo `landing_experiment.csv` esté en la misma carpeta que el notebook.** El notebook lo carga con una ruta relativa (`pd.read_csv('landing_experiment.csv')`), así que ambos archivos deben estar juntos.

5. **Ejecuta Jupyter**
   ```bash
   python -m jupyter lab
   ```

6. **Abre el archivo** `S9_Version_Student_Proyecto_Landing_Experiment_V2.ipynb` desde el explorador de JupyterLab y ejecuta las celdas en orden (Run All, o celda por celda).

## 📈 Resultado

El notebook concluye con un apartado de **Insight Ejecutivo para Stakeholders**, que resume los hallazgos estadísticos y recomienda cuál versión de la landing page conviene implementar.

## 🛠️ Autor

Jose Mejia Contreras
