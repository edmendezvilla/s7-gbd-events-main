obtener la edad promedio de los miembros:
  - Sentencia:
 SELECT AVG(EXTRACT(YEAR FROM AGE(NOW(), dateOfBirth))) AS edad_promedio
FROM Members;


<img src="![alt text](image.png)" 

obtener la edad mínima de los miembros:
  - Sentencia:
 SELECT MIN(EXTRACT(YEAR FROM AGE(NOW(), dateOfBirth))) AS edad_minima
FROM Members;
<img src="![alt text](image-1.png)" 

obtener el número total de registros asistidos:
  - Sentencia:
 SELECT COUNT(*) AS total_registros_asistidos
FROM Registrations
WHERE attendance_status = 'Attended';
<img src="![alt text](image-2.png)" 


obtener el número total de asistentes a todas las conferencias
  - Sentencia:
SELECT SUM(total_attendees) AS total_asistentes
FROM Events;
<img src="![alt text](image-3.png)" 

obtener el número total de eventos por cada ciudad:
  - Sentencia:
SELECT city, COUNT(*) AS total_eventos
FROM Events
GROUP BY city;
<img src="![alt text](image-4.png))" 

obtener el número de registros por cada miembro:
  - Sentencia:
SELECT member_id, COUNT(*) AS total_registros
FROM Registrations
GROUP BY member_id;
<img src="![alt text](image-5.png)" 

obtener el número de registros por cada conferencia:
  - Sentencia:
SELECT conference_id, COUNT(*) AS total_registros
FROM Registrations
GROUP BY conference_id;
<img src="![alt text](image-6.png)" 




