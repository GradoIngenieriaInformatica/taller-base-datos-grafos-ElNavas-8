MATCH (p:Persona)-[:AMIGO_DE]-(amigo:Persona),
      (p)-[:VIVE_EN]->(ciudad_p:Ciudad),
      (amigo)-[:VIVE_EN]->(ciudad_amigo:Ciudad)
WHERE ciudad_p <> ciudad_amigo
RETURN DISTINCT p.nombre;
