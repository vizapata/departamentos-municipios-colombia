# Departamentos y Municipios de Colombia

Este plugin provee una lista de los departamentos y municipios de Colombia actualizada con base en la información disponible en el portal de datos abiertos: https://www.datos.gov.co/en/Mapas-Nacionales/DEPARTAMENTOS/25e3-npng

Lista de funciones disponibles:
- `dmcol_all`: Lista de todos los departamentos con sus respectivos municipios
- `dmcol_by_state_name`: Detalles de un departamento específico según el nombre del departamento
- `dmcol_by_state_name_and_city_name`: Detalles de un municipio según el nombre del departamento y del municipio
- `dmcol_city_state_by_state_name_and_city_name`: Detalles combinados de un departamento y municipio con base en el nombre del departamento y del municipio. 

Ejemplo: 
```php
$details = dmcol_city_state_by_state_name_and_city_name('ANTIOQUIA', 'MEDELLÍN');

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

