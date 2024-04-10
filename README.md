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
    - [ ] Definição
    - [ ] Declarando uma função
    - [ ] Como chamar uma função
    - [ ] Parâmetros e argumentos
    - [ ] Atividade cálculo do IMC - Índice de Massa Corporal

### Funções - Definição
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

### Funções - Declarando uma função
Uma declaração de função mínima consiste no **tipo de retorno**, **nome da função** e **lista de parâmetros** (que pode estar vazia).

O seguinte exemplo é uma declaração de função:
```c++
int soma(int a, int b);
```

### Funções - Como chamar uma função
### Funções - Parâmetros e argumentos
### Funções - Atividade cálculo do IMC - Índice de Massa Corporal