MATCH (p:Persona)-[]-(:Proyecto)
RETURN DISTINCT p.nombre;
