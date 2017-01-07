Instrucciones para cargar correctamente ejercicio coperativa sancarlos:
1-empezamos metiendo 0_usuarios.csv del sistema
	configuracion/usuarios/usuarios/vista lista/importar/ 0_usuarios.csv
2-metemos los nombres de cuenta para cliente/proveedor
	contabilidad/configuracion/cuentas/cuentas/vista lista/importar/1_account_account.csv
3-metemos clientes/provedores
	ventas/clientes/vista lista/importar/2_clientes_proveedores.csv (codificacion win-1252,separador:Tabulacion)
4-metemos categorias del producto(correcion añadimos las categorias a todas / se pueden vender)
	ventas/configuracion/categorias y atributos de categoria/categorias de producto/importar/3_categorias.csv (codificacion win-1252,separador:Tabulacion)
5-metemos atributo COLOR a mano
	ventas/configuracion/categorias y atributos de categoria/atributos/crear/COLOR 
6-metemos valores de atributo COLOR
	ventas/configuracion/categorias y atributos de categoria/valores de atributos/importar/4_attributes.csv
7-metemos articulos relacionandolos con su [categoria y su variantes]
	ventas/productos/productos/importar/5_productosok.csv
[EN ESTE CASO LA PORTABILIDAD DEL SIGUIENTE ARCHIVO SE DEBE A QUE TODOS TRABAJAMOS SOBRE UN CLON DE LA MISMA BASE DE DATOS]
8-metemos las reglas de reabastecimiento:
	almacen/configuracion/reglas de reabastecimiento/importar/6_Reglas_Abastecimiento_Servidor_Clase.csv
[EN CASO DE ERROR EN EL SIGUIENTE PASO, TIENES QUE EXPORTAR SOBRE TU BASE DE DATOS LAS VARIANTES DEL PRODUCTO VENTAS/PRODUCTOS/VARIANTES DE PRODUCTO/ORDENADO POR NOMBRE Y EXPORTA, SELECINAS NOMBRE PARA COMPROBAR QUE LA EXPORTACION LO HACE ALFABETICAMENTE, COJES LA COLUMNA ID LA COPIAS Y LA PEGAS SOBRE LA COLUMNA D DEL ARCHIVO 6_Reglas_Abastecimiento_Servidor_Clase.csv(este archivo lo abres como una hoja de calculo) LA RENOMBRAS CON product_id/id LA GUARDAS Y YA TENDRIAS EL ARCHIVO LISTO PARA IMPORTARLO.]
