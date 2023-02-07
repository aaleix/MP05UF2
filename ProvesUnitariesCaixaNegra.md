public class PizzeriaPepe {

    public static void main(String[] args) {
        System.out.println(potCarregar(5));
    }

    public static boolean potCarregar(int pizzes){
        boolean pot = false;
        if(pizzes <=10 && pizzes >= 1){
            pot = true;
        }
        return pot;
    }
}

![image](https://user-images.githubusercontent.com/113586080/217350674-7972ae87-550c-4aa6-9206-6015a56d073f.png)

public class TransportsJeanClaude {
    public static void main(String[] args) {
        System.out.println(potPortar(500, 600));
    }
    public static int potPortar(int carrega, int capacitat){
        int resultat = -1;
        if (carrega>=500 && carrega<=900){
            if (capacitat>=500 && capacitat<=750){
                if (capacitat>=carrega){
                    resultat=0;
                }
            }

        }
        return resultat;
    }
}

![image](https://user-images.githubusercontent.com/113586080/217352476-972bb059-3d89-4e5c-a9b4-72e351566e65.png)


public class ControlTemperatura {

    public static void main(String[] args) {
        System.out.println(modificadorTemperatura(15, 20));
    }
    public static int modificadorTemperatura(int medidor, int termostat) {
        int resultat = -1;

        if (medidor > termostat) {
            resultat = 0;
        }

        int variableAuxiliar = Math.abs(termostat - medidor);
        if (variableAuxiliar >= 0 && variableAuxiliar <= 2) {
            resultat = 1;
        }
        variableAuxiliar=medidor-termostat;

        if (variableAuxiliar<-2){
            resultat=2;
        }
        if (medidor<-10 || medidor>50 || termostat<15 || termostat>40){
            resultat=-1;
        }
        return resultat;
    }
}

![image](https://user-images.githubusercontent.com/113586080/217352821-3063495a-19fb-4b86-bd5e-f32ea10fa23f.png)



