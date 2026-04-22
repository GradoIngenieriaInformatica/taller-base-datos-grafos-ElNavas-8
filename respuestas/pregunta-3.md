MATCH (p:Persona)-[:TRABAJA_EN]->(e:Empresa) 
RETURN e.nombre, count(p) AS num_empleados 
ORDER BY num_empleados DESC