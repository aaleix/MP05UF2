public class Factorial {

    public static void main(String[] args) {
        System.out.println("El factorial del número és: " + facotorial(5));
    }

    public static int facotorial(int numero) {
        if (numero > 1) {
            return numero * facotorial(numero - 1);
        }
        return numero;
        }
    }

![image](https://user-images.githubusercontent.com/113586080/217348027-6b4288de-e5f4-4851-bd7a-06e4533ee0fe.png)



import java.util.Arrays;

public class TaularMultiplicar {
    public static void main(String[] args) {
        System.out.println(Arrays.toString(multiplicacions(4)));
    }
    public static int[] multiplicacions(int numero){
        int[] numerosTaula = new int[]{1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
        for (int i = 0; i < numerosTaula.length; i++) {
            numerosTaula[i] = numerosTaula[i] * numero;
        }
        return numerosTaula;
    }
}


![image](https://user-images.githubusercontent.com/113586080/217348186-d8f7e60b-5eee-4018-8f0a-9fe6ab702763.png)

