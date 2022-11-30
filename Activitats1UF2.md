# Activitats: 

Per dibuixar els diagrames de flux podeu fer servir [draw.io](https://draw.io) o qualsevol altra eina online.

1. Calcula el CC de les següents figures:
  - ![image](https://user-images.githubusercontent.com/110727546/204613022-4ab64342-2e06-438d-a7e8-570685b3c406.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204613180-6d55bf09-28b8-417e-96f4-f71a762ac44c.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204655229-8c3f28d7-3d8b-4746-a55d-331f89da39d2.png)

  - **Resultat 1:** 17 camins - 14 nodes + 2 = 5
  - **Resultat 2:** 16 camins - 14 nodes + 2 = 4
  - **Resultat 3:** 8 camins - 6 nodes + 2 = 4


2. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:
  - ![image](https://user-images.githubusercontent.com/110727546/204615125-363e5e6c-173b-4ec0-8c0b-cb97985ade06.png)

  - **Diagrama:** ![image](https://user-images.githubusercontent.com/113586080/204739252-91dc8062-4e70-462e-bdd1-fcdc1d295bc3.png)


  - **Resultat CC:** 2 + 1 = 3

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

  - **Diagrama:** ![image](https://user-images.githubusercontent.com/113586080/204746505-66d671f3-bdb2-4ae2-b267-6802e339e2af.png)

  - **Resultat CC:** 4 + 1 = 5

  - **Resultat proves camins:** CAMI1= Roba=res
                                       Temperatura<0 true 
                                       Roba=roba d'esquiar
                                       Return roba
                                CAMI2= Roba=res
                                       Temperatura<0 false
                                       Temperatura<10 true
                                       Roba=roba de muntanya
                                       Return roba
                                CAMI3= Roba=res
                                       Temperatura<0 false
                                       Temperatura<10 false
                                       Temperatura<20 true
                                       Roba=roba d'hivern
                                       Return roba
                                CAMI4= Roba=res
                                       Temperatura<0 false
                                       Temperatura<10 false
                                       Temperatura<20 false
                                       Temperatura<30 true
                                       Roba=roba d'estiu
                                       Return roba
                                CAMI5= Roba=res
                                       Temperatura<0 false
                                       Temperatura<10 false
                                       Temperatura<20 false
                                       Temperatura<30 false
                                       Return roba

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
  - **Diagrama:** ![image](https://user-images.githubusercontent.com/113586080/204750603-0ee70d87-eb34-408f-9342-aa48fd333a7f.png)


  - **Resultat CC:** 2 + 1 = 3
  
  - **Resultat proves camins:** CAMI1= Llums=false
                                       Hora <= 8 true
                                       Llums=true
                                       Return llums
                                CAMI2= Llums=false
                                       Hora <= 8 false
                                       Hora >= 20 true
                                       Llums=true
                                       Return llums         
                                CAMI3= Llums=false
                                       Hora <= 8 false
                                       Hora >= 20 false
                                       Return llums
                              

5. Investiga sobre les proves de caixa negra:

  - Què són?
  - Quina diferència principal tenen sobre les de caixa blanca?
