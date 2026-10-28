# Pronosticar el éxito en la NFL

Proyecto del curso "Programar con criterio en la era de la IA".
Pregunta: ¿qué características de un jugador, conocidas en el draft,
permiten pronosticar su éxito profesional?

Autor/a: Constanza Regina Ordóñez Hernández

## Datos
- Archivo: nfl_data.csv del repositorio phcs971/nfl-draft-dataset
  (licencia MIT), leído desde una URL fijada a la versión 54730ea.
- Contenido: Información para el análisis de los jugadores de la NFL.
    - 14,163 jugadores → Filas
    - 59 variables → Columnas
- Base de análisis: jugadores con información disponible sobre su carrera profesional y sobre las características observadas antes del draft.

## Variables principales
- Éxito observado:
    - Variable: pro_bowls
    - ¿Qué mide? La cantidad de veces que un jugador fue seleccionado al Pro Bowl durante su carrera profesional en la NFL. Un mayor número de selecciones se interpreta como un mayor éxito deportivo.
- Predictores:
    - posición (pos)
    - estatura (height)
    - peso (weight)
    - tamaño de mano (hand_size)
    - longitud de brazo (arm_length)
    - resultados de pruebas físicas (40-yard dash, bench press, salto vertical, broad jump, shuttle)
    - universidad (college) y
    - posición en el draft (draft_round y draft_pick)

## Decisiones de limpieza
1. Filtrar todos los jugadores que no tengan información de career_av, ya que no es posible medir su éxito profesional.
2. Eliminar las observaciones con datos faltantes en las variables utilizadas en el análisis para evitar errores en los resultados.
3. Seleccionar únicamente las variables relevantes para el análisis y descartar aquellas que no aportan información para predecir el éxito profesional
4. Eliminar los registros duplicados.

## Carpetas
- sesion-1/ a sesion-5/: trabajos de cada sesión
