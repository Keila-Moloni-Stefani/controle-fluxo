# Controle de Fluxo - Desafio DIO
Projeto desenvolvido como parte do desafio da Formação Java Developer na plataforma DIO (Digital Innovation One).

## Descrição do Projeto
Este projeto tem o objetivo de criar um sistema simples que valida parâmetros de entrada e realiza contagem numérica, explorando conceitos de:

- ✅ Controle de fluxo (if, for, try-catch)
- ✅ Tratamento de exceções customizadas
- ✅ Entrada de dados via terminal
- ✅ Boas práticas de programação em Java

## Objetivo

Criar um programa que:
1. Recebe dois números inteiros via terminal
2. Realiza a contagem incremental entre esses números
3. Lança uma exceção customizada quando o primeiro parâmetro for maior ou igual ao segundo

## Como Funciona

### Exemplo de Execução Válida:
```
Digite o primeiro parâmetro
12
Digite o segundo parâmetro
30
Imprimindo o número 1
Imprimindo o número 2
Imprimindo o número 3
...
Imprimindo o número 18
```

### Exemplo com Exceção:
```
Digite o primeiro parâmetro
30
Digite o segundo parâmetro
12
O segundo parâmetro deve ser maior que o primeiro
```

## Tecnologias Utilizadas
- Java JDK 8+
- Visual Studio Code (ou IDE de sua preferência)


## Estrutura do Projeto

```
DesafioControleFluxo/
│
├── Contador.java                      # Classe principal com lógica de contagem
└── ParametrosInvalidosException.java  # Exceção customizada
```

## Como Executar
Pré-requisitos
- JDK (Java Development Kit) instalado
- Terminal/Prompt de comando

### 1. Clone o repositório
```bash
git clone https://github.com/Keila-Moloni-Stefani/controle-fluxo.git
cd desafio-controle-fluxo
```

### 2. Compile os arquivos Java
```bash
javac Contador.java ParametrosInvalidosException.java
```

### 3. Execute o programa
```bash
java Contador
```

### 4. Insira os parâmetros quando solicitado
- Digite o primeiro número e pressione Enter
- Digite o segundo número e pressione Enter
- Observe o resultado da contagem ou a mensagem de erro

## Detalhes da Implementação

### Classe Contador
- Método `main`: Responsável pela entrada de dados e tratamento da exceção
- Método `contar`: Valida os parâmetros e realiza a impressão dos números

### Classe ParametrosInvalidosException
- Exceção customizada que estende `Exception`
- Lançada quando o primeiro parâmetro é maior ou igual ao segundo

### Lógica de Validação
```java
if (parametroUm >= parametroDois) {
    throw new ParametrosInvalidosException();
}
```

### Lógica de Contagem
```java
int contagem = parametroDois - parametroUm;
for (int i = 1; i <= contagem; i++) {
    System.out.println("Imprimindo o número " + i);
}
```

## Conceitos Aplicados

- **Controle de Fluxo**: Estruturas condicionais e de repetição
- **Exceções**: Criação e tratamento de exceções customizadas
- **Entrada de Dados**: Utilização da classe Scanner
- **Boas Práticas**: Validação de dados e tratamento de erros

## Licença
Este projeto foi desenvolvido para fins educacionais como parte do desafio da DIO.

## Desenvolvedor
Desenvolvido por Keila Moloni Stefani
⭐ Se este projeto foi útil para você, considere dar uma estrela!
