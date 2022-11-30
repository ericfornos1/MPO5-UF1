# Activitats: 

Per dibuixar els diagrames de flux podeu fer servir [draw.io](https://draw.io) o qualsevol altra eina online.

1. Calcula el CC de les següents figures:
  - ![image](https://user-images.githubusercontent.com/110727546/204613022-4ab64342-2e06-438d-a7e8-570685b3c406.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204613180-6d55bf09-28b8-417e-96f4-f71a762ac44c.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204655229-8c3f28d7-3d8b-4746-a55d-331f89da39d2.png)


 - **Resultat 1:**

5

  - **Resultat 2:**
 
5

  - **Resultat 3:**

6


2. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:
  - ![image](https://user-images.githubusercontent.com/110727546/204615125-363e5e6c-173b-4ec0-8c0b-cb97985ade06.png)

  - **Diagrama:**

![image](https://user-images.githubusercontent.com/113585897/204740229-7b4e9264-2fec-474d-9791-370ffd019b7a.png)




  - **Resultat CC:**

3


3. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:

```
public class proves {
    public static  String queEmPoso(int temperatura) {
        String roba = "res";
        if(temperatura<0){
           roba = "roba d'esquiar";
        }
        else if(temperatura<10){
           roba = "roba de muntanya";
        }
        else if(temperatura<20){
           roba = "roba d'hivern";
        }
        else if(temperatura<30){
           roba = "roba d'estiu";
        }
        return roba;
    }    
}
```

  - **Diagrama:**

![image](https://user-images.githubusercontent.com/113585897/204746007-84f6cfd0-9e5b-4ef0-af2c-5f201f93e495.png)


  - **Resultat CC:**

3

  - **Resultat proves camins:**

temperatura = -1 = roba = "roba d'esquiar"


temperatura = 9 = roba = "roba de muntanya"


temperatura = 19 = roba = "roba d'hivern"


temperatura 29 = roba = "roba d'estiu"



4. Dibuixa el diagrama de flux representat per aquest codi, calcula la seva CC i crea una prova per a cada camí posible:

```
    public static Boolean llumsEncesos(int hora) {
        Boolean llums = false;
        if(hora <= 8 || hora >= 20){
            llums = true;
        }
        return llums;
    }
```
  - **Diagrama:**



  - **Resultat CC:**




       


5. Investiga sobre les proves de caixa negra:

  - Què són?

Una caixa negra és, en teoria de sistemes, aquell element que és estudiat des del punt de vista de les entrades que rep i les sortides o respostes que produeix, sense tenir en compte el seu funcionament intern.


  - Quina diferència principal tenen sobre les de caixa blanca?


La principal diferencia entre una caixa blanca i una caixa negra es que la caixa blanca té en compte el funcionament i la caixa negra funciona sense tenir en compte el seu funcionament intern.



![image](https://user-images.githubusercontent.com/113585897/204749627-aeef2381-748c-4b7b-9f2f-ff053b29eb1b.png)


