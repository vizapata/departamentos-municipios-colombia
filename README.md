# Departamentos y Municipios de Colombia

Este plugin provee una lista de los departamentos y municipios de Colombia con base en la información disponible en el portal de datos abiertos.

- URL Dataset: https://www.datos.gov.co/en/Mapas-Nacionales/DIVIPOLA-C-digos-municipios/gdxc-w37w
- Fecha de actualización dataset: 15 de diciembre de 2020

## Lista de funciones disponibles:
- `dmcol_all_states`: Lista de todos los departamentos con sus respectivos municipios
- `dmcol_get_state_by_name`: Detalles de un departamento específico según el nombre del departamento
- `dmcol_get_city_by_state_and_name`: Detalles de un municipio según el nombre del departamento y del municipio
- `dmcol_get_state_and_city_by_name`: Detalles combinados de un departamento y municipio con base en el nombre del departamento y del municipio. 

Ejemplo: 
```php
$details = dmcol_get_state_and_city_by_name('ANTIOQUIA', 'MEDELLÍN');

/*
Array
(
  [state_name] => ANTIOQUIA
  [state_code] => 05
  [city_code] => 05001
  [city_name] => MEDELLÍN
)
*/
```

## Nota
Es muy importante el uso correcto de mayúsculas y tildes. La búsqueda de la información se hace utilizando el mismo formato y nombres que los indicados en el dataset del portal de datos abiertos descrito al inicio de este documento.