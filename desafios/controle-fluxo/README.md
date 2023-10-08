# trilha-java-basico

```markdown
# Desafio Controle de Fluxo

Projeto Java para contagem de números em um intervalo e tratamento de exceção personalizada.

## Descrição

Este projeto consiste em um programa Java que recebe dois números inteiros como entrada e realiza uma contagem de números dentro do intervalo entre esses dois números. Além disso, ele possui um tratamento de exceção personalizada (`ParametrosInvalidosException`) para lidar com casos em que o primeiro parâmetro é maior que o segundo.

## Conteúdo

- [Instruções de Uso](#instruções-de-uso)
- [Pré-requisitos](#pré-requisitos)
- [Instalação](#instalação)
- [Desafio Aplicado](#desafio-aplicado)
- [Contribuição](#contribuição)
- [Licença](#licença)

## Instruções de Uso

1. Clone este repositório em sua máquina local:

   ```bash
   git clone https://github.com/seu-usuario/DesafioControleFluxo.git
   ```

2. Compile o projeto:

   ```bash
   javac Contador.java
   ```

3. Execute o programa:

   ```bash
   java Contador
   ```

4. Siga as instruções para inserir os dois números inteiros.

## Pré-requisitos

- Java JDK instalado (versão 8 ou superior).

## Desafio Aplicado

Aqui está o código completo:

import java.util.Scanner;

// Classe de exceção personalizada
class ParametrosInvalidosException extends Exception {
    public ParametrosInvalidosException(String message) {
        super(message);
    }
}

public class Contador {
    public static void main(String[] args) {
        Scanner terminal = new Scanner(System.in);
        System.out.println("Digite o primeiro parâmetro");
        int parametroUm = terminal.nextInt();
        System.out.println("Digite o segundo parâmetro");
        int parametroDois = terminal.nextInt();

        try {
            contar(parametroUm, parametroDois);
        } catch (ParametrosInvalidosException e) {
            System.out.println(e.getMessage());
        }
    }

    static void contar(int parametroUm, int parametroDois) throws ParametrosInvalidosException {
        if (parametroUm > parametroDois) {
            throw new ParametrosInvalidosException("O segundo parâmetro deve ser maior que o primeiro");
        }

        int contagem = parametroDois - parametroUm + 1; // Adicione +1 para incluir o valor final
        for (int i = 1; i <= contagem; i++) {
            System.out.println("Imprimindo o número " + i);
        }
    }

Neste código:

Criamos a classe ParametrosInvalidosException que herda da classe Exception para criar nossa exceção personalizada com a mensagem desejada.

No método main, usamos um Scanner para obter os parâmetros digitados pelo usuário.

No método contar, verificamos se o primeiro parâmetro é maior que o segundo. Se for o caso, lançamos a exceção personalizada ParametrosInvalidosException. Caso contrário, calculamos a contagem e usamos um loop for para imprimir os números incrementados.

### Caso Válido

Se você fornecer os números 12 e 30 como entrada, o programa imprimirá os números de 1 a 19, pois há 19 números inteiros entre 12 e 30 (inclusive).

### Caso Inválido

Se você fornecer o primeiro parâmetro maior que o segundo, como 30 e 12, o programa lançará a exceção `ParametrosInvalidosException` com a mensagem "O segundo parâmetro deve ser maior que o primeiro", e essa mensagem será impressa no console.

## Contribuição

Sinta-se à vontade para contribuir para este projeto. Você pode abrir problemas (issues) ou enviar solicitações de pull request com melhorias.

## Licença

Este projeto está sob a [Licença MIT](LICENSE).
```

Lembre-se de personalizar o conteúdo conforme necessário e garantir que os URLs e as informações de contato estejam corretos. Este `README.md` fornece informações sobre como usar o projeto, exemplos e informações de contribuição e licença.
