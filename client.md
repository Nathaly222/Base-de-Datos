# Tarea en clase Semana 8
## La funcion count
###   Creacion de tabla
EEL siguiente codigo genera la tanla **client**
```
CREATE TABLE IF NOT client (
  id SERIAL,
  nui VARCHAR (10) NOT NULL,
  fullname VARCHAR (100) NOT NULL,
  phone VARCHAR (10),
  type_of_client VARCHAR (50) DEFAULT 'BASIC'
  city VARCHAR (50),
  credit_limit DECIMAL (7,2)
);
```

### Inserción de datos. 
```
INSERT INTO client (nui, fullname, phone, type_of_client, city, credit_limit) VALUES
('0123456789', 'Juan Perez', '0998765432', 'PREMIUM', 'Quito', 1500.00),
('0987654321', 'Maria Gomez', '0987654321', 'BASIC', 'Guayaquil', 800.00),
('1234567890', 'Luis Martinez', '0976543210', 'BASIC', 'Cuenca', 500.00),
('9876543210', 'Ana Torres', '0965432109', 'GOLD', 'Quito', 2000.00),
('2345678901', 'Carlos Ramirez', '0954321098', 'BASIC', 'Loja', 300.00),
('8765432109', 'Sofia Fernandez', '0943210987', 'SILVER', 'Manta', 1200.00),
('3456789012', 'Jose Vargas', '0932109876', 'PREMIUM', 'Ambato', 1800.00),
('7654321098', 'Rosa Diaz', '0921098765', 'GOLD', 'Santo Domingo', 2500.00),
('4567890123', 'Pedro Ruiz', '0910987654', 'BASIC', 'Esmeraldas', 600.00),
('6543210987', 'Elena Salazar', '0909876543', 'SILVER', 'Riobamba', 1000.00);

INSERT INTO client (nui, fullname, phone, type_of_client, city, credit_limit) VALUES
('5678901234', 'Luis Arboleda', NULL, 'BASIC', 'Machala', 700.00),
('6789012345', 'Patricia Suarez', NULL, 'GOLD', 'Portoviejo', 2500.00),
('7890123456', 'Diego Paz', NULL, 'PREMIUM', 'Ibarra', 1900.00),
('8901234567', 'Carmen Calderon', NULL, 'SILVER', 'Latacunga', 1200.00),
('9012345678', 'Andres Moreno', NULL, 'BASIC', 'Babahoyo', 500.00);

```
### Captura
![Captura de pantalla 2024-05-27 094139](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/66533699-2c4c-450a-8c3e-6672c635669a) 

### Mostrar total de nombres.
Para mostrar el total de nombres usamos la funcion **COUNT () ** pasandole como parametro el campo en este caos "fullname"
```
SELECT COUNT (fullname) AS total_names
FROM client;
```
### Captura
![Captura de pantalla 2024-05-27 094631](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/7302da99-765b-402e-ae49-58dec1cd9f54)

### Mostrar total de phone 

Para mostrar el total de números de teléfono en la tabla client, usamos la función **COUNT()** pasándole como parámetro el campo phone.
```
SELECT COUNT (phone) AS total_phone
FROM client;
```
### Captura

 ![Captura de pantalla 2024-05-27 095104](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/964310f3-0b1c-4d32-848a-19d1c603ca5c)

 ### Mostrar total phone and name 
 Para mostrar el total de números de teléfono y nombres completos, usamos la función **COUNT()**pasándole como parámetro los campos phone y fullname respectivamente. 
 ```
SELECT COUNT (phone) AS total_phone,COUNT (fullname) AS total_names
FROM client;
 ```
 ### Captura

![Captura de pantalla 2024-05-27 095217](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/7cb57187-9b0a-499f-a99c-8847a0e4c1b2)

### Mostar total de cities with DISTINCT
Para mostrar el total de ciudades únicas en la tabla client, usamos la función **COUNT() con el modificador DISTINCT** para contar únicamente los valores distintos. 
```
SELECT COUNT (DISTINCT city) AS total_cities
FROM client;
```
### Captura
![Captura de pantalla 2024-05-27 100024](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/5002bbfb-5155-490b-b05e-aedac3f372dc)








