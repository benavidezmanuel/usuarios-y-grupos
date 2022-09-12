paso 1: corremos el comando adduser para agregar los nombres de nuestros padres y el nuestro para que el comando los reconozca

adduser Enrique , adduser Helena adduser Manuel

paso 2: despues ejecutaremos el comando groupadd para crear el grupo donde estaran los nombres

groupadd casa 

paso 3: usamos comando getent group y verficamos que el grupo se ha creado sin problemas el grupo junto con los nombres que colocamos

getent group casa

paso 4: ahora para que podamos modificar el monbre del grupo casa a familia ejecutamos el siguiente comando groupmod -n familia casa, no se preocupen 
por como se ve simplemente damos enter y vemos el resultado


paso 5: en esta parte volvemos a ejecutar el comando getent group para verificar el cambio de nombre de la siguiente manera

getent group familia

dato adicional: una vez que ejecutemos el comando nos tiene que mostrar el orden de nombres que insertamos ejemplo: (Enrique,Helena,Manuel) dentro del grupo familia
