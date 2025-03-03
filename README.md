# SergiVergaraEco_Actuary_R

Este repositorio contiene código y herramientas actuariales desarrolladas en **R Studio** para la modelización del **riesgo de longevidad en hipotecas inversas** mediante **métodos numéricos**.  

# Contenido del repositorio
- 📂 `Calculadora_hipoteca_Inversa_Máxima/`
  - 📝 `Codigo_general.txt` → Código principal del modelo actuarial.
  - 🛠️ `Funciones_entorno.txt` → Funciones auxiliares usadas en los cálculos.
  - 📊 `Riesgo_de_longevidad_Hipotecas_Inversas.R` → Script en R para la simulación del modelo.
  - 📖 `Riesgo_Longevidad_Hipotecas_Inversas.pdf` → Documento con la teoría detrás del modelo.
  - 📑 `TABLA_VIDA.xlsx` → Datos de tablas de mortalidad utilizadas en el cálculo.
  - 🏡 `VIVIENDA.xlsx` → Datos de mercado inmobiliario para el análisis.

#Objetivo del Proyecto
El objetivo de este repositorio es proporcionar una **herramienta actuarial en R** para evaluar la **prima de riesgo y anualidad máxima** en hipotecas inversas, considerando el **riesgo de longevidad** mediante técnicas como:
- **Interpolación lineal**
- **Modelos de capitalización y revalorización**
- **Método de Newton-Raphson multidimensional**
- **Análisis de VaR actuarial**

La idea del trabajo es obtener una prima de riesgo de equilibro mediante el uso de metodos numericos.
  
Este trabajo forma parte de mi formación en el **Máster en Ciencias Actuariales y Financieras (UB)** y es resultado de la aplicación de conocimientos en cálculo numérico, estadística actuarial y modelización financiera.  

# Instalación y Uso
1. Descarga la carpeta, si solo estas interesado en la calculadora bastaría el script en R.
2. Ejecuta el script desde "source", el script esta montado para generar el entorno directamente. Aun así he dejado el entorno en archivos por lo que puedes cargarlo manualente si lo prefieres
3. Introduce los datos
4. Obten soluciones de mi modelo


Podría ser interesante de cara a una aplicación mas precisa modificar el codigo cargando tablas de mortalidad segregada.


Este proyecto se distribuye bajo la MIT License, permitiendo su uso libre con fines educativos y de investigación.

Email: sergivergaraeco@outlook.com
LinkedIn: https://www.linkedin.com/in/sergivergaraeco/

