# TAS8 - Sentencia multiple where

## 1. Contar el número de productos de una categoría específica. 

- Sentencia:
```
SELECT COUNT (category) AS total_category
FROM product
WHERE category = 'Electronics';
```

- Captura

<img src="./capturas/Pasted image 20240602101949.png" alt="drawing0" width="500"/>
 
 ## 2. Contar el número de clientes en una ciudad específica.  

- Sentencia:
  
```
SELECT COUNT (city) AS total_city
FROM client
WHERE city = 'Cuenca'
```

- Captura

<img src="./capturas/Pasted image 20240602102448.png" alt="drawing0" width="500"/>

## 3. Contar el número de productos cuyo precio está dentro de un rango específico.

- Sentencia:

```
SELECT COUNT (price) AS price_total
FROM product
WHERE price >100 AND price < 500;
```

- Captura

<img src="./capturas/Pasted image 20240602105733.png" alt="drawing0" width="500"/>

## 4. Seleccionar clientes que viven en una ciudad específica y tienen un tipo de cliente específico.

- Sentencia:
  
```
SELECT * FROM client
WHERE city = 'Cuenca' AND type_of_client = 'VIP'
```

- Captura

<img src="./capturas/Pasted image 20240602110328.png" alt="drawing0" width="500"/>

## 5. Seleccionar productos que pertenecen a una categoría específica y cuyo precio está por encima de un valor específico.

- Sentencia:

```
SELECT * FROM product
WHERE category = 'Electronics' AND price > 500;
```

- Captura

<img src="./capturas/Pasted image 20240602114251.png" alt="drawing0" width="500"/>

## 6. Seleccionar productos que fueron producidos en un año específico y en un país de origen específico.

- Sentencia:

```
SELECT * FROM product
WHERE year_of_production = '2021' AND country_of_origin = 'Japan'
```

- Captura

<img src="./capturas/Pasted image 20240602115130.png" alt="drawing0" width="500"/>

## 7. Seleccionar clientes cuyo nombre completo comience con 'J'.  

- Sentencia:

```
SELECT * FROM client
WHERE fullname LIKE 'J%';
```

- Captura

<img src="./capturas/Pasted image 20240602115454.png" alt="drawing0" width="500"/>

## 8. Seleccionar clientes cuya ciudad contenga la letra 'a'.

- Sentencia:

```
SELECT * FROM client
WHERE city LIKE '%a%';
```

- Captura

<img src="./capturas/Pasted image 20240602115956.png" alt="drawing0" width="500"/>
