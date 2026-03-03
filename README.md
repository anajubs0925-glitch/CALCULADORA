
import java.util.Scanner;

public class Calculadora {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Digite o primeiro número:");
        int a = sc.nextInt();

        System.out.println("Digite o segundo número:");
        int b = sc.nextInt();

        System.out.println("Escolha a operação:");
        System.out.println("1 - Soma");
        System.out.println("2 - Subtração");
        System.out.println("3 - Divisão");
        System.out.println("4 - Multiplicação");

        int op = sc.nextInt();

        switch (op) {

            case 1:
                System.out.println("Resultado: " + (a + b));
                break;

            case 2:
                System.out.println("Resultado: " + (a - b));
                break;

            case 3:
                if (b != 0) {
                    System.out.println("Resultado: " + (a / b));
                } else {
                    System.out.println("Não é possível dividir por zero.");
                }
                break;

            case 4:
                System.out.println("Resultado: " + (a * b));
                break;

            default:
                System.out.println("Opção inválida!");
        }

        sc.close();
    }
}
