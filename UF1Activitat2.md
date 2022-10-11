# Activitat 2 - Pràctica amb llenguatges.

PER PARELLES:
Ara que ja coneixeu uns quants llenguatges de programació el que farem serà
crear un programa d’exemple.
El programa simplement ha de generar un número aleatori de l’1 al 6 i
s’anomenarà “d6”, simula el llançament d’un dau de 6 cares.
Heu de crear al repositori de GitHub MP05UF1 un fitxer de text nou anomenat
UF1Activitat2.md que confingui la següent informació:
Escolliu 3 llenguatges de programació, un de compilat, un d’interpretat i un de MV


#### Per al llenguatge compilat (C++):
# **Activitat 2 - Pràctica amb llenguatges.**

PER PARELLES:
Ara que ja coneixeu uns quants llenguatges de programació el que farem serà
crear un programa d’exemple.  

El programa simplement ha de generar un número aleatori de l’1 al 6 i
s’anomenarà “d6”, simula el llançament d’un dau de 6 cares.
Heu de crear al repositori de GitHub MP05UF1 un fitxer de text nou anomenat
UF1Activitat2.md que confingui la següent informació:

Escolliu 3 llenguatges de programació, un de compilat, un d’interpretat i un de MV.

---
**Per al llenguatge compilat:**

● Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament  
escriureu el programa en un fitxer de text que sigui el codi font, el codi font
l’adjunteu dins el document.    

Abans de res, hem de **instal·lar** el següent paquet, per a poder utilitzar el comando **"gcc"**, que es el que ens permetrà transformar un arxiu en extensió **".c"** a executable mitjançant el comando **./(nom_de_l'arxiu)** a **Ubuntu**.

  ![image](https://user-images.githubusercontent.com/113585897/194006531-4a53f241-13ff-487b-a149-15e41f7b7168.png)      



El programa simplement genera un número aleatori de **l’1 al 6** i, simula el llançament d’un **dau de 6 cares**
```
#include <stdio.h>
#include <stdlib.h>

int main()

{
    int randomnumber;
    srand(time(NULL));
    randomnumber = rand() % 6;
    printf("%d\n", randomnumber);
    return 0;
}
```

  ![image](https://user-images.githubusercontent.com/113585897/194005594-2839c610-5947-4af5-83f7-fe6fd06b823e.png)  

La comanda **gcc dado.c -o prova2.c** serveix per transformar l'arxiu a executable. D'aquesta manera podrem utilitzar el **./(nom_de_l'arxiu)** i executar-lo

  ![image](https://user-images.githubusercontent.com/113585897/194005507-4c9f0de7-c0cf-4f1a-ba04-8194e4348bf4.png)  

Si l'executem mes d'una vegada, podem veure que dona resultats diferents.

  ![image](https://user-images.githubusercontent.com/113585897/194005840-380ab257-262e-4f06-baa3-c4e928946617.png)  

● Identifiqueu el compilador real que utilitzeu (nom de l’executable) i la
comanda per utilitzar-lo per passar de codi font a codi objecte.  

El nom del compilador que utilitzem en aquest cas es "GCC" i serveix per C tant com per C++.  
El comando que utilitzem es **gcc arxiu1.c -o arxiu2.c**  

● Descriviu com passar de codi font a codi objecte.

Mitjançant un procés que es diu "Compilació". Aquest procés s'encarrega de traduir un programa escrit en llenguatge font.


● Mostreu les extensions dels fitxers de codi font i codi objecte.  

L'extensió predeterminada per **C** es **".c"**

![image](https://user-images.githubusercontent.com/113585897/194008617-101b499a-f6c0-437c-993e-3319c727e8ef.png)

● Descriviu com passar de codi objecte a executable.  

Mitjançant un procés que es diu "Enllaçador" o, "Linker" en anglès.
El "Linker" es un programa que ajuda a enllaçar mòduls d'objectes d'un programa en un sol fitxer d'objectes.

● Expliqueu els avantatges d’utilitzar un llenguatge compilat i els punts febles.  

Avantatges: Es pot separar de l'entorn de desenvolupament, executar-se de manera independent en una plataforma específica i té una eficiència més gran.

Desavantatges: no es pot trasplantar; cal trasplantar, recopilació del codi font.

● Busqueu 3 IDEs de desenvolupament pel llenguatge.  
Els IDEs més utilitzats en ordre per a C són:

1. Visual Studio Code  
2. Eclipse  
3. NetBeans
---

#### Per al llenguatge interpretat (PHP):
● Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament
escriureu el programa en un fitxer de text que sigui el codi font, el codi font
l’adjunteu dins el document.

● Identifiqueu l'intèrpret del llenguatge (l’executable).

![image](https://user-images.githubusercontent.com/114953110/194021975-7d6d922f-6459-4ec0-ba69-49cc944b1e16.png)





● Descriviu com funciona l’intèrpret.
● Mostreu les extensions dels fitxers de codi font.
● Expliqueu els avantatges d’utilitzar un llenguatge interpretat i els punts febles.
● Busqueu 3 IDEs de desenvolupament pel llenguatge

#### Per al llenguatge de MV (Java - JVM):
● Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament
escriureu el programa en un fitxer de text que sigui el codi font, el codi font
l’adjunteu dins el document.

```
public class activitat2 {

	public static void main (String[] args) {
	
		int min = 0;
		int max = 6;
		
		int d6 = (int)Math.floor(Math.random()*(max-min+1)+min);
		System.out.println(d6);
	}
}
```

● Identifiqueu el compilador real (nom d’executable) que utilitzeu i la comanda
per utilitzar-lo per passar de codi font a ByteCode.

el compilador de java es javac, l'instal·lem d'aquesta forma

![image](https://user-images.githubusercontent.com/114953110/194002865-8fffa9a6-10e1-43a0-81ed-2908c04fba90.png)
![image](https://user-images.githubusercontent.com/114953110/194005745-d13f7453-df8a-4878-8113-b3273d9ae24b.png)

i el fem servir aixi

![image](https://user-images.githubusercontent.com/114953110/194005893-e1d778c5-01bb-45a7-90ee-68e72426c7c9.png)

si no surt cap error significa que javac ha compilat de forma correcta

● Descriviu com passar de codi font a ByteCode.

una vegada afetgim la extensio .java al nostre codi font es genera l'arxiu .class que es on guarda el ByteCode

● Mostreu les extensions dels fitxers de codi font i ByteCode.

codi font: .java ![image](https://user-images.githubusercontent.com/114953110/194004922-cfd67e0f-9902-4cc9-81c1-a2dbc7ff46da.png)


ByteCode: .class ![image](https://user-images.githubusercontent.com/114953110/194004891-7e87433f-631c-403f-8bae-9e638684ec71.png)


● Descriviu com executar el programa.

una vegada instal·lem javac podem utilitzar la comanda 

```
java activitat2.java
```

![image](https://user-images.githubusercontent.com/114953110/194003109-c02080d9-a66d-40d6-9693-33fae90d8920.png)



● Expliqueu els avantatges d’utilitzar un llenguatge de MV i els punts febles.

- Avantatges:

1. En el cas especific de Java la gran ventatja que te es que tel JVM que es un entorn de maquina virtual que executa programes d'aquest llenguatge
2. El codi de bytes de Java s'escriu una vegada i despres s'executa en multiples plataformes. No te que ser portat a un entornde hardware en especific ja que s'executa en JVM
3. La maquina virtual de Java s'ha incorporat en les caracteristiques de seguretat. Evita tambe que el software malintencionat posi en perill el Sistema Operatiu


- Punts febles:

1. Els programes Java exectutas en JVM solen tenir un rendiment mes lent que els programes equivalents a escrits amb C++. La neuralitat del sistema de codis de Byte actua com una desventatja quan es trata de rendiment
2. JVM te que estar lliure de errors per a que el programa funcioni correctament, aquesta dependencia de JVM introdueix un posible punt de fallo per a que el programa funcioni correctament
3. Com a espasa de doble fulla tansols podrem utilitzar un programa de java amb JVM 



● Busqueu 3 IDEs de desenvolupament pel llenguatge. 

- **Intelij IDEA**

![image](https://user-images.githubusercontent.com/114953110/194006880-5e863724-48c4-4456-acb1-bdccc49f1a1a.png)


- **Eclipse IDE**

![image](https://user-images.githubusercontent.com/114953110/194006679-5e9b2ed8-0831-456b-8df6-0bdd4544f737.png)

- **Apache NetBeans**

![image](https://user-images.githubusercontent.com/114953110/194006811-121e08d0-44ce-49d2-bacd-c6d9d8df0eef.png)



##### Recordeu corregir les faltes d’ortografia.
##### Presentar el document de forma ordenada amb capçaleres adients i imatges de reforç.
##### El codi del programa fiqueu-lo dins del tag ``` codi ```.
##### Indiqueu la webgrafia utilitzada.

**c++**



**php**

https://www.geeksforgeeks.org/php-rand-function/
https://php.watch/articles/compile-php-ubuntu

**java**

https://www.educative.io/answers/how-to-generate-random-numbers-in-java

https://muylinux.xyz/como-ejecutar-programas-java-en-la-terminal-en-ubuntu-y-otros-linux/

https://geekflare.com/es/top-java-ide-and-online-compilers/

https://www.seabrookewindows.com/DMRkaEmWw/

https://adictoalcodigo.blogspot.com/2016/07/ventajas-y-desventajas-de-programar-en.html




