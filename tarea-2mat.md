## 1.  Obtiene información de cada evento junto con el número de conferencias asociadas a cada uno. 
  - Sentencia:
  ```
SELECT 
    e.id,
    e.description,
    e.city,
    (SELECT COUNT(*) FROM conference WHERE conference.event_id = e.id) AS conference_count
FROM 
    event e;

  ```
## Captura 
![Captura de pantalla 2024-07-01 105409](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/1a6bc717-5757-45f2-9f84-12e8e9f49083)


## 2. Calcula el total de asistentes en todas las conferencias asociadas a cada evento.
  - Sentencia:
  ```
SELECT 
    e.id,
    e.description,
    e.city,
    (SELECT SUM(total_attendees) FROM conference WHERE conference.event_id = e.id) AS total_attendees_in_conferences
FROM 
    event e;

  ```
## Captura 
![Captura de pantalla 2024-07-01 104910](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/707e0c6c-c7fb-4e2f-b647-1b026675cd9f)

