# Práctica 12 - Creación de un SQL Database

## Innovaccion Virtual (VII Edición) #IAWizards

### Semana 2 - Sesión 6

En esta práctica se creó un SQL Databse desde el portal de Azure con la terminal Bash.

------------------------------------------------------

#### Requerimientos 

- Cuenta de Azure con suscripción.

------------------------------------------------------

#### Pasos a seguir

1. Accediendo al siguiente link: [https://github.com/josejesusguzman/acordeon-az900-innovaccion/blob/main/res/consultas-sql.md](https://github.com/josejesusguzman/acordeon-az900-innovaccion/blob/main/res/consultas-sql.md) se encontrará con los comandos a usar para la realización de esta práctica, así como los recursos a necesitar. Como primer paso, se copiará el primer comando mostrado en el acordeón: 

`git clone https://github.com/MicrosoftLearning/DP-900T00A-Azure-Data-Fundamentals dp-900`

2. En el portal de Azure ingresamos a la terminal Bash y pegamos el comando previamente copiado para clonar un repositorio dentro de Azure.

![P12I1](Images\Sesión 6 - P12 01.PNG)

3. Al dar enter, se creará una serie de archivos y documentos. Entramos a una de estas carpetas a través del siguiente comando que se encuentra en el acordeón:

`cd dp-900/sql`

![P12I2](Images\Sesión 6 - P12 02.PNG)

4. Ejecutamos el siguiente comando y esperamos un rato a que se termine de ejecutar.

`bash setup.sh`

![P12I3](Images\Sesión 6 - P12 03.PNG)

5. Vamos a nuestro grupo de recursos y buscamos en el primer grupo de recurso creado (es mejor revisar todos los recursos creados) para verificar si se ha creado ahí la base de datos SQL y le damos en el apartado de ‘Información general’.

![P12I4](Images\Sesión 6 - P12 04.PNG)

![P12I5](Images\Sesión 6 - P12 05.PNG)

6. En Información general nos vamos al apartado de ‘Establecer firewall de servidor’ y en ‘Reglas de firewall’ le damos en ‘Agregar la dirección IPv4 el cliente’ y le damos en ‘Guardar’.

![P12I6](Images\Sesión 6 - P12 06.PNG)

7. Regresamos a la base de datos y le damos en el apartado de ‘Editor de consultas’ y nos logueamos con las credenciales localizadas en el siguiente link: [https://github.com/MicrosoftLearning/DP-900T00A-Azure-Data-Fundamentals/blob/master/sql/setup.sh](https://github.com/MicrosoftLearning/DP-900T00A-Azure-Data-Fundamentals/blob/master/sql/setup.sh)

![P12I7](Images\Sesión 6 - P12 07.PNG)

8. Para consultar los datos de alguna tabla, seleccionamos la cual queremos consultar (Inventory por ejemplo) y escribimos en ‘Consulta 1’: `SELECT * FROM Inventory` y le damos en ‘Ejecutar’. Con el comando: `SELECT * FROM CustomerOrder` muestra la relación entre las tablas.

![P12I8](Images\Sesión 6 - P12 08.PNG)

9. Para agregar un dato, podemos escribir lo siguiente: `INSERT INTO Inventory (Id, Inventory.Name, Stock) values(7, ‘Strawberry’, 500)`; y para leer esto se realiza lo siguiente: `SELECT * FROM Inventory`.

![P12I9](Images\Sesión 6 - P12 09.PNG)

![P12I10](Images\Sesión 6 - P12 10.PNG)