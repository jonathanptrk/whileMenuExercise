# whileMenuExercise
Como usuário eu gostaria de ter um menu visual que seja navegável através de números. O menu deve ser exibido da seguinte forma:  1. Calcular o imposto 2. Depositar salario 3. Sair  O menu deve ficar disponível em quanto eu nao digitar o numero 3. Dessa forma o sistema ficará em execução, evitando ter que ser reiniciado


/* Como usuário eu gostaria de ter um menu visual que seja navegável através de números.
O menu deve ser exibido da seguinte forma:

1. Calcular o imposto
2. Depositar salario
3. Sair

O menu deve ficar disponível em quanto eu nao digitar o numero 3.
Dessa forma o sistema ficará em execução, evitando ter que ser reiniciado. */


        package Testes;
        import java.util.Scanner;
        
        public class exercicioWhile2 {
            public static void main(String[] args) {

            Scanner teclado = new Scanner(System.in);        
            int opcao = 0;

            while(opcao != 3){
                System.out.println("Digite uma opção: ");
                System.out.println("1. Calcular imposto: ");
                System.out.println("2. Depositar salário: ");
                System.out.println("3. Sair: ");
                opcao = teclado.nextInt();

                if(opcao == 1){
                    System.out.println("Calcular imposto selecionado");
                    System.out.println("------------------------------------------------------------------------------------------");
                } else if (opcao == 2){
                    System.out.println("Depositar imposto selecionado");
                    System.out.println("------------------------------------------------------------------------------------------");
                } else if (opcao == 3){
                    break;
                } else {
                    System.out.println("Opcao inválida");
                    System.out.println("------------------------------------------------------------------------------------------");
            }
        }
    }
}
