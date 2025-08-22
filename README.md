
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
