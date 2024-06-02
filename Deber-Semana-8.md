# Deber TAS7 - Events
## 1. Contar el número de productos de una categoría específica.
  - Sentencia:
  ```
  SELECT COUNT(*) 
FROM product 
WHERE category = 'Electronics';

  ```
  - Captura:

![Captura de pantalla 2024-06-02 092417](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/44bfaa2c-d80c-4c7f-ad84-1a159ee34624)


## 2. Contar el número de clientes en una ciudad específica.
  - Sentencia:
  ```
 SELECT COUNT(*) 
FROM client 
WHERE city = 'Quito';

  ```
  - Captura:

![Captura de pantalla 2024-06-02 093001](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/0292be7e-966e-4d5a-879e-d59f4f6a9354)



## 3. Contar el número de productos cuyo precio está dentro de un rango específico 
  - Sentencia:
  ```
 SELECT COUNT(*) 
FROM product 
WHERE price BETWEEN 100.00 AND 500.00;

  ```
  - Captura:

![Captura de pantalla 2024-06-02 093910](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/94ea95b5-308d-4c80-86d5-d7ef09f14a34)


## 4. Seleccionar clientes que viven en una ciudad específica y tienen un tipo de cliente específico

 - Sentencia:
  ```
SELECT * 
FROM client 
WHERE city = 'Quito' 
  AND type_of_client = 'PREMIUM';

  ```
  - Captura:

![Captura de pantalla 2024-06-02 094432](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/602678be-9f67-454d-aceb-f48796b681c8)


## 5. Seleccionar productos que pertenecen a una categoría específica y cuyo precio está por encima de un valor específico

 - Sentencia:
  ```
SELECT * 
FROM product 
WHERE category = 'Electronics' 
  AND price > 500.00;

  ```
  - Captura:

![Captura de pantalla 2024-06-02 094809](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/502d649a-2118-46a6-97b5-f3e80342ab2a)


## 6. Seleccionar productos que fueron producidos en un año específico y en un país de origen específico

 - Sentencia:
  ```
SELECT * 
FROM product 
WHERE year_of_production = 2023 
  AND country_of_origin = 'USA';

  ```
  - Captura:

![Captura de pantalla 2024-06-02 095210](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/7baf8f81-573e-44ad-8946-093c8b43701f)


## 6. Seleccionar clientes cuyo nombre completo comience con 'J'.

 - Sentencia:
  ```
SELECT * 
FROM client 
WHERE fullname LIKE 'J%';

  ```
  - Captura:

![Captura de pantalla 2024-06-02 095621](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/dfba4fdb-0251-44a6-a7dd-1cd32ea60e14)


## 6. Seleccionar clientes cuya ciudad contenga la letra 'a'
 - Sentencia:
  ```
SELECT * 
FROM client 
WHERE city LIKE '%a%';

  ```
  - Captura:

![Captura de pantalla 2024-06-02 095948](https://github.com/Nathaly222/Base-de-Datos/assets/146012550/d4984f5c-65bb-4936-9598-a57bc4bef8e0)

