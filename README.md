<div align="center">
  <img src="https://hermes.dio.me/courses/cover/ffd40f3e-17c9-4ccd-9140-8f44b6add39f_landingpage.png" alt="Descrição da imagem">
</div>

# trilha-java-basico

## Resolução de Desafios propostos pela plataforma da DIO

## [POO - Desafio](desafios/poo/README.md) 🔗

## Modelagem e diagramação da representação em UML e Código no que se refere ao componente iPhone.

Com base no vídeo de lançamento do iPhone conforme link abaixo, elabore em uma ferramenta de UML de sua preferência a diagramação das classes e interfaces com a proposta de representar os papéis do iPhone de: Reprodutor Musicial, Aparelho Telefônico e Navegador na Internet. Em seguida crie as classes e interfaces no formato de arquivos .java

Lançamento iPhone 2007


</br>
Comportamentos esperados: </br>
Repodutor Musicial: tocar, pausar, selecionarMusica </br>
Aparelho Telefônico: ligar, atender, iniciarCorrerioVoz </br>
Navegador na Internet: exibirPagina, adicionarNovaAba, atualizarPagina


## [Controle de Fluxo - Desafio](desafios/controle-fluxo) 🔗
Vamos exercitar todo o conteúdo apresentado no módulo de Controle de Fluxo codificando o seguinte cenário.

O sistema deverá receber dois parâmetros via terminal que representarão dois números inteiros, com estes dois números você deverá obter a quantidade de interações (for) e realizar a impressão no console (System.out.print) dos números incrementados, exemplo:

* Se você passar os números 12 e 30, logo teremos uma interação (for) com 18 ocorrências para imprimir os números, exemplo: `"Imprimindo o número 1"`, `"Imprimindo o número 2"` e assim por diante.
* Se o primeiro parâmetro for MAIOR que o segundo parâmetro, você deverá lançar a exceção customizada chamada de `ParametrosInvalidosException` com a segunda mensagem: "O segundo parâmetro deve ser maior que o primeiro"   


1. Crie o projeto `DesafioControleFluxo`
2. Dentro do projeto, crie a classe `Contador.java` para realizar toda a codificação do nosso programa.
3. Dentro do projeto, crie a classe `ParametrosInvalidosException` que representará a exceção de negócio no sistema. 

## [Sintaxe - Desafio](desafios/sintaxe/README.md) 🔗
Vamos exercitar todo o conteúdo apresentado no módulo de Sintaxe codificando o seguinte cenário.

1. Crie o projeto `ContaBanco` que receberá dados via terminal contendo as características de conta em banco conforme atributos abaixo:
2. Dentro do projeto, crie a classe `ContaTerminal.java` para realizar toda a codificação do nosso programa.

###### Revise sobre regras de declaração de variáveis

| Atributo  | Tipo     | Exemplo   
| --------- | ---------| ------- 
| Numero    | Inteiro  | 1021 
| Agencia   | Texto    | 067-8
| Nome Cliente | Texto    | MARIO ANDRADE
| Saldo | Decimal |237.48


###### Revise sobre terminal, main args e a classe Scanner
2. Permita que os dados sejam inseridos via terminal sendo que o usuário receberá a mensagem de qual informação será solicitada, exemplo:

* Programa: "Por favor, digite o número da Agência !"
* Usuário: 1021 *(depois ENTER para o próximo campo)* 

###### Revise sobre concatenação e classe String com método concat

3. Depois de todas as informações terem sido inseridas, o sistema deverá exibir a seguinte mensagem:

*"Olá [Nome Cliente], obrigado por criar uma conta em nosso banco, sua agência é [Agencia], conta [Numero] e seu saldo [Saldo] já está disponível para saque".*

Os campos em [ ] devem ser alterados pelas informações que forem inseridas pelos usuários.

# LINKS DOS DESAFIOS:  👇 
**Acesse aqui embaixo os desafios que foram concluidos:**
------

[![POO](https://img.shields.io/badge/POO%20-black?style=for-the-badge&logo=web)](desafios/poo/README.md)
[![Controle de Fluxo](https://img.shields.io/badge/Controle%20de%20Fluxo%20-black?style=for-the-badge&logo=pdf)](desafios/controle-fluxo/README.md)
[![Sintaxe](https://img.shields.io/badge/Sintaxe%20-black?style=for-the-badge&logo=web)](desafios/sintaxe/README.md)

