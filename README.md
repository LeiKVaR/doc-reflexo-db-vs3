
## Módulo 1 - Architect
Este módulo contiene toda la funcionalidad de autenticación, usuarios, permisos y roles del sistema, reorganizada en una estructura modular y mantenible.

### Tabla Base
---

|     Atributos    |   Tipo de Datos   |         Restricciones        |
|------------------|-------------------|------------------------------|
|id		           |    INT(20)        |                              |
|name              |    VARCHAR(255)   |                        |
|description       |    VARCHAR(255)   |                        |
|created_at        |    TIMESTAMP      |                        |
|updated_at        |    TIMESTAMP      |                        |
|deleted_at        |    TIMESTAMP      |                        |

---

| Atributos   | Tipo de Datos   | Restricciones                                         |
|-------------|-----------------|-------------------------------------------------------|
| created_at  | DATETIME        | DEFAULT CURRENT_TIMESTAMP                             |
| updated_at  | DATETIME        | DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP |
| is_active   | TINYINT(1)      | DEFAULT 1                                             |

---

## Módulo 2 - 










## Módulo 4 - Therapists

|Atributos:            |	   Tipo de Datos   |       Restricciones      |
|----------------------|-----------------------|--------------------------|
|id                    |      INT(20)          |                          |
|document_number,      |	  VARCHAR(20)	   |			              |
|last_name_paternal,   |	  VARCHAR(100)     |			              |
|last_name_maternal,   |	  VARCHAR(100)	   |			              |
|first_name,           |      VARCHAR(100)     |			              |
|birth_date,           |	  DATETIME	       |			              |
|gender,               |      VARCHAR(20)	   |		        	      |
|personal_references,  |	  VARCHAR(255)	   |		        	      |
|is_active,            |	  TINYINT(1)	   |		        	      |
|phone,                |	  VARCHAR(15)	   |		        	      |
|email,                |	  VARCHAR(255)	   |		        	      |
|country,              |	  VARCHAR(100)	   |		        	      |
|department,           |	  VARCHAR(100)	   |		        	      |
|province,             |	  VARCHAR(100)	   |		        	      |
|district,             |	  VARCHAR(100)	   |		        	      |
|address,              |	  TEXT		       |		        	      |
|profile_picture       |	  VARCHAR(255)	   |		        	      |





## Módulo 7 - Therapists


# Tablas - Independientes

## Distrito

| **Atributos** | **Tipos de Datos** | **Descripción** |
|---------------|--------------------|-----------------|
| Id            | AutoField (PK)     | Identificador único del distrito |
| name          | VARCHAR(20)        | Nombre del distrito |
| province      | VARCHAR(20)        | Relación con la provincia a la que pertenece |
| deleted_at    | Date               | Fecha de eliminación lógica (soft delete) |
| ubigeo_code   | INTEGER            | Código UBIGEO de 6 dígitos |
| created_at    | VARCHAR            | Fecha de creación del registro |
| updated_at    | VARCHAR(20)        | Última fecha de actualización |

---

## Province

| **Atributos** | **Tipos de Datos** | **Descripción** |
|---------------|--------------------|-----------------|
| Id            | AutoField (PK)     | Identificador único de la provincia |
| name          | CharField          | Nombre de la provincia |
| región        | VARCHAR(20)        | Relación con la región a la que pertenece |
| deleted_at    | DateTimeField      | Fecha de eliminación lógica (soft delete) |
| ubigeo_code   | INTEGER            | Código UBIGEO de 4 dígitos |
| created_at    | DateTimeField      | Fecha de creación del registro |
| updated_at    | DateTimeField      | Última fecha de actualización |

---

## Región

| **Atributos** | **Tipos de Datos** | **Descripción** |
|---------------|--------------------|-----------------|
| Id            | AutoField (PK)     | Identificador único de la región |
| name          | CharField          | Nombre de la región |
| deleted_at    | DateTimeField      | Fecha de eliminación lógica (soft delete) |
| ubigeo_code   | INTEGER            | Código UBIGEO de 2 dígitos |
| created_at    | DateTimeField      | Fecha de creación del registro |
| updated_at    | DateTimeField      | Última fecha de actualización |