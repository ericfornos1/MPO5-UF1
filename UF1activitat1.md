
# Python

- *Naixement, creadors i evolució històrica.*

A finals dels 80 Guido van Rossum va crear el llenguatje Python, va començar a implementarlo al decembre del 89 i el febrer del 91
va publicar la primera versio publica (0.9.0) la 1.0 al 94, la 2.0 al 2000 i la 3.0 al 2008.

fins el 2018 el desenvolupament de python ha estat dirigit per Guido van Rossum, amb la fundacio "Python Software Foundation". El juliol de 2018
Guido anuncia que deixara que dirigit el desenvolupament de python llavors des-de 2019 el desenvolupament de python ha estat dirigit per un consell de 5 membres escollits entre els desarrolladors de python y que cada any es renoven

- *Característiques del llenguatge.*

**Programacio orientada a Objectes**: aixo significa que el codi s'organitza en unitats denominades clases i objectes, aixo permet representar conceptes cotidians en un programa

**multiplataforma**: Aquest esta disponibles en els principals sistemes operatius.. Linux, Windows, Unix, MacOS... es a dir que aquest pot ser executat en casi cualsevol sistepa operatiu sempre i quan porti un interpret adequat

**Tipat Dinamic**: Aixo permet que les variables no tinguin que especificar el seu tipus, aquestes adopten un tipus en funcio del valor que se li assigne

**Open Source**: Python es un llenguatge de codi obert, per lo que no requereix de llicencies de pago per treballar amb ell

**Ampliament respatllat** Les sebes caracteristiques i funcionalitats fan que aquest llenguatge siqui molt interessant. Per aixo, python ha generat una comunitat d'usuaris molt gran al seu alrededor que pot ser utilitzada quan volem trovar informacio o demanar ajuda per desenvolupar el codi

- *Imperatiu, declaratiu, OOP...*

**Imperatiu** ja que li indiquem una secuencia de operacions que ha de realitzar

- *Compilat, interpretat, híbrid...*

**Llenguatge interpretat**: No es necessari compilar amb Python ja que els interpretes que utilitzen aquest llenguatge s'encarreguen d'executar els programes a traves d'escripts propis

- *Avantatges i inconvenients respecte altres llenguatges.*

Les principals avantatges de python son:

-Llenguatge "facil" d'utilitzar comparat amb altres llenguatges
-Es polivalent, es pot utilitzar per desenvolupar software, scrips de web, GUI d'escriptori, data science...
-Te una amplia coleccio de biblioteques i frameworks
-compatibilitat amb qualsevol sistema operatiu
-gratis i de codi obert
-comunitat molt forta 

i alguns dels inconvenients son

-alt consum de memoria
-lentitut
-el desenvolupament per a movil no es el seu fort

- *Principals entorns on es fa servir el llenguatge.*

python tot i que es pot fer utilitzar en molts entorns, principalment es fa utilitzar per desenvolupar llocs web i software automatitzacio de tasques, analisi de dades
i visualitzacio de dades 

- *Exemple de codi (valoraré especialment si mostreu que ho heu implementat i provat).*

**Aquest codi de python esta fet per mi, el vaig fer l'any passat a smx per el treball de final de curs on teniem un servidor i habiem de implementar serveis web, moodle, xarxa local amb dhcp dns... i una de les coses que tenia que fer jo era control·lar quan el processador passes de certa temperatura, tambe es un exemple de que amb python es pot fer un programa sencill amb poques linees**

```
import wmi
import time
from tkinter import messagebox

w = wmi.WMI(namespace= "root/OpenHardwareMonitor")
temperature_infos = w.Sensor()

def temperatura():
        for sensor in temperature_infos:
            if sensor.SensorType==u'Temperature':
                if sensor.Value > 60 and sensor.Name == ("CPU Core #2"):
                    messagebox.showerror("cpu safe temp exceded", "Please check the refrigeration system from the CPD or reboot the server, if the problem persists call the technician")
                   
                    
def init():
    while True:
        temperatura()
        time.sleep(15)

init()
```

- *Hola mòn (Molt fàcil de trobar).*

``` print("Hola Mon") ```

- *Demanar el nom a l'usuari i mostrar-lo (haureu de buscar una mica més).*

```
name = input("Enter your name: ")
print("Hello", name + "!")
```

- *Buscar com estan les ofertes de treball a Infojobs del llenguatge.*

![image](https://user-images.githubusercontent.com/95549844/192841068-ab464341-9625-43ba-9fb7-9bea2ddf1591.png)

aqui es veu que hi han moltes ofertes de treball buscan python i de segur cada dia en surten moltes mes

- *WebGrafia.*

https://www.mikedane.com/programming-languages/python/getting-user-input/
https://www.mclibre.org/consultar/python/otros/historia.html
https://keepcoding.io/blog/ventajas-y-desventajas-de-python/
https://similaranswer.es/para-que-se-usa-principalmente-python/

# Java

- *Naixement, creadors i evolució històrica.*

Java va naixer el 1991 desarrollat en els seus inicis per James Gosling conegut principalment amb el nom "OAK" posteriorment cambiat a Green per problemes legals, finalment amb la denominacio actual Java.

La primera versio del llenguatge Java es publicada per Sun Microsystems en el 1995 i es en la versio del llenguatge JDK 1.0.2 al 1996 quan pasa a dir-se Java

- *Característiques del llenguatge.*

les principals caracteristiques de java son:

- Orientacio a objectes
- Es robust el que significa que realitza verificacions en busca de problemes
- la seva seguretat elimina en el llenguatge caracteristiques com els punters o el casting implicit que fan els compiladors de C i C++, d'aquesta forma s'empidex el acces il·legal a la memoria 
- es un llenguatge porbale 

- *Imperatiu, declaratiu, OOP...*

java es un llenguatge imperatiu, segueix una serie de indicacions que ha de seguir

- *Compilat, interpretat, híbrid...*

java es un llenguatge interpretat per tant no es compila

- *Avantatges i inconvenients respecte altres llenguatges.*

avantatges:

-curva d'aprenentatje curta
-multiplataforma
-lliberacio de memoria
-compatible amb llibreries estandar i editor
-ofereix gestio d'errors

inconvenients

-requereix experiencia de programacio
-es de sintaxis complexa
-es depenent del JVM
-els codis escrits son detallats 

- *Principals entorns on es fa servir el llenguatge.*

s'utilitza per a entorns d'aplicacions GUI d'escriptori, aplicacions web, aplicacions movils, aplicacions empresarials, " " cientifiques, servidors web i d'aplicacions, sistemes integrats..

- *Exemple de codi (valoraré especialment si mostreu que ho heu implementat i provat).*

Aques codi quan l'executes mostra de -50 fins 50 dient si el numero es parell o imparell

```
public class exercicibucle {
    public static void main(String[] args) {
        byte comptador =-50;

        while (comptador <= 50){
            System.out.print(comptador+ " es ");
            if(comptador % 2 == 0) System.out.println(" parell");
            else System.out.println(" imparell");
            comptador = (byte) (comptador+1);
        }
        System.out.println("has sortit del bucle");
    }
}
```

![image](https://user-images.githubusercontent.com/95549844/193092044-55489547-5e59-4208-9ab8-864bac9c5653.png)


- *Hola mòn (Molt fàcil de trobar).*

``` 
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!"); 
    }
}
```

- *Demanar el nom a l'usuari i mostrar-lo (haureu de buscar una mica més).*

```
import java.util.Scanner;

public class hellouser {
    public static void main(String[] args) {
        Scanner input  = new Scanner(System.in);
        System.out.println("Enter your Name");
        String nom = input.next();

        System.out.println("Hello "+ nom);
    }
}
```

- *Buscar com estan les ofertes de treball a Infojobs del llenguatge.*

![image](https://user-images.githubusercontent.com/95549844/193028215-971871eb-754e-4440-8ada-a711eb6f3ed0.png)

en infojobs hi han mes ofertes de java que no de python


- *WebGrafia.*

https://www.crehana.com/blog/desarrollo-web/ventajas-desventajas-java/
http://www.itlp.edu.mx/web/java/Tutorial%20de%20Java/Intro/carac.html
https://www.manualweb.net/java/historia-java/#:~:text=El%20lenguaje%20Java%20fue%20desarrollado,Java%2C%20corr%C3%ADa%20el%20a%C3%B1o%201996.
https://spa.myservername.com/what-is-java-used

# C#

- *Naixement, creadors i evolució històrica.*

Andrés Hejlsberg va decidir formaar al 1999 un equip de treball per crear un nou llenguatge de programacio, al principi el nom inicial va ser Cool (c Object Oriented Language) que avui en dia coneixem com C#.

la seba primera versio era molt semblant a Java, de fet aquest va ser creat per ser una alternativa de Java

- *Característiques del llenguatge.*

les caracteristiques principals d'aquest llenguatge son:

-sintaxis sencilla
-sistema de tipo unificat (permet realitzar operacions comuns i que tots els valors es puguin emmagatzemar transportar i utilitzar de forma coherent)
-orientacio a components (pots definir propietats sense necessitat de crear metodes)
-Biblioteques de clases
-Integracions amb altres llenguatges 
-multifil, pots dividir el codi en multiples execucions treball en paral·lel..

- *Imperatiu, declaratiu, OOP...*

C# es un llenguatge de tipus imperatiu

- *Compilat, interpretat, híbrid...*

es un llenguatge que es compila a un llenguatge intermig i despres aquest es compilat al codi de cada maquina la primera vegada que s'utilitza

- *Avantatges i inconvenients respecte altres llenguatges.*

avantatges:

-Declaracions a l'espai de noms: en començar a programar alguna cosa, es pot definir una o més classes dins d'un mateix espai de noms. 
-Tipus de dades: a C# hi ha un rang més ampli i definit de tipus de dades que els que es troben a C, C++ o Java. 
-Atributs: cada membre d'una classe té un atribut daccés del tipus públic, protegit, intern, intern protegit i privat. 
-Pas de paràmetres: aquí es pot declarar els mètodes perquè acceptin un nombre variable de paràmetres. Per defecte, el passi de paràmetres és per valor, tret que s'utilitzi la paraula reservada ref, la qual indica que el passi és per referència.

Els inconvenints:

-els principals inconvenients es la portabilitat i la dificultat del desenvolupament d'un software complet amb C#
-la curva d'aprenetatge es mes llarga
-la biblioteca que porta per defecte no es molt amplia i es tenen que utilitzar de tercers

- *Principals entorns on es fa servir el llenguatge.*

Aquest llenguatge es utilitzat majoritariament per fer videojocs, l'utilitza el motor grafic "unity" per escriure els scripts

- *Exemple de codi (valoraré especialment si mostreu que ho heu implementat i provat).*

Aquest codi el que fa es crear un directori

```
namespace EjemploCrearDirectorio
{
    class Program
    {
        static void Main(string[] args)
        {
            string ruta = @"D:\dev\proyCs\archivos\directorio_nuevo";
            if (!Directory.Exists(ruta))
            {
                Console.WriteLine("Creando el directorio: {0}", ruta);
                DirectoryInfo di = Directory.CreateDirectory(ruta);
            }
            Console.WriteLine("Presiona Enter para terminar.");
            var name = Console.ReadLine();
        }
    }
```

- *Hola mòn (Molt fàcil de trobar).*

```
namespace HelloWorld
{
    class Hello {         
        static void Main(string[] args)
        {
            System.Console.WriteLine("Hello World!");
        }
    }
}
```

- *Demanar el nom a l'usuari i mostrar-lo (haureu de buscar una mica més).*

```
class MainClass {
  public static void Main (string[] args) {
    Console.WriteLine ("Please enter your name:");
    string name = Console.ReadLine();
    Console.WriteLine("Hello {0}", name); 
   }
}
```

- *Buscar com estan les ofertes de treball a Infojobs del llenguatge.*

![image](https://user-images.githubusercontent.com/95549844/193122352-06e038de-291d-482f-b175-b1f4bd6cce22.png)


- *WebGrafia.*

https://social.msdn.microsoft.com/Forums/es-ES/6a73a0de-2d41-4df7-8fcc-56bc7fc913d8/intrpretes-c?forum=vcses#:~:text=C%23%20no%20es%20interpretado%2C%20es,primera%20vez%20que%20se%20ejecuta.
https://www.tokioschool.com/noticias/c-que-es/#:~:text=Andr%C3%A9s%20Hejlsberg%20decidi%C3%B3%20formar%20un,de%20programaci%C3%B3n%20orientado%20a%20objetivos.
https://es.quora.com/Cu%C3%A1les-son-las-ventajas-y-desventajas-de-C
http://programacion1abundiz.blogspot.com/2009/09/ventajas-del-c-y-desventajas.html


# SQL

- *Naixement, creadors i evolució històrica.*

La historia de SQL començla al 1969 quan l'investigador de IBM Edgar F. Codd definex el model de base de dades relacional. Aquest model es basa en la asociacio de <<claus>> amb varies dades.

Uns anys mes tard IBM va crear un lenguatge per als sistemes de gestio de bases relacionals basades en el traball de Codd, que es va dir SEQUEL <<Structured English Query Language>> i mes tard despres de variesimplementacions i revisions van pasar a dir-se SQL
    
Les proves van començar el 1978, i després IBM va començar a desenvolupar productes comercials com SQL/DS el 1981 i DB2 el 1983. El van seguir altres proveïdors, com Sybase, Ingres o Oracle, que va llançar el seu primer producte el 1979.



- *Característiques del llenguatge.*
        
-Integritat de dades, amb aixo ens referim a que les dades siguin correctes i completes      
-Llenguatge estandaritzat, aixo vol dir que es poden desplegar implementacions del mateix llenguatge en diferents sistemes
-Sencillez i claritat sql es un llenguatge integral desde el punt de vista conceptual, aixo vol dir que sql es un llenguatge unificat, clar simple i de facil comprension
-Flexibilitat, sql es un llenguatge flexible a la hora d'implantar solucions
       

- *Imperatiu, declaratiu, OOP...*

sql es un llenguatge declaratiu osigue que el codi l'escrivim de forma clara i objectiva      

- *Compilat, interpretat, híbrid...*

sql es un llenguatge interpretat, osigue no existeixen pasos complexes de compilacio ni de edicio de enllaços i resultats inmediats

- *Avantatges i inconvenients respecte altres llenguatges.*

 Els avantatges de sql son
        
-Portabilitat
-Escritura simple
-Estandars ben definits
        
i els inconvenients
   
-dificultats de creixement, quan aquestes base de dades començen a creixer l'almacenament i el cost de manteniment es un problema
-complexitat en la instal·lacio, algunes base de dades sql es veuen condicionades per el sistema operatiu en el que funcionaran i els requisits dels servidors i ordenadors
-dificultat en la interfaç, son mes complexes que afetgir alguna linea de codi

        
- *Principals entorns on es fa servir el llenguatge.*
        
s'utilitzen mes en la salud, la banca, educacio, telecomunicacions, defensa....
        
- *Hola mòn (Molt fàcil de trobar).*
    
 ```       
 CREATE TABLE helloworld (phrase TEXT);
INSERT INTO helloworld VALUES ("Hello, World!");
INSERT INTO helloworld VALUES ("Goodbye, World!");
SELECT COUNT(*) FROM helloworld;       

SELECT * FROM helloworld WHERE phrase = "Hello, World!";
```
- *Buscar com estan les ofertes de treball a Infojobs del llenguatge.*

![image](https://user-images.githubusercontent.com/95549844/193333582-a235f6c9-d805-4471-82ef-632e78a2aa50.png)


- *WebGrafia.*
        
https://www.learnsqlonline.org/en/Hello,_World!#:~:text=Here%20is%20the%20basic%20syntax,equal%20to%20Hello%2C%20World!%20.
https://guidocutipa.blog.bo/principales-ventajas-desventajas-bases-de-datos-relacionales-no-relacionales-nosql-vs-sql/
https://bigdata-analytics.es/sql/       
https://datascientest.com/es/sql-todo-lo-que-necesitas-saber-sobre-el-lenguaje-de-programacion-de-bases-de-datos#:~:text=La%20historia%20de%20SQL%20comienza,y%20un%20n%C3%BAmero%20de%20tel%C3%A9fono.
