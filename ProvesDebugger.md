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
