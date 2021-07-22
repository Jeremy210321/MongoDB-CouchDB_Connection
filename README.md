# MongoDB-CouchDB_Connection
### Conección entre MongoDB y CouchDB



**Los integrantes del grupo son:**

Daniel Guachamín → @DanielGuachamin
Cindy Yazán → @Cindyk2052
Jeremy León → @Jeremy210321

1. Se creo un nuevo Proyecto en Mongo DB Atlas, con el nombre de Ejercicio Colleccitions

![image](https://user-images.githubusercontent.com/66692550/126083137-3e4e13b6-d9e1-4962-9b09-55288b4b8203.png)

![image](https://user-images.githubusercontent.com/66692550/126083146-b1c9d335-f82e-4ba3-9cc6-18c222403e3a.png)

2. A continuación se ha creado el Cluster para realizar la conexión MongoDB Compass

![image](https://user-images.githubusercontent.com/66692550/126083150-1e140a20-eda5-4a9b-a578-e3c51ab12046.png)

3. Una vez creado el Cluster,  se da el acceso a cualquier persona, se debe añadir la dirección IP, junto con un usuario y contraseña

![image](https://user-images.githubusercontent.com/66692550/126083160-c770668b-b281-45d6-b531-affd69d29c24.png)

![image](https://user-images.githubusercontent.com/66692550/126083164-27be8b82-5137-48c1-b1ff-2e6ed2a6fd37.png)

4. En el Cluster se elige la opción de Conectar con MongoDB Compass, se presentará un string para conectarse a la base de datos en Compass. 

![image](https://user-images.githubusercontent.com/66692550/126083169-da2b1738-860c-49b2-a6be-98a63a64a399.png)

5. Continuamos con la creación de una nueva base de datos con el nombre de ExerciseCollections y también la inserción de una colección.

![image](https://user-images.githubusercontent.com/66692550/126083170-79ff043e-a7ab-4cad-b964-2de6e17ab71d.png)

6. Los integrantes se conectaron a la base de datos por medio de la cadena de string anterior y crearon una colección cada uno.

![image](https://user-images.githubusercontent.com/66692550/126083173-3356f38f-ae0e-44b6-b442-edf890883dc3.png)

7. Luego se insertaron los documentos obtenidos de los Datasets de Kaggle, cada integrante del equipo eligió una base de datos de su preferencia para subirlos en la base de datos (ExerciseCollections)

![image](https://user-images.githubusercontent.com/66692550/126083177-335863bb-2221-4595-8887-cda68110d515.png)

8. En el IDE jupyter para Python, se procedió a instalar argparse, pymongo, snappy, gssapi, srv, tls y bson para luego utilizarlos.

![image](https://user-images.githubusercontent.com/66692550/126083180-a0af5248-d994-4fe1-97fe-340fe4bb8944.png)
![image](https://user-images.githubusercontent.com/66692550/126084334-5e1d17cd-b504-4559-8a99-64a7d3ed20d6.png)

9. Ahora se debe dirigir a MongoDB Atlas para generar una conexión por aplicación.

![image](https://user-images.githubusercontent.com/66692550/126083185-eac689c0-ef22-4059-90b6-a649e87f7612.png)

![image](https://user-images.githubusercontent.com/66692550/126083186-e1eb77af-b83f-4fbd-8ad2-2f5eff640c8a.png)

10. En DRIVER se selecciona el lenguaje Python con versión de 3.12 o más y se copia el string de conexión que está a continuación.

![image](https://user-images.githubusercontent.com/66692550/126083190-dfcda3c2-104a-4079-b17e-70f33d9b4e49.png)

11. En el script de “mongo2couch.py” se cambian algunos campos. En el URL se ponen las credenciales de CouchDB. En la sección CLIENT se pega el string generado anteriormente (no olvidar cambiar la contraseña con la que se creó la base de datos en Atlas). Se debe colocar el nombre de la base de datos de MongoDB Atlas en DBS y finalmente darle un nombre a la base de datos de CouchDB. Esta última es a la cual se copiarán los datos de Atlas. 

![image](https://user-images.githubusercontent.com/66692550/126083194-b68b1c36-5ca3-4830-802f-3dc5bc4b4dc4.png)

![image](https://user-images.githubusercontent.com/66692550/126083199-5da1e8f1-be92-4824-9acc-fee73b1a020c.png)

![image](https://user-images.githubusercontent.com/66692550/126083202-52334bcd-074c-4ef1-b72f-8b090abab991.png)

![image](https://user-images.githubusercontent.com/66692550/126083208-ea243b6f-ace0-45df-86ba-300296e75c46.png)


Los resultados se reflejan en la siguiente imagen. Todos los datos de MongoDB Atlas se han copiado a la base de datos “mongo_destino6” de CouchDB.

![image](https://user-images.githubusercontent.com/66692550/126084393-f361ee7b-d033-4f81-b03c-d6ef3eb82bf1.png)

El script utilizado para la conección es 
[MongoCouch.py](https://github.com/Jeremy210321/MongoDB-CouchDB_Connection/blob/master/MongoCouch.py)

