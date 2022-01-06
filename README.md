# HackthonGo

##  Desafío
En el sistema de ventas de Fantasy Products, se perdieron los datos de la base de datos, pero alguien antes de que
se rompiera pudo descargar unos archivos .txt que hacen referencia a las tablas que se borraron (tienen algunas
cosillas que hay que ver y acomodar, pero están los datos)

Se puede observar en el repositorio de GitHub dentro de la carpeta data que hay 4 archivos, es decir,
4 tablas (sales.txt, products.txt, invoices.txt, customers.txt), cada uno de ellos tiene los registros de dicha tabla.

Se sabe que los campos y el orden de cada tabla son:

sales.txt 💸 id, id_product, id_invoice, quantity
products.txt 🛒 id, description, price
invoices.txt 🧾 id, datetime, id_customer, total
customers.txt 👨‍💼 id, last_name, first_name, condition

Objetivos
Como se habrá dado cuenta, la tabla de facturas, perdió el dato de total, por lo tanto es necesario que usted
pueda recalcular con los datos que dispone entre sales, invoices y products.

Escribir una API que pueda:
- Crear los distintos INSERT en la base de datos desde el repository.
- Crear los distintos UPDATE que sean necesarios para modificar los datos.
- Tener un endpoint que pueda importar cada uno de los archivos en las tablas de la base de datos (que deberá crear).
- Por último se te pide alcanzar un porcentaje de cobertura tanto para el repository como para el service mayor o igual al 80%.

Consultas a realizar:
Montos totales redondeados a 2 decimales por condition del customer
Salida esperada

Condition                                   Total

Inactivo                                 95035592564.67
Bloqueado                                58831557301.94
Activo                                   72408070525.46


Top 5 de los products más vendidos
Salida esperada

Description                                 Total

Gatorade - Cool Blue Raspberry           268586.4
Arctic Char - Fresh, Whole               224348.5
Yoplait Drink                            224082
Sesame Seed Black                        224017.5
Huck Towels White                        223943.4


El Top 5 de los customers ordenados por last_name que compraron el product más barato.
Salida esperada

Last_name                                  First_name

Braganca                                 Willa
Close                                    Cody
Flaherty                                 Stavro
Kaliszewski                              Norby
Pleat                                    Ajay

##