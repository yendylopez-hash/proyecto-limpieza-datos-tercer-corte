# proyecto-limpieza-datos-tercer-corte
PARCIAL CORTE 3
# Proyecto: Limpieza de Datos con POO
Análisis y limpieza de una encuesta socioeconómica usando Python.
## Descripción
Sistema de limpieza de datos implementado con POO (clase Limpiador).
Normaliza textos, genera género, convierte ingresos y edades, elimina
duplicados e inválidos, y genera resumen estadístico.
## Objetivo
- Diagnosticar errores en datos reales
- Implementar métodos de limpieza usando POO
- Validar datos contra criterios específicos
- Generar estadísticas descriptivas
Programación de Computadores Universidad ECCI 3

## Archivos
- Proyecto_Tercer_Corte_Limpieza_POO.ipynb
- encuesta_sucia.csv
- README.md
## Dataset
Archivo: encuesta_sucia.csv
- Filas brutas: 58
- Filas válidas: 50
- Columnas: id, ciudad, edad, ingreso, genero
## Categorías de Error
Texto ciudad: BOGOTÁ, medellin, Medellín
Género: f, Femenino, M, masculino
Ingreso: $2.200.000, 3.500.000 COP
Edad: 39 anios, 61 años
Duplicados: Mismo id múltiples veces
Basura: Ciudad inexistente, edad=200
## Clase Limpiador
- limpiar_texto(): normaliza ciudad
- limpiar_genero(): convierte a F o M
- limpiar_ingreso(): elimina símbolos
- limpiar_edad(): elimina palabras
- es_valida(): valida criterios
- limpiar(): procesa dataset
- resumen(): estadísticas
## Resultados Esperados
n=50, Ciudades=5, F=29, M=21
Edad: min=18, max=65, prom=39.16
Ingreso: min=1300000, max=8000000, prom=4018000.0
## Notas Técnicas
Python puro, sin pandas. Manejo de tildes con chr().
CSV con csv.DictReader.
## Autor
[Yendy Daniela Lopez Celis] - Estudiante Estadística - Universidad ECCI - 2026-I
