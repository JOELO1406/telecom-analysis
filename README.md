# telecom-analysis                      <img width="406" height="94" alt="image" src="https://github.com/user-attachments/assets/9aef58ee-b171-4e6b-ba7d-cfd5e199a73d" />

📊 Análisis de Comportamiento de Usuarios y Segmentación - ConnectaTel

Este repositorio contiene el análisis exploratorio de datos (EDA) y la segmentación de clientes para **ConnectaTel**. El objetivo principal es comprender las pautas de consumo en minutos, llamadas y mensajes por tipo de plan para generar recomendaciones comerciales y optimizar la oferta de servicios.

---

## 🎯 Objetivo del Proyecto

* **Analizar el consumo:** Evaluar los patrones de uso en llamadas, duración de minutos y envío de mensajes entre los distintos planes (Básico vs. Premium).
* **Identificar perfiles y outliers:** Detectar la presencia de *heavy users* (usuarios de alto consumo) y analizar cómo afecta la edad al comportamiento de uso.
* **Proponer estrategias comerciales:** Traducir los hallazgos en recomendaciones accionables de negocio para mejorar la retención, empaquetado de tarifas y rentabilidad.

---

## 📁 Datasets Utilizados

El análisis se basa en el procesamiento de la información agregada de los usuarios:

* **`user_profile` / Datasets de Consumo:**
  * `age`: Edad de los usuarios (rango de 18 a 80 años).
  * `plan`: Tipo de tarifa suscrita (*Básico* o *Premium*).
  * `cant_mensajes`: Cantidad de mensajes enviados por usuario.
  * `cant_llamadas`: Cantidad total de llamadas realizadas.
  * `cant_minutos_llamada` / `total_minutos_llamada`: Suma de minutos consumidos en llamadas.
  * `grupo_uso`: Columna categórica creada para clasificar a los usuarios según su nivel de consumo.

---

## 🛠️ Etapas del Análisis Realizadas

1. **Limpieza y Preparación de Datos:**
   * Estandarización de nombres de columnas y verificación de inconsistencias.
   * Análisis de valores nulos e integridad de las variables numéricas.

2. **Análisis Exploratorio de Datos (EDA) y Distribuciones:**
   * Cálculo de la distribución porcentual por tipo de plan mediante `value_counts(normalize=True)`.
   * Análisis gráfico mediante histogramas para determinar el tipo de distribución de cada variable (uniforme para edad; sesgadas a la derecha para mensajes, llamadas y minutos).

3. **Detección y Tratamiento de Outliers:**
   * Generación automatizada de **Boxplots** mediante bucles `for` en Seaborn/Matplotlib.
   * Cálculo de límites superiores utilizando el método del Rango Intercuartílico (**IQR**).
   * Justificación de negocio para mantener los valores atípicos (*heavy users* de voz y mensajes) en el dataset final.

4. **Segmentación y Creación de Características:**
   * Incorporación de la variable `grupo_uso` utilizando condicionales (`np.select`) para categorizar a los usuarios según su nivel de interacción.

5. **Insights Ejecutivos para Stakeholders:**
   * Redacción de conclusiones clave orientadas al negocio, evaluando el impacto operacional y estratégico de los hallazgos.

---

## 🚀 Cómo Ejecutar el Notebook

Puedes ejecutar este proyecto fácilmente desde la nube utilizando **Google Colab** o de forma local en **Jupyter Notebook**.

### Opción 1: Abrir directamente en Google Colab (Recomendado)

1. Haz clic en el botón de abajo (si está configurado en tu repositorio) o dirígete a [📊 Análisis de Comportamiento de Usuarios y Segmentación - ConnectaTel

Este repositorio contiene el análisis exploratorio de datos (EDA) y la segmentación de clientes para **ConnectaTel**. El objetivo principal es comprender las pautas de consumo en minutos, llamadas y mensajes por tipo de plan para generar recomendaciones comerciales y optimizar la oferta de servicios.

---

## 🎯 Objetivo del Proyecto

* **Analizar el consumo:** Evaluar los patrones de uso en llamadas, duración de minutos y envío de mensajes entre los distintos planes (Básico vs. Premium).
* **Identificar perfiles y outliers:** Detectar la presencia de *heavy users* (usuarios de alto consumo) y analizar cómo afecta la edad al comportamiento de uso.
* **Proponer estrategias comerciales:** Traducir los hallazgos en recomendaciones accionables de negocio para mejorar la retención, empaquetado de tarifas y rentabilidad.

---

## 📁 Datasets Utilizados

El análisis se basa en el procesamiento de la información agregada de los usuarios:

* **`user_profile` / Datasets de Consumo:**
  * `age`: Edad de los usuarios (rango de 18 a 80 años).
  * `plan`: Tipo de tarifa suscrita (*Básico* o *Premium*).
  * `cant_mensajes`: Cantidad de mensajes enviados por usuario.
  * `cant_llamadas`: Cantidad total de llamadas realizadas.
  * `cant_minutos_llamada` / `total_minutos_llamada`: Suma de minutos consumidos en llamadas.
  * `grupo_uso`: Columna categórica creada para clasificar a los usuarios según su nivel de consumo.

---

## 🛠️ Etapas del Análisis Realizadas

1. **Limpieza y Preparación de Datos:**
   * Estandarización de nombres de columnas y verificación de inconsistencias.
   * Análisis de valores nulos e integridad de las variables numéricas.

2. **Análisis Exploratorio de Datos (EDA) y Distribuciones:**
   * Cálculo de la distribución porcentual por tipo de plan mediante `value_counts(normalize=True)`.
   * Análisis gráfico mediante histogramas para determinar el tipo de distribución de cada variable (uniforme para edad; sesgadas a la derecha para mensajes, llamadas y minutos).

3. **Detección y Tratamiento de Outliers:**
   * Generación automatizada de **Boxplots** mediante bucles `for` en Seaborn/Matplotlib.
   * Cálculo de límites superiores utilizando el método del Rango Intercuartílico (**IQR**).
   * Justificación de negocio para mantener los valores atípicos (*heavy users* de voz y mensajes) en el dataset final.

4. **Segmentación y Creación de Características:**
   * Incorporación de la variable `grupo_uso` utilizando condicionales (`if/else`, `np.where` o `np.select`) para categorizar a los usuarios según su nivel de interacción.

5. **Insights Ejecutivos para Stakeholders:**
   * Redacción de conclusiones clave orientadas al negocio, evaluando el impacto operacional y estratégico de los hallazgos.

---

## 🚀 Cómo Ejecutar el Notebook

Puedes ejecutar este proyecto fácilmente desde la nube utilizando **Google Colab** o de forma local en **Jupyter Notebook**.

### Opción 1: Abrir directamente en Google Colab (Recomendado)

1. Haz clic en el botón de abajo (si está configurado en tu repositorio) o dirígete a https://github.com/JOELO1406/telecom-analysis
2. Selecciona la pestaña **GitHub** e ingresa la URL de este repositorio.
3. Abre el archivo `.ipynb` del proyecto.
4. Ejecuta las celdas en orden presionando `Shift + Enter`.

---
Proyecto Elaborado por Ing. Joel Serrato Guzmán.
