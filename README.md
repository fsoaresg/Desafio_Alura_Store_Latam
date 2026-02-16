---

# Alura Store LATAM – Optimización Estratégica del Portafolio de Tiendas

Proyecto de análisis end-to-end orientado a identificar la unidad menos eficiente del portafolio y traducir métricas operativas en una decisión estratégica de inversión.

---

## Problema de Negocio

El Sr. Juan, propietario de la cadena Alura Store, desea vender una de sus 4 tiendas para financiar un nuevo emprendimiento.

La decisión no puede basarse en percepción, sino en:

- Rentabilidad comparativa
- Eficiencia operativa
- Satisfacción del cliente
- Desempeño comercial por categoría
- Impacto estratégico dentro del portafolio
- 
El objetivo del proyecto fue determinar, con base en datos, qué tienda aporta menor valor estratégico al negocio.

---

## Enfoque Analítico

El análisis siguió una estructura orientada a toma de decisión ejecutiva:

1. Extracción de datos desde GitHub (4 datasets independientes)
2. Limpieza y validación de datos
3. Cálculo de KPIs comparativos
4. Análisis de eficiencia multidimensional
5. Identificación de causa raíz
6. Recomendación estratégica fundamentada

---

## Indicadores Evaluados

Se construyó una evaluación comparativa basada en:

- Ingresos totales y participación porcentual
- Ventas por categoría
- Calificación promedio de clientes
- Productos más y menos vendidos
- Costo de envío promedio
- Matriz de Eficiencia (Satisfacción vs Costos)
- Matriz de Valor Estratégico (Satisfacción vs Ingresos)
- Eficiencia Global (modelo ponderado)

El análisis no se limitó a métricas aisladas, sino a una evaluación integrada del desempeño.

---

## Hallazgos Clave

**La Tienda 4:**

- **Presenta el menor ingreso total de las cuatro tiendas**
  Es la unidad con menor contribución financiera dentro del portafolio.

- **No lidera en ninguna categoría estratégica**
   No destaca ni en volumen de ventas ni en rotación de productos clave.

- **Tiene una calificación promedio inferior**
   Reflejando una menor satisfacción del cliente.

- **Presenta bajo desempeño incluso con vendedores experimentados**
   Vendedores con buen historial en otras sucursales, como Pedro Gomez, muestran bajo rendimiento, lo que sugiere problemas estructurales u operativos.

- **Con un menor costo de envío no logra compensar sus debilidades**
   Aunque posee el costo de envío más bajo, este factor no logra equilibrar sus debilidades en ingresos y percepción del cliente.

- **Sus productos más vendidos no alcanzan el nivel de desempeño observado en otras tiendas**
   Incluso sus top sellers muestran menor tracción relativa frente a los líderes del portafolio.

- **Posee productos con baja rotación**
   Especialmente en:
     - Instrumentos musicales
     - Electrodomésticos
       
- **Presenta la menor eficiencia global dentro del portafolio**
   El modelo ponderado confirma que Tienda 4 ocupa la última posición en desempeño integral.

---

## Resultado Final

- **Tienda con mayor eficiencia global: Tienda 1**
- **Tienda con menor eficiencia global: Tienda 4**

---

## Recomendación Estratégica

**Vender Tienda 4.**

Desde una perspectiva de portafolio:

- Es la unidad con menor aporte estratégico.
- No presenta ventajas competitivas diferenciales.
- Su eficiencia global es la más baja del grupo.
- La reinversión del capital en un nuevo proyecto podría generar mayor retorno esperado.

La decisión no responde únicamente a ingresos, sino a una evaluación integral de eficiencia y valor estratégico.

---

## Tecnologías utilizadas

- **Python 3**
- **Pandas**: manipulación y análisis de datos.
- **NumPy**: operaciones numéricas.
- **Matplotlib**: visualización de datos estática.
- **Folium**: mapas interactivos para análisis geográfico.
- **Google Colab**: entorno de ejecución y colaboración.

---

## Datos

Se analizaron las ventas de las 4 tiendas:  

| Tienda | Dataset |
|--------|---------|
| Tienda 1 | [CSV](https://raw.githubusercontent.com/fsoaresg/Desafio-Alura-Store-Latam/main/base-de-datos-alura-store-latam/tienda_1%20.csv) |
| Tienda 2 | [CSV](https://raw.githubusercontent.com/fsoaresg/Desafio-Alura-Store-Latam/main/base-de-datos-alura-store-latam/tienda_2.csv) |
| Tienda 3 | [CSV](https://raw.githubusercontent.com/fsoaresg/Desafio-Alura-Store-Latam/main/base-de-datos-alura-store-latam/tienda_3.csv) |
| Tienda 4 | [CSV](https://raw.githubusercontent.com/fsoaresg/Desafio-Alura-Store-Latam/main/base-de-datos-alura-store-latam/tienda_4.csv) |

**Variables principales:**  
- Producto  
- Categoría del producto  
- Precio  
- Costo de envío  
- Calificación promedio  
- Vendedor  
- Ubicación (latitud y longitud)

---

## Visualizaciones Generadas

![Ingresos totales por tienda](images/Ingresos%20totales%20por%20tienda.png)

![Ventas por categoría de productos](images/Popularidad%20de%20Categor%C3%ADas%20por%20Tienda.png)

![Calificación promedio de los clientes](images/Satisfacci%C3%B3n%20promedio%20de%20los%20clientes%20por%20tienda.png)

![Productos más y menos vendidos](images/Productos%20m%C3%A1s%20y%20menos%20vendidos%20por%20tienda.png)

![Costo de envío promedio](images/Env%C3%ADo%20promedio%20por%20tienda.png)

![Análisis integrado: eficiencia, valor estratégico y desempeño](images/Matriz%20de%20Eficiencia%20y%20Matriz%20de%20Valor%20Estrat%C3%A9gico.png)

![Mapa de calor](images/mapa%20de%20calor.png)

## Mapa interactivo de las ventas

[![Explorar Mapa Interactivo](https://img.shields.io/badge/Explorar-Mapa%20Interactivo-2563eb?style=for-the-badge&logo=leaflet&logoColor=white)](https://superb-starburst-6b8092.netlify.app/)

**Vista Previa:**
![Captura de visualizaciones interactivas]((images/mapa%20interactivo%20vista%20previa.png)

---

## Contenido del proyecto

1. **Importación de datos**
   - Se importaron los datasets de las 4 tiendas desde GitHub.
   - Cada dataset contiene: `Producto`, `Categoría del Producto`, `Precio`, `Calificación`, `Costo de envío`, `Vendedor`, `lat`, `lon`.

2. **Análisis de datos**
   - **Ingresos totales por tienda**: cálculo de ingresos y porcentaje sobre el total.
   - **Ventas por categoría**: identificación de categorías con mayor y menor volumen de ventas.
   - **Calificación promedio de clientes**: satisfacción promedio por tienda.
   - **Productos más y menos vendidos**: análisis del desempeño de productos individuales.
   - **Costo de envío promedio por tienda**: evaluación del impacto en eficiencia.
   - **Matriz de Eficiencia**: relación entre satisfacción y costo de envío.
   - **Matriz de Valor Estratégico**: relación entre satisfacción y ingresos.
   - **Eficiencia Global**: combinación ponderada de ingresos, satisfacción y costos de envío.
   - **Causa raíz de baja eficiencia (Tienda 4)**: categorías, productos y vendedores con bajo desempeño.
   - **Análisis geográfico**: concentración de ventas por ubicación y mapa interactivo.

3. **Visualizaciones**
   - Gráficos de barras horizontales para ingresos, satisfacción, costo de envío y productos.
   - Comparativas de ventas por categoría entre tiendas.
   - Matrices de eficiencia y valor estratégico.
   - Mapas de calor y mapas interactivos de ventas.
  
4. **Informe Final**
   - Introducción
   - Desarrollo del análisis
   - Conclusión y recomendación final
   - Recomendación adicional

---

## Cómo usar este proyecto

1. Abrir el cuaderno en **[Google Colab](https://colab.research.google.com/github/fsoaresg/Desafio-Alura-Store-Latam/blob/main/AluraStoreLatam.ipynb)**.
2. Ejecutar las celdas paso a paso para:
   - Importar los datos desde GitHub.
   - Generar métricas de ingresos, ventas, satisfacción y eficiencia.
   - Visualizar los gráficos y mapas interactivos.
3. Analizar los resultados y tomar decisiones estratégicas basadas en los insights.

---

## Estructura del repositorio

├── Challenge-Alura-Store.ipynb # Cuaderno de Colab con análisis completo

├── README.md # Este archivo

├── 📂 images/

├── 📂 base-de-datos-alura-store-latam/

│ ├── tienda_1.csv

│ ├── tienda_2.csv

│ ├── tienda_3.csv

│ └── tienda_4.csv

---

## Competencias Demostradas

Este proyecto evidencia capacidad en:

- Análisis comparativo multivariable
- Construcción de KPIs estratégicos
- Evaluación de eficiencia operativa
- Identificación de causa raíz
- Storytelling orientado a negocio
- Traducción de métricas en decisiones ejecutivas
- Análisis geoespacial aplicado
- Pensamiento estratégico de portafolio

---

## Autor

**Fátima Soares**  
Data Analyst | Enfoque en análisis estratégico y toma de decisiones basada en datos.
Especializada en transformar métricas operativas en insights ejecutivos accionables.
[GitHub](https://github.com/fsoaresg)

---

## Licencia

Este proyecto es de **uso educativo y demostrativo**, con base en un desafío de Alura Latam.
