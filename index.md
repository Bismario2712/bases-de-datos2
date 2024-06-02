create database bases_de_datos;
use bases_de_datos;

create table empleados(id_empleado int primary key, nombre_emp varchar(20), apellido_emp varchar (15));

create table clientes(id_clientes int primary key AUTO_INCREMENT, nombre_clien varchar(20), apellido_clien varchar (15));

CREATE TABLE tabla_padre (id INT PRIMARY KEY, nombre VARCHAR(255));

 CREATE TABLE tabla_hija (id INT PRIMARY KEY, nombre VARCHAR(255), tabla_padre_id INT, FOREIGN KEY (tabla_padre_id) REFERENCES tabla_padre(id));