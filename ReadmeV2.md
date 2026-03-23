¿Cuántas líneas de código habéis ahorrado al usar grupos?

attributeGroup datosGestion agrupa tres atributos (id, estado, ubicacion) que se repiten en <servidor> y <almacenamiento>, sin el grupo habría que escribirlos dos veces

group especificacionesTecnicas agrupa cpu, ram y discos. Sin el grupo habría que repetir ese bloque en cada tipo de servidor que lo necesite. En este catálogo se usa en un único punto, pero el bloque ocupa unas 20 líneas, si hubiera dos tipos de servidor distintos el ahorro sería de 20 líneas más.
En conclusión ahorramos entre 4 y 24 líneas, dependiendo de cuántos elementos reutilicen los grupos. La ventaja no es solo el ahorro de líneas sino que si hay que modificar un atributo, se cambia en un solo sitio.

¿Qué error os da VS Code si intentáis poner dos servidores con el mismo ID?

El subrayado rojo aparece directamente sobre el atributo id duplicado en el XML, y en el hover del error indica exactamente el nombre del xs:unique que no se está respetando, por ello es importante ponerle un nombre descriptivo como por ejemplo idServidorUnico.
