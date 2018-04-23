# README

Este repositorio se creó para realizar la entrega de la prueba de 'Rappi ML assessment' para la empresa Rappi. Todo el código fue desarrollado por Diego Fernando Trujillo Bedoya y es exclusivamente para validar conocimientos según la prueba


Por otro lado, el proyecto no posee la data. Pero corre simplemente si se tiene la data en la misma ubicación donde se descargue el programa en Python (jupyter notebook).

Los datos pueden encontrarse en el siguiente [link](https://drive.google.com/file/d/0B5XtSrqMH82icDlmME83NkNmaUE/view). En este repositorio también hay algunas imágenes que siguen un proceso de flujo de trabajo con las descripciones pertinentes.

Y estas son las directrices:


In this assignment, you will forecast the demand of a product for a given week, at a particular store. The dataset you are given consists of 9 weeks of sales transactions in Mexico. Every week, there are delivery boys that deliver products to the vendors. Each transaction consists of sales and returns. Returns are the products that are unsold and expired. The demand for a product in a certain week is defined as the sales this week subtracted by the return next week.

Things to note:
* There are duplicate Cliente_ID's in cliente_tabla, which means one Cliente_ID may have multiple NombreCliente that are very similar. This is due to the NombreCliente being noisy and not standardized in the raw data, so it is up to you to decide how to clean up and use this information.
* The adjusted demand (Demanda_uni_equil) is always >= 0 since demand should be either 0 or a positive value. The reason that Venta_uni_hoy - Dev_uni_proxima sometimes has negative values is that the returns records sometimes carry over a few weeks.


File descriptions
* data.csv — the training set
* cliente_tabla.csv — client names (can be joined with train/test on Cliente_ID)
* producto_tabla.csv — product names (can be joined with train/test on Producto_ID)
* town_state.csv — town and state (can be joined with train/test on Agencia_ID)



Data fields
* Semana — Week number (From Thursday to Wednesday)
* Agencia_ID — Sales Depot ID
* Canal_ID — Sales Channel ID
* Ruta_SAK — Route ID (Several routes = Sales Depot)
* Cliente_ID — Client ID
* NombreCliente — Client name
* Producto_ID — Product ID
* NombreProducto — Product Name
* Venta_uni_hoy — Sales unit this week (integer)
* Venta_hoy — Sales this week (unit: pesos)
* Dev_uni_proxima — Returns unit next week (integer)
* Dev_proxima — Returns next week (unit: pesos)
* Demanda_uni_equil — Adjusted Demand (integer) (This is the target you will predict)



Dataset
You can download the dataset here



