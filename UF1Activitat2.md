# Activitat 2 - Pràctica amb llenguatges.

PER PARELLES:
Ara que ja coneixeu uns quants llenguatges de programació el que farem serà
crear un programa d’exemple.
El programa simplement ha de generar un número aleatori de l’1 al 6 i
s’anomenarà “d6”, simula el llançament d’un dau de 6 cares.
Heu de crear al repositori de GitHub MP05UF1 un fitxer de text nou anomenat
UF1Activitat2.md que confingui la següent informació:
Escolliu 3 llenguatges de programació, un de compilat, un d’interpretat i un de MV


#### Per al llenguatge compilat:
● Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament
escriureu el programa en un fitxer de text que sigui el codi font, el codi font
l’adjunteu dins el document.
● Identifiqueu el compilador real que utilitzeu (nom de l’executable) i la
comanda per utilitzar-lo per passar de codi font a codi objecte.
● Descriviu com passar de codi font a codi objecte.
● Mostreu les extensions dels fitxers de codi font i codi objecte.
● Descriviu com passar de codi objecte a executable.
● Expliqueu els avantatges d’utilitzar un llenguatge compilat i els punts febles.
● Busqueu 3 IDEs de desenvolupament pel llenguatge.

#### Per al llenguatge interpretat:
● Utilitzant la línia de comandes, sense utilitzar un IDE de desenvolupament
escriureu el programa en un fitxer de text que sigui el codi font, el codi font
l’adjunteu dins el document.
● Identifiqueu l'intèrpret del llenguatge (l’executable).
● Descriviu com funciona l’intèrpret.
● Mostreu les extensions dels fitxers de codi font.
● Expliqueu els avantatges d’utilitzar un llenguatge interpretat i els punts febles.
● Busqueu 3 IDEs de desenvolupament pel llenguatge

#### Per al llenguatge de MV:
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

● Busqueu 3 IDEs de desenvolupament pel llenguatge. 

##### Recordeu corregir les faltes d’ortografia.
##### Presentar el document de forma ordenada amb capçaleres adients i imatges de
##### reforç.
##### El codi del programa fiqueu-lo dins del tag ``` codi ```.
##### Indiqueu la webgrafia utilitzada.

https://www.educative.io/answers/how-to-generate-random-numbers-in-java
https://muylinux.xyz/como-ejecutar-programas-java-en-la-terminal-en-ubuntu-y-otros-linux/

