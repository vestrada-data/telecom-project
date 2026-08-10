# Análisis de una empresa de telecomunicaciones  - Sprint 7

Este repositorio contiene el análisis del caso ConnectaTel.

 ## 🎯 Objetivo General

El objetivo es identificar patrones de uso, detectar comportamientos atípicos y comprender qué segmentos de clientes muestran necesidades diferenciadas, con el fin de optimizar la oferta comercial y mejorar la experiencia del usuario.

Trabajaremos con tres datasets principales de información, relacionadas con usuarios, actividad y planes del servicio de telecomunicaciones:

*plans.csv:*  Catálogo de planes con sus precios y beneficios. <br>
*users_latam.csv:*  Información de cada usuario (datos personales, plan, fecha de registro, churn). <br>
*usage.csv* Actividad generada por los usuarios: llamadas, mensajes, duración, longitud. <br>

Contamos con  40,000 registros con valores faltantes, sentinels, outliers y problemas de calidad diseñados para simular datos reales.

## 🛠️ Herramientas Utilizadas
Python (Pandas, Matplotlib, Seaborn)

## KPIs monitoreados

## 🧠 Objetivo del análisis
- Identificar problemas de calidad de datos
- Limpieza  básica (reemplazar sentinels, convertir fechas, impitar o marcar NA)
- Summary statistics
- Visualización & outliers
- Segmentación
- Analizar comportamientos, distribuciones y outliers
- Generar insights para Stakeholders

##  🔎 Hallazgos

Se detectaron datos nulos y centinelas en diferentes columnas
• El 11.72% del total de city eran datos nulos y 96 registros tenían el centinela ‘?’
• Encontré que date, tiene nulos pero con un porcentaje muy bajo del 0.12%, solo 50 registros.
• duration con 22076 registros, que representan el 55.19% eran valores nulos.
• length con un 44% también es un dato valioso para el análisis, por lo que es importante su revisión para decidir su imputación. No será eliminado.
• churn_date, tenía un valor alto del 88.35% , valor esperado ya que corresponde a la fecha de cancelación de la suscripción.
• Identifique 55 valores centinel -999 en age.

Segmentos por Edad
El segmento Adulto (30 a 59 años) domina el mercado, es el más valioso por volumen con más de 2000 usuarios.Este grupo representa el núcleo de tu base de clientes.
Adulto Mayor (60+ años): Es el segundo grupo en importancia, con poco más de 1,250 usuarios
Joven (menores de 30 años): Es el segmento más pequeño, con aproximadamente 750 usuarios.

Segmentos por Nivel de Uso
El segmento Adulto es el que más contribuye al volumen del Uso Medio, consolidándose como el perfil de cliente estándar.
A pesar de la diferencia de edad entre Adultos y Adultos Mayores, ambos tienden a concentrarse en el nivel de Uso Medio, lo que sugiere que la edad no es un factor que dispare el consumo hacia el nivel "Alto" de forma agresiva.

## 💡 Insights: El Alto Uso es un comportamiento excepcional en todos los rangos de edad, representando la menor proporción de la muestra total. Aunque es pequeño, con menos de 500 usuarios, son los clientes que superan las 10 llamadas o mensajes, lo que indica una alta dependencia del servicio.

Esto sugiere que, el uso extremo no parece ser exclusivo de una sola edad, sino que actúa como un comportamiento distribuido de forma minoritaria. Alto es un segmento que representa una oportunidad para migrarlos a planes de gama alta .
Los outliers identificados podrían representar pequeños emprendedores o trabajadores independientes con consumos mayores.
También es importante considerar que el aumento en el número de usuarios que generan estos oultiers, podría comprometer la capacidad técnica de la empresa y afectar la estabilidad de los usuarios de Uso medio.

## Recomendaciones
a) Identificar a los usuarios del segmento de Alto uso que actualmente tienen planes básicos y ofréceles una actualización a un plan Premium para generar un mayor ingreso promedio por usuario.
b) Dado que los usuarios del segmento Adulto Mayor son el segundo grupo más grande, se podrían diseñar planes con beneficios específicos como redes sociales ilimitadas, para asegurar su lealtad
c) Dirigir campañas publicitarias al segmento Adulto que es el de mayor volumen.
d) ConnectaTel podría lanzar promociones enfocadas en datos móviles al segmento Joven que es el de menor volumen.
e) Investigar si hay usuarios del segmento Alto uso que utilizan su línea personal para fines profesionales, lo que abre la puerta para crear productos específicos para microempresas.


<img width="548" height="368" alt="Actividad   Telefonica" src="https://github.com/user-attachments/assets/a7aed735-a135-40da-ae39-6f9b1355c87d" />
<img width="612" height="371" alt="Distribucion Mensajes" src="https://github.com/user-attachments/assets/a246bb97-bfde-4992-8b52-cd050165eea3" />
 <img width="553" height="363" alt="Minutos Llamada" src="https://github.com/user-attachments/assets/6e51fa28-c2bc-46da-b931-0f0e4126c114" />
 
## ▶ Cómo abrir el notebook en Google Colab
Haz clic en el siguiente botón:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/11yrhUvfrQaq69nP1ZmriXNMOP2RkErim#scrollTo=ee7c578d)


2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)


