Proyecto de Arquitectura de Datos: Northwind OLTP \& DW

Este repositorio contiene el desarrollo de una solución integral de datos basada en el dominio de ventas de Northwind. El proyecto abarca desde el diseño transaccional (OLTP) hasta el modelado analítico (Data Warehouse) y su empaquetado profesional.



📋 Resumen del Proyecto

Dominio: Gestión de Ventas y Distribución.



Tecnologías: SQL Server 2022, SSMS 22.5.2, GitHub.



Modelos: OLTP (Normalizado en 3FN) y Data Warehouse (Esquema Estrella).



🛠️ Estructura del Repositorio

/scripts: Scripts SQL para la creación de bases de datos y carga de datos.



/dacpac: Paquetes de despliegue de base de datos.



/docs: Documentación técnica y diagramas.



🏗️ 1. Modelo OLTP (Transaccional)

Se implementó un modelo normalizado para garantizar la integridad referencial y eliminar la redundancia de datos.



Entidades principales: Clientes, Pedidos, Productos, Categorías y Detalles de Pedido.



Normalización: Aplicada hasta la Tercera Forma Normal (3FN).



Datos de prueba: El script incluye más de 20 registros por tabla principal para validación de procesos.



📊 2. Modelo Data Warehouse (Analítico)

Diseñado para la toma de decisiones y análisis de Ciencia de Datos mediante un Modelo Estrella.



Tabla de Hechos (Fact\_Sales): Contiene métricas clave como cantidad vendida y montos totales.



Dimensiones:



Dim\_Product: Desnormalizada para reportes rápidos.



Dim\_Customer: Información demográfica de clientes.



Dim\_Date: Dimensión de tiempo para análisis de tendencias (ventas por mes/año).



📦 3. Empaquetado y Despliegue (DACPAC)

Para asegurar un despliegue profesional, se generaron archivos DACPAC. Estos archivos permiten recrear la estructura de la base de datos sin necesidad de ejecutar scripts manuales uno a uno.



Archivo: Northwind\_OLTP.dacpac



Método de despliegue: Mediante la opción "Publish Data-tier Application" en SQL Server Management Studio.



🚀 Instrucciones de Instalación

Clonar el repositorio: git clone \[URL-de-tu-repo].



Ejecutar el script /scripts/01\_Northwind\_OLTP\_Full.sql para crear la base transaccional con datos.



Ejecutar el script /scripts/02\_Northwind\_DW.sql para preparar el entorno analítico.



Opcionalmente, desplegar los archivos .dacpac desde SSMS.



Autor

Jorge Felix Zientarski Balderrama



Senior Consultant \& Database Administrator

El script incluye tanto la estructura como los datos de prueba.

