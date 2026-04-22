MATCH (p1:Persona)-[:VIVE_EN]->(c1:Ciudad),
      (p1)-[:AMIGO_DE]-(p2:Persona)-[:VIVE_EN]->(c2:Ciudad)
WHERE c1 <> c2
RETURN DISTINCT p1.nombre