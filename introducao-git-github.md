# 👋 The Basics of GitHub - Relatório da Atividade

## ✅ O que aprendi

Durante o curso *The Basics of GitHub*, aprendi os seguintes conceitos:

- O que é o **Git**: um sistema de controle de versão distribuído para acompanhar mudanças no código.
- O que é o **GitHub**: uma plataforma para hospedar projetos Git, colaborar com outras pessoas e gerenciar repositórios.
- O fluxo de trabalho do GitHub (**GitHub Flow**) com uso de **branches**, **commits**, **pushes**, **pull requests** e **merges**.
- A importância dos **repositórios**, **clonagem local**, **commits com mensagens claras**, e **push para o repositório remoto**.
- Conceitos como:
  - `Forks` (quando queremos colaborar em projetos de outras pessoas),
  - `Issues` (para acompanhar bugs e tarefas),
  - `README` (para explicar o projeto),
  - `Project boards` (para organizar tarefas),
  - `Perfil do usuário` (que mostra histórico de contribuições e pode conter um README próprio),
  - `Markdown` (para estilizar textos no GitHub).

Também explorei a aba **GitHub Explore**, onde é possível encontrar projetos e pessoas para seguir.

## 🤔 O que ainda fiquei em dúvida

- Diferença prática entre `merge` e `rebase`, e quando usar cada um.
- Como resolver conflitos complexos de merge.
- Fluxos de trabalho recomendados para times grandes.

## 🎯 Conclusão

O curso forneceu uma base sólida para começar a usar Git e GitHub. Me sinto mais confiante para criar repositórios, usar branches e colaborar por meio de pull requests. A prática com Markdown também foi útil para documentar o que aprendi. 

### 🧩 Conceitos importantes 




- **Forks** → permitem copiar um repositório de outra pessoa para o seu perfil e experimentar mudanças sem afetar o projeto original. Muito usado em projetos *open source*.  
- **Issues** → funcionam como listas de tarefas ou relatórios de problemas/bugs. Também servem para propor novas funcionalidades.  
- **README** → arquivo inicial de um repositório, explica o objetivo do projeto, como utilizá-lo e instruções de instalação/execução.  
- **Project boards** → quadros visuais para organizar tarefas, bugs e melhorias. Úteis em projetos maiores, lembram ferramentas como o Trello.  
- **Perfil do usuário** → página pessoal que mostra os repositórios, contribuições e pode incluir um README de apresentação.  
- **Markdown** → linguagem simples de formatação usada no GitHub para criar textos com títulos, listas, **negrito**, *itálico*, links, imagens e muito mais.  
### 🧠 Conceitos importantes que aprendi:

- **Forks**: usados para copiar repositórios de outras pessoas e fazer experimentos sem afetar o projeto original. Muito comum em projetos open source.
- **Issues**: servem para relatar bugs, sugerir melhorias ou registrar tarefas. Podem ser atribuídas a membros do projeto.
- **README**: arquivo de apresentação do projeto. Explica sua utilidade, como rodar, objetivos e instruções de uso.
- **Project boards**: quadros semelhantes ao  que organizam tarefas com base em *issues* e *pull requests*, muito úteis em projetos maiores.
- **Perfil do usuário**: mostra seus repositórios, contribuições, atividades e pode conter um README pessoal com descrição sobre você.
- **Markdown**: linguagem de marcação simples para formatação de texto

---

**Aluno:** Gabriel Ferraz Duque  
**Data:** 22/09/2025  
**Curso:** Ciência da Computação – UNICAP   


 #include <stdio.h>  
int main() {
    printf("Olá, Git e GitHub em C!\n");
    return 0;
// main.c
#include <stdio.h>

int main() {
    printf("Olá, Git e GitHub em C!\n");
    return 0;
}
// Fim do arquivo: main.c
// Para compilar e executar:
// gcc main.c -o main
// ./main
// Saída esperada: Olá, Git e GitHub em C!
// Fim do código
// Este código em C imprime uma mensagem simples no console. 
// Ele pode ser compilado e executado em qualquer ambiente que suporte C. 
// Certifique-se de ter um compilador C instalado, como GCC. 
// Salve o código em um arquivo chamado main.c e siga as instruções de compilação          
// e execução acima.
// Este código é um exemplo básico para demonstrar o uso de Git e GitHub.       

// Você pode fazer commit deste arquivo em um repositório Git e enviá-lo para o GitHub.
// Fim do código
// Este código em C imprime uma mensagem simples no console.

#include <stdio.h> 
int main() {
    printf("Olá, Git e GitHub!\n");
    return 0;
}
// Fim do arquivo: hello.c
// Para compilar e executar:
// gcc hello.c -o hello
// ./hello      

// Ele pode ser compilado e executado em qualquer ambiente que suporte C. 
// Certifique-se de ter um compilador C instalado, como GCC.

#include <stdio.h>

int main() {
    printf("Olá, Git e GitHub!\n");
    return 0;
}
// Fim do arquivo: hello.c 
// Para compilar e executar:
// gcc hello.c -o hello
// ./hello  
// Saída esperada: Olá, Git e GitHub!   
// Fim do código
// Este código em C imprime uma mensagem simples no console. 
// Ele pode ser compilado e executado em qualquer ambiente que suporte C. 
// Certifique-se de ter um compilador C instalado, como GCC. 
// Salve o código em um arquivo chamado hello.c e siga as instruções de compilação e execução acima. 
// Este código é um exemplo básico para demonstrar o uso de Git e GitHub. 
// Você pode fazer commit deste arquivo em um repositório Git e enviá-lo para o GitHub.
// Fim do código
// Este código em C imprime uma mensagem simples no console. 
// Ele pode ser compilado e executado em qualquer ambiente que suporte C. 
// Certifique-se de ter um compilador C instalado, como GCC. 
// Salve o código em um arquivo chamado hello.c e siga as instruções de compilação e execução acima. 
// Este código é um exemplo básico para demonstrar o uso de Git e       GitHub. 
// Você pode fazer commit deste arquivo em um repositório Git e enviá-lo para o. GitHub. 







#include <stdio.h> 
#include <stdlib.h> 
#include <math.h>  
// media(float* vetor, int tam)
// variancia(float* vetor, int tam, float m)  


 float media(float* vetor, int tam) {

    float soma = 0.0;
    for (int i = 0; i < tam; i++) {
        soma += vetor[i];
    }
    return soma / tam;
}

float variancia(float* vetor, int tam, float m) {
    float soma = 0.0;
    for (int i = 0; i < tam; i++) {
        soma += (vetor[i] - m) * (vetor[i] - m);
    }
    return soma / tam;
}

int main() {
    int n;
    printf("Digite o tamanho do vetor: ");
    scanf("%d", &n);

    float* vetor = (float*)malloc(n * sizeof(float));
    if (vetor == NULL) {
        fprintf(stderr, "Erro ao alocar memória.\n");
        return 1;
    }
 float* vetor = (float*)malloc(n * sizeof(float));
    for (int i = 0; i < n; i++) {
        printf("Digite o elemento %d: ", i);
        scanf("%f", &vetor[i]);
    }

    float m = media(vetor, n);
    float v = variancia(vetor, n, m);

    printf("Media: %.2f\n", m);
    printf("Variancia: %.2f\n", v);

    free(vetor);
    return 0;
}


