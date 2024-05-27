# Tarea TAS7 - Events
## 1. Lista de socios mayores de 30 años, ordenados por edad en orden descendente:
  - Sentencia:
`SELECT * FROM member
WHERE age > 30
ORDER BY age DESC;`

  - Captura:

<img src="Captura de pantalla 2024-05-21 202321.png" alt="drawing" width="500"/>

## 2. Lista para  las conferencias para el evento con ID 1, ordenadas por hora de conferencia:
  - Sentencia:
SELECT * FROM conference
WHERE event_id = 1
ORDER BY hour;

  - Captura:
  <img src="Captura de pantalla 2024-05-21 202415.png" alt="drawing" width="500"/>


## 3. Eventos que se realizarán en 'Nueva York', ordenados por fecha de inicio:
 - Sentencia:
 SELECT * FROM event
WHERE city = 'New York'
ORDER BY start_date;

 - Captura:
 <img src="Captura de pantalla 2024-05-21 202442.png" alt="drawing" width="500"/>


## 4. Inscripciones a las que asistió el socio, ordenadas por fecha de inscripción:
- Sentencia:
SELECT * FROM register
WHERE assisted = TRUE
ORDER BY registered_at;

- Captura:
<img src="Captura de pantalla 2024-05-21 202511.png" alt="drawing" width="500"/>


## 5. Los miembros que se han registrado para una conferencia, ordenados por el ID de la conferencia para el que se registraron:
- Sentencia:
SELECT member.fullName, member.email, register.conference_id
FROM member
JOIN register ON member.id = register.member_id
ORDER BY register.conference_id;

- Captura:
<img src="Captura de pantalla 2024-05-21 202621.png" alt="drawing" width="500"/>
