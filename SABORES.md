package app;

import java.util.Scanner;

public class Sabores {

    public static void main(String[] args) {
        // Criação do Scanner para entrada de dados
        Scanner entrada = new Scanner(System.in);

        // Boas-vindas
        System.out.println("Bem-vindo à Snack Express!");
        System.out.println("Confira nosso cardápio:");

        // Exibição do cardápio
        System.out.println("1 - Hambúrguer Simples - R$12.0");
        System.out.println("2 - Cheeseburguer - R$15.0");
        System.out.println("3 - Hot Dog - R$10.0");
        System.out.println("4 - Batata Frita - R$8.0");
        System.out.println("5 - Refrigerante 350ml - R$5.0");
        System.out.println("6 - Suco Natural - R$6.0");
        System.out.println("7 - Salada Caesar - R$14.0");
        System.out.println("8 - Milkshake - R$12.0");

        // Solicitar a escolha do usuário
        System.out.print("Digite o número do item desejado: ");
        int escolha = entrada.nextInt();

        // Variáveis para armazenar o nome do item e preço
        String itemEscolhido = "";
        double preco = 0.0;

        // Estrutura condicional para definir item e preço
        if (escolha == 1) {
            itemEscolhido = "Hambúrguer Simples";
            preco = 12.0;
        } else if (escolha == 2) {
            itemEscolhido = "Cheeseburguer";
            preco = 15.0;
        } else if (escolha == 3) {
            itemEscolhido = "Hot Dog";
            preco = 10.0;
        } else if (escolha == 4) {
            itemEscolhido = "Batata Frita";
            preco = 8.0;
        } else if (escolha == 5) {
            itemEscolhido = "Refrigerante 350ml";
            preco = 5.0;
        } else if (escolha == 6) {
            itemEscolhido = "Suco Natural";
            preco = 6.0;
        } else if (escolha == 7) {
            itemEscolhido = "Salada Caesar";
            preco = 14.0;
        } else if (escolha == 8) {
            itemEscolhido = "Milkshake";
            preco = 12.0;
        } else {
            System.out.println("Opção inválida! Encerrando o pedido.");
            entrada.close();
            return;
        }

        // Exibir resumo do pedido
        System.out.println("\nResumo do Pedido:");
        System.out.println("Item escolhido: " + itemEscolhido);
        System.out.println("Valor total: R$" + preco);

        // Fechar o Scanner
        entrada.close();
    }
}
