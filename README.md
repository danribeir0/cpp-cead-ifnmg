# C++ - Funções
Prática - trabalhando com funções e recursividade  
Referência -> [Learn > Microsoft C++, C e Assembler > Documentação do C++ ](https://learn.microsoft.com/pt-br/cpp/cpp/?view=msvc-170)
Referência -> [Learn > Microsoft C++, C e Assembler > Funções (C++) ](https://learn.microsoft.com/pt-br/cpp/cpp/functions-cpp?view=msvc-170)

## Objetivos
- Revisão rápida:
    - [X] História da linguagem
	- [X] Ambientes de Desenvolvimento
	- [X] Inputs e Outputs
	- [X] Tipos de dados - fortemente tipadas / fracamente tipadas
	- [X] Variáveis e Constantes
	- [X] Operadores aritméticos
	- [X] Operadores relacionais
	- [X] Operadores lógicos
	- [X] Ordem de precedência
	- [X] Estruturas condicionais
	- [X] Laços de repetição
    - [ ] Funções
	- [ ] Recursividade - Funções Recursivas
	- [ ] Vetores
	- [ ] Estrutura de dados

- Funções
    - [ ] O que é uma função?
    - [ ] Declarando e definindo uma função (criando uma função)
    - [ ] Como chamar uma função (usando a função)
    - [ ] Parâmetros e argumentos
    - [ ] Atividade cálculo do IMC - Índice de Massa Corporal

### 1. O que é uma função?
Uma função é um bloco de código que executa alguma operação.
```c++
void minhaFuncao(){
    std::cout << "Você chamou a função 'minhaFuncao'"
}
```

As funções são úteis para encapsular operações comuns em um só bloco reutilizável, idealmente com um nome que descreve de modo claro o que a função faz.

Opcionalmente, uma função pode definir parâmetros de entrada que permitem que os chamadores passem argumentos para a função.

Uma função também pode retornar um valor como saída.

A função a seguir aceita dois inteiros de um chamador e retorna sua soma; `num1` e `num2` são parâmetros do tipo int.
```c++
int soma(int num1, int num2){
    return num1 + num2;
}
```

### 2. Declarando e definindo uma função (criando uma função)
Uma declaração de função mínima consiste no **tipo de retorno**, **nome da função** e **lista de parâmetros** (que pode estar vazia).

O seguinte exemplo é uma declaração de função:
```c++
int soma(int a, int b);
```

Uma definição de função consiste em uma declaração mais o corpo da função, que é todo o código entre as chaves:
```c++
int soma(int num1, int num2){
    return num1 + num2;
}
```

As partes necessárias para a declaração de uma função são:

1. O tipo de retorno, que especifica o tipo do valor que a função retorna ou __void__ se nenhum valor é retornado. No C++ 11, **auto** é um tipo de retorno válido que instrui o compilador a inferir o tipo da instrução return.

2. O nome da função, que deve começar com uma letra ou sublinhado e não pode conter espaços.

3. A lista de parâmetros, um conjunto delimitado por parenteses, separados por vírgula, com nenhum ou mais parâmetros.

```c++
auto soma(int num1, int num2){
    return num1 + num2;
}
```

### 3. Como chamar uma função (usando a função)
Uma função pode ser invocada ou chamada de qualquer lugar do programa. Os valores que são passados para a função são os argumentos, cujos tipos devem ser compatíveis com os tipos de parâmetro na definição de função.

```c++
int main() {
    minhaFuncao();
    std::cout << soma(12, 27);
}
```

### 4. Parâmetros e argumentos
Uma função pode ter uma lista de parâmetros separada por vírgulas, cada um dos quais tem um tipo e um nome pelo qual pode ser acessado dentro do corpo da função.  
Uma função pode ter parâmetros de tipos diferentes. O chamador/invocador passa argumentos, que são valores concretos cujos tipos são compatíveis com a lista de parâmetros.

### 5. Atividade cálculo do IMC - Índice de Massa Corporal
Mãos na massa.

Criar um programa em C++ que receba o peso e a altura de uma pessoa e calcule o Índice de Massa Corporal.  
O programa deve ter **uma função que calcule e retorne o IMC**  