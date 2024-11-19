# API_Categoria

## POST: Crear Categoria
```json
{
  "categoriaID": "C12345",
  "nombre": "Categoria de Ejemplo",
  "descripcion": "Descripción detallada de la categoría."
}
```
## GET: Consultar Categoria
```
Query Params (solo uno es necesario, tenantID o categoriaID):
tenantID: "202411-123e4567-e89b-12d3-a456-426614174000"
categoriaID: "C12345"
```
## PUT: Actualizar Categoría
```json
{
  "categoriaID": "C12345",
  "tenantID": "202411-123e4567-e89b-12d3-a456-426614174000",
  "nombre": "Categoria actualizada",
  "descripcion": "Nueva descripción"
}
```
## DELETE: Eliminar Categoría
```json
{
  "categoriaID": "C12345",
  "tenantID": "202411-123e4567-e89b-12d3-a456-426614174000"
}
```
## GET: Listar Categorías
```
Query Params (opcional para paginación):
limit: "10" (cantidad máxima de categorías por página)
lastEvaluatedKey: "{\"categoriaID\": \"C12345\", \"tenantID\": \"202411-123e4567-e89b-12d3-a456-426614174000\"}" (para continuar desde la última categoría evaluada)
```

## ENDPOINTS:
```
  POST - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/categorias/create
  GET - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/categorias/get
  PUT - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/categorias/update
  DELETE - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/categorias/delete
  GET - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/categorias/list
```
