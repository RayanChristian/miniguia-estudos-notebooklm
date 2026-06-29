# Miniguia de Estudos: Estudo da Linguagem C

## 🎯 Contexto e Objetivos
O assunto escolhido se refere ao conhecimento amplo da Linguagem C. Esta linguagem é amplamente utilizada como base estrutural no ensino superior e técnico para fundamentar os conceitos de programação, facilitando a compreensão posterior de linguagens consideradas mais avançadas.

## 📚 Curadoria de Fontes
* **Fonte 1:** [Curso de Linguagem C - USP (IME)](https://www.ime.usp.br/~slago/slago-C.pdf)
* **Fonte 2:** [Programação de Computadores em C - Kufunda](https://www.kufunda.net/publicdocs/Programacao%20de%20Computadores-C.pdf)
* **Fonte 3:** [Introdução à Linguagem C - USP (MAC1101)](https://www.ime.usp.br/~mms/mac1101s2013/aula04%20introducao%20ao%20C.pdf)

## 🛠️ Engenharia de Prompts e "Cicatrizes" (Troubleshooting)
Durante o desenvolvimento do caderno temático de Linguagem C, o processo de refinamento das interações com a IA passou pelas seguintes etapas:

1. **Abordagem Inicial (Ampla demais):**
   * **Prompt:** *"Quais as 3 melhores fontes disponíveis na internet que melhor abordam a linguagem c?"*
   * **Problema encontrado:** A IA recomendou portais e sites inteiros, o que dificultaria a curadoria exata de arquivos para o NotebookLM.
   * **Solução:** Refinei a abordagem exigindo arquivos específicos e diretos.
   * **Prompt de correção:** *"Então me diga 3 documentos disponíveis gratuitamente para que eu possa aplicá-los ao notebook LM."*

2. **Problema de Didática (Falta de Prática):**
   * **Prompt:** *"Me ensine a coisa mais básica da linguagem c."*
   * **Problema encontrado:** A IA retornou um grande volume de texto teórico, mas carecia de exemplos práticos de código e aplicações reais.
   * **Solução (Troubleshooting):** Em vez de apenas pedir "coloque exemplos", configurei uma diretriz estrita de comportamento para a IA para que todas as respostas adotassem uma estrutura de aprendizado ativo.
   * **Instrução/Padrão adotado:** `"Seguir padrão de resposta: Explicação -> Exemplos -> Dúvidas comuns com resoluções"`.

**Resultado:** Após essa intervenção de engenharia de prompt, as respostas tornaram-se significativamente mais focadas, facilitando a absorção dos conceitos básicos da Linguagem C e gerando um material muito mais rico para o Miniguia final.

## 📖 Miniguia de Estudo (Entrega Final)

### Resumos Estruturados
A linguagem C é uma linguagem de programação de alto nível e de paradigma imperativo, o que significa que o código consiste em uma sequência de comandos que descrevem como o computador deve modificar seu estado na memória para realizar uma tarefa.

Os pilares fundamentais para iniciantes são:
* **A Estrutura do Programa:** Todo programa em C deve, obrigatoriamente, possuir uma função chamada `main`, que é o ponto onde a execução se inicia. O corpo das funções e os blocos de instruções são delimitados por chaves `{ }`.
* **Sintaxe Básica:** Cada instrução ou comando individual deve terminar com um ponto e vírgula `;` para indicar ao compilador o fim daquela operação. Comentários podem ser inseridos usando `/* texto */` para blocos ou `// texto` para linhas únicas.
* **Variáveis e Tipos de Dados:** Antes de usar qualquer dado, é necessário declará-lo. Os tipos mais comuns são:
  * `int`: para números inteiros (ex: 10, -5).
  * `float` e `double`: para números com casas decimals.
  * `char`: para armazenar um único caractere (como 'A' ou '7').
* **Entrada e Saída:** Para interagir com o usuário, utilizam-se funções da biblioteca `stdio.h`:
  * `printf()`: exibe informações formatadas na tela.
  * `scanf()`: lê valores digitados pelo usuário.
* **O Processo de Compilação:** O código-fonte escrito em C precisa passar por um programa chamado compilador, que o traduz para um arquivo executável que o processador entende.

#### Exemplo Prático
Abaixo, um exemplo de programa básico que lê um número inteiro e exibe o seu dobro:

```c
#include <stdio.h> // Diretiva para incluir funções de entrada e saída

int main() { // Função principal obrigatória
    int numero, resultado; // Declaração de variáveis inteiras

    printf("Digite um valor: "); // Exibe mensagem na tela
    scanf("%d", &numero); // Lê um inteiro digitado e guarda em 'numero'

    resultado = numero * 2; // Operação de atribuição e aritmética

    printf("O dobro de %d e: %d\n", numero, resultado); // Exibe resultados formatados

    return 0; // Indica que o programa terminou com sucesso
}
```
### 📚 Glossário de Conceitos
* **Alocação Dinâmica:** Processo que permite a um programa requisitar memória adicional durante a sua execução através de funções como malloc().
* **Arranjo (Vetor ou Matriz):** Coleção de variáveis de um mesmo tipo que compartilham o mesmo nome e ocupam posições consecutivas na memória.
* **Bit:** A menor unidade de informação em um computador, podendo assumir os valores 0 ou 1.
* **Bloco:** Uma sequência de comandos agrupados entre chaves { }.
* **Compilador:** Programa que traduz o código escrito em linguagem de alto nível (como C) para a linguagem de máquina que o processador entende.
* **Diretiva de Pré-processamento:** Comandos iniciados por # (como #include e #define) que são processados antes da compilação propriamente dita.
* **Endereço de Memória:** Um número inteiro que identifica uma posição específica na memória RAM onde um dado está armazenado.
* **Estrutura (struct):** Uma coleção de variáveis logicamente relacionadas, que podem ser de tipos diferentes, agrupadas sob um único nome.
* **Função main:** É a função principal de um programa em C, servindo como o ponto obrigatório de início da execução.
* **Ponteiro:** Uma variável especial que, em vez de armazenar um valor comum, armazena o endereço de memória de outra variável.
* **Recursividade:** Princípio de programação onde uma função chama a si mesma para resolver uma instância menor do mesmo problema.
* **String:** Em C, é um vetor de caracteres que termina obrigatoriamente com o caractere nulo \0.
* **Tipo de Dado:** Define o conjunto de valores que uma variável pode assumir e o espaço que ocupará na memória (ex: int, float, char).

### 🔄 Prompts Reutilizáveis
Para guiar futuras revisões ou expandir o conhecimento deste caderno temático, utilize a seguinte estrutura de prompt no Gemini ou no NotebookLM:

* **Prompt de Aprendizado Ativo:**
  > "Atue como um tutor acadêmico especialista em computação, utilizando as fontes fornecidas. Siga o padrão de resposta: Explicação -> Exemplos práticos em código C -> Dúvidas comuns com resoluções."
