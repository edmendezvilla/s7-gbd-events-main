Contar el número de productos de una categoría específica.
  - Sentencia:
 SELECT COUNT(*) AS product_count
FROM product
WHERE category = 'Electronics';


<img src="![alt text](image.png)" 

Contar el número de clientes en una ciudad específica.
  - Sentencia:
  SELECT COUNT(*) AS client_count
FROM client
WHERE city = 'Quito';

  - Captura:

<img src="![alt text](image-1.png)" 

Contar el número de productos cuyo precio está dentro de un rango específico
 - Sentencia:
SELECT COUNT(*) AS product_count
FROM product
WHERE price BETWEEN 100 AND 500;

<img src="![alt text](image-2.png)" 
 
 Seleccionar clientes que viven en una ciudad específica y tienen un tipo de cliente específico
 - Sentencia:
 SELECT *
FROM client
WHERE city = 'Quito' AND type_of_client = 'Retail';
<img src="![alt text](image-3.png)" 


Seleccionar productos que pertenecen a una categoría específica y cuyo precio está por encima de un valor específico

 - Sentencia:
SELECT *
FROM product
WHERE category = 'Electronics' AND price > 1000;
<img src="![alt text](image-4.png)" 

Seleccionar productos que fueron producidos en un año específico y en un país de origen específico
- Sentencia:
SELECT *
FROM product
WHERE year_of_production = 2021 AND country_of_origin = 'USA';
<img src="![alt text](image-5.png)" 

Seleccionar clientes cuyo nombre completo comience con 'J'.
- Sentencia:
SELECT *
FROM client
WHERE fullname LIKE 'J%';
<img src="![alt text](image-6.png)" 

Seleccionar clientes cuya ciudad contenga la letra 'a'
- Sentencia:
SELECT *
FROM client
WHERE city LIKE '%a%';
<img src="![alt text](image-7.png)" 



