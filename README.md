# descripcion_De_pandas2

+ import pandas as pd: what it does is important the necessary libraries

+ users = pd.read_csv('https://raw.githubusercontent.com/justmarkham/DAT8/master/data/u.user', 
                      sep='|', index_col='user_id'): lo que hace es buscar la base de datos del link y usar como user_id como la primaria.
                      
+users.head(26): lo que hace es mostrar el numero de datos que se escriban dentro del parentesis

+ users.tail(11) a diferencia del head este muestra pero desde el ultimo, el head inicia desde el principio este inicia desde el final los numeros de datos

users.shape[0] lo que hace es mostrar de forma vertical y horizontal, con el 0 muestra de vertical cuantos datos hay en esa fila y si usamos el 1 muestra de forma horizontal las columnas de arriba que divide los datos.

users.columns: este comando muestra las columnas, la diferencia del shape es que muestra numero y este muestra con nombres y tipo.

users.index: esto muestra los datos totales que hay en forma de numeros.

users.dtypes: muestra el tipo de dato que es si es int64 o object

users['occupation'] muestra junto con el id el orden en el que esta y alado la fila que seleccionamos mostrar, muestra id correspondiente junto lo que queremos ver.

users.occupation.nunique(): muestra los diferentes datos que tiene, si hay datos repetidos encuentra todos y muestra como solo 1.

users.occupation.value_counts().head(1).index[0]: de todos los datos muestra cual es el mas usado o el mas repetido de todos y se busca escribiendo la fila de cual queremos saber que se repite.

users.describe(include = "all"): esto describe todo de la base de datos, la cantidad, el tipo, porcentaje, etc.

users.occupation.describe() resume solo la columna en espesifico mostrando el dato mas usado, el tipo de datos, cuantos datos y la frecuencia usada

round(users.age.mean()) muestra la edad promedio de la base de datos que son los usuarios.

users.age.value_counts().tail(): muestra la edad que menos es usada los que menos se usan de todos a si como puede mostrar el de las otras tablas.
