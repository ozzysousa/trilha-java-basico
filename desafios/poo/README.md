## POO - Desafio

Modelagem e diagramação da representação em UML e Código no que se refere ao componente iPhone.

Com base no vídeo de lançamento do iPhone conforme link abaixo, elabore em uma ferramenta de UML de sua preferência a diagramação das classes e interfaces com a proposta de representar os papéis do iPhone de: Reprodutor Musicial,  Aparelho Telefônico e Navegador na Internet. Em seguida crie as classes e interfaces no formato de arquivos .java

[Lançamento iPhone 2007](https://www.youtube.com/watch?v=9ou608QQRq8)

###### Comportamentos esperados:
* Repodutor Musicial: tocar, pausar, selecionarMusica
* Aparelho Telefônico: ligar, atender, iniciarCorrerioVoz
* Navegador na Internet: exibirPagina, adicionarNovaAba, atualizarPagina

# iPhone Component - UML and Java Code Example

Welcome to the iPhone Component example README. This README provides a detailed explanation of the UML class diagram and the Java code implementation for an iPhone component.

## UML Class Diagram

Here is a simplified UML representation of the classes and interfaces for the iPhone component:
```@startuml

interface ReprodutorMusical {
  + tocar()
  + pausar()
  + selecionarMusica()
}

interface AparelhoTelefonico {
  + ligar(numero: String)
  + atender()
  + iniciarCorreioVoz()
}

interface NavegadorInternet {
  + exibirPagina(url: String)
  + adicionarNovaAba()
  + atualizarPagina()
}

class IPhone {
  - estado: String
}

IPhone --> ReprodutorMusical
IPhone --> AparelhoTelefonico
IPhone --> NavegadorInternet

@enduml 
```
![UML Class Diagram](uml.png)

## Java Code

Below is the Java code that implements the classes and interfaces for the iPhone component:

```
interface ReprodutorMusical {
    void tocar();
    void pausar();
    void selecionarMusica();
}

interface AparelhoTelefonico {
    void ligar(String numero);
    void atender();
    void iniciarCorreioVoz();
}

interface NavegadorInternet {
    void exibirPagina(String url);
    void adicionarNovaAba();
    void atualizarPagina();
}

class IPhone implements ReprodutorMusical, AparelhoTelefonico, NavegadorInternet {
    private String estado;

    @Override
    public void tocar() {
        // Implementação para tocar música
    }

    @Override
    public void pausar() {
        // Implementação para pausar música
    }

    @Override
    public void selecionarMusica() {
        // Implementação para selecionar uma música
    }

    @Override
    public void ligar(String numero) {
        // Implementação para ligar para um número
    }

    @Override
    public void atender() {
        // Implementação para atender chamadas
    }

    @Override
    public void iniciarCorreioVoz() {
        // Implementação para iniciar correio de voz
    }

    @Override
    public void exibirPagina(String url) {
        // Implementação para exibir uma página da internet
    }

    @Override
    public void adicionarNovaAba() {
        // Implementação para adicionar uma nova aba no navegador
    }

    @Override
    public void atualizarPagina() {
        // Implementação para atualizar a página no navegador
    }
}
```
## Installation Instructions

Follow these steps to install and run the Java code:

1. **Ensure you have the Java Development Kit (JDK) installed on your system.** You can download it from [Oracle JDK](https://www.oracle.com/java/technologies/javase-downloads.html) or [OpenJDK](https://adoptopenjdk.net/).

2. **Copy the provided Java code into a `.java` file.** For example, you can create a file named `IPhone.java` and paste the `IPhone` code into it.

3. **Open a terminal or command prompt and navigate to the directory where you saved the Java file.**

4. **Compile the Java code by running the following command:**

   ```bash
   javac IPhone.java

   After successful compilation, you can run the program:

  ```bash
Copy code
java IPhone
That's it! The Java code should now be running.
   ```

