Instrucciones para cargar correctamente ejercicio coperativa sancarlos:
1-empezamos metiendo 0_usuarios.csv del sistema
	configuracion/usuarios/usuarios/vista lista/importar/ 0_usuarios.csv
2-metemos los nombres de cuenta para cliente/proveedor(CONCILIACION AÑADIDA)
	contabilidad/configuracion/cuentas/cuentas/vista lista/importar/1_account_account.csv(EnekOdoo)
3-metemos clientes/provedores()
	ventas/clientes/vista lista/importar/2_clientes_proveedores.csv (AÑADIDOS CUENTAS IBAN APORTADAS POR JOSE LUIS)0102
4-metemos categorias del producto(correcion añadimos las categorias a todas / se pueden vender)
	ventas/configuracion/categorias y atributos de categoria/categorias de producto/importar/3_categorias.csv 
5-metemos atributo COLOR a mano
	ventas/configuracion/categorias y atributos de categoria/atributos/crear/COLOR 
6-metemos valores de atributo COLOR
	ventas/configuracion/categorias y atributos de categoria/valores de atributos/importar/4_attributes.csv
7-metemos articulos relacionandolos con su [categoria y su variantes]
	ventas/productos/productos/importar/5_productosok.csv
[EN ESTE CASO LA PORTABILIDAD DEL SIGUIENTE ARCHIVO SE DEBE A QUE TODOS TRABAJAMOS SOBRE UN CLON DE LA MISMA BASE DE DATOS]
8-metemos las reglas de reabastecimiento:(Aitor estabas en lo cierto algo raro pasaba en este punto)
	almacen/configuracion/reglas de reabastecimiento/importar/6_Reglas_abastecimientoServidorClase.csv
[EN CASO DE ERROR EN EL SIGUIENTE PASO, TIENES QUE EXPORTAR SOBRE TU BASE DE DATOS LAS VARIANTES DEL PRODUCTO VENTAS/PRODUCTOS/VARIANTES ]
