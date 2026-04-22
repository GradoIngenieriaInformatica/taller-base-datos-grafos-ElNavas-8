MATCH (p:Persona)-[:TRABAJA_EN]->(e:Empresa)
RETURN e.nombre, count(p) AS total_empleados
ORDER BY total_empleados DESC;
