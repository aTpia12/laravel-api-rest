1.- Ejecutar el siguinete comando para instalar Passport:
    - composer require laravel/passport
    
2.- Ejecutar las migraciones para las tablas en la BD

3.- Probando desde Postman el metodo register (Para registrar usuarios). 
    * http://localhost:8000/api/register. 
    * En los headers configurar KEY = Accept, VALUE = application/json. 
    * En el body, seleccionamos x-www-form-urlencoded y enviamos los siguientes parametros.     
        - name = "Nombre de usuario". 
        - email = "Email de usuario". 
        - password = "Contraseña". 
        - password_confirmation = "Repetir password". 
        : Una vez ralizado el envio obtendremos la respuesta con los datos del usuario creado asi como su token de accessToken. 
4.- Probando login de usuario desde Postman. 
    * http://localhost:8000/api/login. 
    * En el body, utilizar la siguiente configuracion. 
        - email = "email registrado previamente". 
        - password = "password de usuario registrado". 
        : Obtendremos la informacion del usuario mas su token
