# da
create database actividad3;

use actividad3;

create table actividad(
 id INT PRIMARY KEY,
 nombre VARCHAR(255),
 edad INT
);

CREATE TABLE actividad3(
 id INT PRIMARY KEY AUTO_INCREMENT,
 nombre VARCHAR(255),
 edad INT
);

CREATE TABLE padre (
 id INT PRIMARY KEY,
 nombre VARCHAR(255)
);

CREATE TABLE hija (
 id INT PRIMARY KEY,
 nombre VARCHAR(255),
 tabla_padre_id INT,
 FOREIGN KEY (tabla_padre_id) REFERENCES padre(id)
);
