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
