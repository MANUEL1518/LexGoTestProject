Documentación - **Prueba Técnica FullStack LEXGO**

Finalidad de este es mostrár organización y control de los datos usando
framework **Angular Javascript** con:

\- NodeJs Server

\- Angular Front Framework

\[+\] Sass / Transpilador CSS

\- Mongoose - ODM, Models/DB Request Manager

**\[CRUD\]:** Opciones para cambiar empleado/ejecutivo de departamento y
a su vez poder **Crear, Editar, Borrar** Empleados.

**Criterios de aceptación:**

\- Que sea permitido cambiar un Ejecutivo (Empleado con Sub-Empleados)
de departamento sin mover sus empleados heredados. en su lugar se pasan
los empleados al Departamento sin necesidad de moverlos junto al
Ejecutivo.

**\[TREE PATH\]**

**lexgoApp/src**

**lexgoApp_backend/application**

**Modelos Mongoose Empleados:**

\- **\[Company\]:**

company_id (primary)

company_name String:required

\- **\[Departament\]:**

departament_id **primary**

departament_name **String:required**

company :: **\[Company\] foreing**

\- **\[Employee\]:**

\*username **String:required**

\*role **String:required**

\*company **\[Company\] foreing**

\*departament **\[Departament\] foreing**

\*ejective **\[Employee\] foreing nullable**

**Backend EndPoints:**

**\[GET\]** \"/business_structure\"

**\[DELETE\]** \"/employee/:employee_id\"

**\[PUT\]** \"/employee/:employee_id\"

**\[POST\]** \"/employee\"

**- Documentación de Usuario -**

**\* Borrar Ejecutivo:**

\[1\]

\[2\]

\[3\]

**\* Crear Empleado:**

\[1\]

\[2\]

\[3\]

**\* Mover \[Empleado\] -\> \[Ejecutivo\]**

\[1\]

\[2\]

\[3\]

**\* Edit Employee:**

\[1\]

\[2\]

**- Documentación de Programador -**

En la carpeta se encuentra \"lexGoApp\" como frontEnd:

**\[Para iniciar\]**

**\> npm install**

**\> npm run start**

**Previamente se inicia la DB usando \"mongod.exe\" (previo instalado)**

**\* Como iniciar DB:**

**\> mongod \--dbpath \[dbpath\]**

**LexGoApp_backend**

\* Para correr **\"seeders\"** y aprovicionar la Base de datos:

**\[lexgoApp_backend\\application\\api\\seeders\]**

Aquí se encuentra el archivo que inicia y aproviciona la DB:

\* Para iniciar:

\> **node seed.js**

**\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_**

**\[Nota al pie\]:**

Dejo en usted sus observaciones sobre la organización de los modelos,
conexión con DB, UX/IU.

Me esforcé por enfocar el uso de la aplicación al intercambio standart
de delegados para un Lead.

Gracias por su atención

Manuel. H. Ponce
