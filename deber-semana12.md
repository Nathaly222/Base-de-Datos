# Deber TAS12 - views
## 1. Crear una vista que muestre la lista de productos comprados por los clientes con las siguientes columnas: 
  - Sentencia:
  ```
SELECT c.fullname, i.create_at, p.description, d.quantity
FROM 
    client c
JOIN 
    invoice i ON c.id = i.client_id
JOIN 
    detail d ON i.id = d.invoice_id
JOIN 
    product p ON d.product_id = p.id;

  ```
  - Captura:
![Captura de pantalla 2024-06-26 223815](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/77014441-e5ef-4531-a620-05788c6e07a1)


## 2. Crear una vista donde se muestre la lista de miembros registrados a las conferencias.
  - Sentencia:
  ```
SELECT c.title, r.code, m.fullname
 FROM member m
JOIN 
  register r ON  m.id = r.member_id
JOIN
  conference c ON r.conference_id = c.id;

  ```
  - Captura:
![Captura de pantalla 2024-06-26 224651](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/11dbf9d3-9d9b-4be3-9a05-9fee1bee8eb6)
