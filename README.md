¿Cuántas filas devuelve cada consulta y por qué son distintas? 
Explicá con ejemplos concretos de los datos qué filas se eliminaron con UNION.
La consulta que utiliza "UNION" devuelve 11 filas, y la otra 14 filas. Son distintas ya 
que la consulta con UNION elimina los duplicados.

¿Por qué UNION ALL es más eficiente que UNION? 
UNION ALL es más eficiente que UNION ya que no tiene que consultar qué filas están duplicadas y eliminarlas.
Esto hace más rápida la consulta.

¿Qué operación adicional realiza UNION internamente que consume más recursos?
La operación adicional que realiza UNION internamente es ver las filas duplicadas en ambas tablas.

¿En qué casos de negocio usarías cada uno? Dá al menos dos ejemplos reales distintos
a los del ejercicio.
La consulta con UNION es útil cuando se quiere consultar listados (de productos, clientes, producto terminado,
materias primas), la consulta UNION ALL es útil cuando se necesita toda la información,
por ejemplo, ante un inventario o información sobre ventas o costos.

¿Qué pasa si las columnas de ambas consultas no coinciden en número o tipo? ¿Qué error genera SQL?
No se van a poder unir las tablas, y va a devolver el siguiente error:
"All queries combined using a UNION, INTERSECT or EXCEPT operator must have an equal number of expressions in their target lists."
