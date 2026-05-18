# Proyecto — Análisis de Datos (Evaluación final)

*Instituto Tecnológico Metropolitano* · Departamento de Sistemas · Ingeniería de Sistemas  
*Curso:* Análisis de Datos · *Docente:* Daniel Alexis Nieto Mora · *Semestre:* 2026-1

## Objetivo del proyecto

Aplicar lo visto en el curso en un caso práctico de *predicción de incumplimiento de SLA (ANS)* en el sistema de soporte técnico *Lillosupport*.

El trabajo incluye:

- Explorar y documentar la fuente de datos (tabular, base relacional operativa).
- Justificar la base utilizada (completitud, relevancia para SLA, documentación del sistema).
- Realizar un EDA completo sobre incidencias y cumplimiento de ANS.
- Aplicar preprocesamiento (codificación, escalado) y modelos de clasificación.
- Construir tablas para visualización en Power BI.

## Fuente de datos

| Elemento | Detalle |
|----------|---------|
| *Tipo* | Tabular (relacional) |
| *Origen* | Base de datos *Supabase* — Sistema Lillosupport |
| *Tablas* | incidencias, ans_resultados, ans_configuracion, tipos_servicio |
| *Variable objetivo* | cumple_ans (1 = cumple ANS, 0 = incumple) |
| *Archivo de entrada* | BD.csv |
| *Archivo procesado* | BD_limpia.csv (generado en Fase 1 — ETL 3) |

## Estructura del repositorio


├── README.md
├── Incumplimiento_SLA.ipynb    # Pipeline: ETL → EDA → BI → modelado


*Notas:*

- Colocar BD.csv en la raíz del proyecto antes de ejecutar las celdas de carga (ETL 1).
- Ejecutar las celdas *en orden*; cada fase depende de la anterior.
- Tras completar ETL 3 se genera BD_limpia.csv; las fases siguientes pueden cargar ese archivo.

## Integrantes

| Integrante |
|------------|
| Danny Mateo Hernández Sánchez|
| Stefany Builes Lopera |
| Leidy Daihana Mora Trujillo |
| Alejandra Alvarez Serna |
