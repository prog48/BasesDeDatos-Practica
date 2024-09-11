# BasesDeDatos-Practica

  ## Descripción:
    Este repositorio está diseñado con el objetivo que el usuario aprenda sobre la gestión de repositorios en GitHub y el manejo básico de Bases de Datos

  ## Instrucciones de Instalación:
    Para el corecto uso del material aportado en este repositorio se debe contar con una serie de requisitos mínimos. Entre ellos están:
      - Acceso a GitHub a través de conexión a Internet, y la url -----
      - Tener Instalada en la PC (local), las aplicaciones Git o GitHub Desktop para la gestion con Git y GitHub, y una versión actualizada de MySql con Un IDE para la interacción con MySql. Como IDE para la interacción con MySql se recomienda MySQL Workbench.

 ## Uso:
    A continuación algunos ejemplos de consultas SQL  y creacion de tablas:
     - CREATE TABLE `empleado` (
                                  `idempleado` int NOT NULL,
                                  `nombre_e` varchar(100) DEFAULT NULL,
                                  `iddepartamento` int DEFAULT NULL,
                                  PRIMARY KEY (`idempleado`),
                                  KEY `fk_empleado_departamento_idx` (`iddepartamento`),
                                  CONSTRAINT `fk_empleado_departamento` FOREIGN KEY (`iddepartamento`) REFERENCES `departamento` (`iddepartamento`)
                                ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
    - SELECT d.nombred AS Departamento, e.nombre_e AS Empleado
      FROM departamento d
      RIGHT JOIN empleado e ON d.iddepartamento = e.iddepartamento;

## Contribución: 

## Licencia:
  MIT, se ha escogido esta licencia por su permitividad, creando asi mejores posibilidades para el parendizaje en el desarrollo y testeo de proyectos de bases de datos en el entorno Git  
   
