# Lista Comandos Básicos de MONGO db

- Muestra las bases de datos que tengamos
```
show dbs 
```
- Muestra el nombre de la base actual en la que nos encontramos
```
db  
```
- Nos permite crear una base o usar una base de datos creada
```
use namedb 
```
- Nos muestra las colecciones que tenemos 
```
show collections         
```
- Nos permite crear una colección
```
db.createCollection("nameNewCollection")       
```
-  Nos permite eliminar una colección
```
db.nameCollections.drop()          
```
- Nos permite ingresar un dato en formato Json 
```
db.nameCollection.insert({dataFormatJson})          
```
- Nos permite ingresar datos en una lista de manera mas rápida
```
db.nameCollection.insert([{dataFormatJson},{dataFormatJson}])    
```
- Nos permite visualizar todos los datos
```
db.namecollection.find()      
```
-  Nos permite visualizar los datos especificando cuantos quiero ver 
```
db.namecollection.find().limit(number) 
```
- Nos permite visualizar los datos por Id  
```
db.namecollection.find({"_id":ObjectId("numberId")})  
```
-  Nos permire visualizar los datos de manera ordenada
```
db.namecollection.find().sort({parameter: 1 }) 
```
- Nos permite visualizar datos y especificar el atributo de busqueda
```
db.namecollection.find({parameter:"data"})        
```
- Nos permite visualizar y mostrar un datos especifico que quiera

```
db.namecollection.find({parameter:"data"},{parameter: 1 })  
```
-  Nos permite actualizar un documento entero 
```
db.namecollection.update({parameter:"data"},{parameter:"data"}) 
```
- Nos permite actualizar un dato en especifico
```
db.namecollection.update({parameter:"data"},{$set:{parameter:"data"}}) 
```
- Nos permite actualizar incrementando un dato numérico        
```
db.namecollection.update({parameter:"data"},{$inc:{parameter:data}})     
```
- Nos permite actualizar el nombre de un atributo 
```
db.namecollection.update({parameter:"data"},{$rename:{parameter:"newName"}}) 
```
-  Nos permite eliminar el documento que especifiquemos
```
db.namecollection.remove({parameter:"data"})     
```
- Nos permite eliminar todo 
```
db.namecollection.remove({})                                              
```


  




