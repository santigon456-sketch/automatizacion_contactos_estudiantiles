# ⚡ Agilidad en extraccion de datos: Consolidación Automatizada de Contactos Académicos

Este repositorio contiene un flujo de automatización bajo demanda (ad-hoc) desarrollado en **Power Automate Desktop**. El objetivo fue resolver un requerimiento urgente de gestión administrativa: la extracción masiva de correos institucionales desde un sistema de gestión académica (SIU Guaraní).

## 🎯 El Desafío: "Sprint" de Recopilación de Datos
Se presentó una tarea de alta prioridad que consistía en obtener el correo electrónico de **200 alumnos** basándose en un listado de nombres y DNIs en Excel. 

### El obstáculo técnico:
* **Falta de API Directa:** El sistema de gestión no permitía una exportación masiva rápida de estos datos específicos.
* **Interfaz Dinámica:** El SIU Guaraní requiere navegación por múltiples menús y el manejo de sesiones activas que expiran.
* **Costo de Oportunidad:** Realizar 200 búsquedas manuales representaba una jornada completa de trabajo administrativo de bajo valor añadido y alto riesgo de error de transcripción.

## 🛠️ Solución Técnica (RPA Scraping)
En lugar de proceder con la carga manual, desarrollé un flujo de **Web Scraping** mediante RPA que automatizó el ciclo completo en una sola mañana.

### Componentes del Flujo:
1. **Data Feeding:** Lectura dinámica de un archivo Excel de origen para iterar sobre cada registro.
2. **Navegación Web Robusta:** Implementación de lógica para manejar los tiempos de respuesta del servidor y la búsqueda por parámetros específicos dentro del portal académico.
3. **Extracción y Limpieza:** Captura de texto (Data Scraping) desde la interfaz de usuario, asegurando que el correo electrónico capturado correspondiera exactamente al alumno buscado mediante validaciones de DNI.
4. **Salida Estructurada:** Escritura automática de los resultados en una nueva columna del archivo Excel original.

## 📊 Resultados e Impacto de Negocio
* **Eficiencia Temporal:** Lo que se estimaba como una tarea de 6-8 horas de trabajo manual, fue resuelto con un desarrollo de **3 horas** (incluyendo pruebas) y una ejecución automática de pocos minutos.
* **Integridad de los Datos:** Se garantizó un **100% de precisión** en los contactos obtenidos, eliminando errores de "copiar y pegar".
* **Mentalidad Data-Driven:** Demostración de capacidad para pivotar ante tareas urgentes y aplicar soluciones técnicas que optimizan los recursos de la facultad.

## 🧠 Lecciones Aprendidas
Este proyecto reforzó mi capacidad para manejar **selectores dinámicos** y tiempos de espera en automatizaciones web, habilidades críticas para cualquier profesional que trabaje con flujos de datos e interoperabilidad entre sistemas antiguos y herramientas modernas.

---
*Proyecto desarrollado por Santiago Gonzalez - Analista Administrativo (FCM-UNL) & Estudiante de Ciencia de Datos e IA.*
