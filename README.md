# LLM-From-Scratch

### Descrição
Este repositório reúne uma tradução comentada e adaptada do livro **[LLM From Scratch](https://github.com/rasbt/LLMs-from-scratch)**, de **[Sebastian Raschka](https://sebastianraschka.com)**. O material foi produzido em português e executado no Google Colab, com o objetivo de desenvolver meus estudos em Modelos Largos de Linguagem (LLMs) para compreender, do zero, como funcionam as LLMs, agora desejo o tornar acessível para estudantes e profissionais brasileiros.

Cada notebook corresponde a um capítulo do livro original, contendo:
- Traduções e explicações conceituais detalhadas;
- Códigos reescritos e comentados em português;
- Observações adicionais sobre fundamentos estatísticos e aspectos de IA generativa.

O projeto nasce do interesse de um estatístico em formação que está se aprofundando em **IA generativa** e **estatística teórica-aplicada**, que busca compreender a base matemática e computacional por trás das arquiteturas modernas de linguagem.

> 💡 O material tem fins exclusivamente educacionais, e os créditos autorais pelo conteúdo original pertencem ao Doutor Sebastian Raschka, autor do livro. Támbem agradeço ao laboratório **[LASSE](https://www.lasse.ufpa.br/pt)**, por proporcionar a oportunidade de desenvolvimento de minhas habilidades nessa área.

---

### Estrutura e Execução

Todos os notebooks foram desenvolvidos no **Google Colab** e podem ser abertos diretamente através dos links “Open in Colab” presentes abaixo, ou baixados diretamente nas pastas de cada capítulo deste repositório.

- **Capítulo 1 - Compreendendo Modelos Largos de Linguagem Introdução e Fundamentos** [***ainda será publicado***]:
    - Explicações de alto nível dos conceitos fundamentais por trás dos grandes modelos de linguagem (LLMs);
    - Insights sobre a arquitetura do transformador da qual os LLMs são derivados;
    - Um plano para construir um LLM do zero.

- **Capítulo 2 - Trabalhando com Dados de Texto**[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1sxiHGbu077Wj8O4-JzxfdAnh2-3nnenk?usp=sharing):
    - Preparando texto para treinamento em modelos de linguagem de grande porte;
    - Dividindo texto em tokens de palavras e subpalavras;
    - Codificação de pares de bytes como uma forma mais avançada de tokenizar texto;
    - Amostrando exemplos de treinamento com uma abordagem de janela deslizante;
    - Convertendo tokens em vetores que alimentam um modelo de linguagem de grande porte.
  
- **Capítulo 3 - Codificando Mecanismos de Atenção**[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1X50vdgIkOnY6Sgap6FoMuCEysFLbAFJk?usp=sharing):
    - Razões para usar mecanismos de atenção em redes neurais;
    - Uma estrutura básica de autoatenção, evoluindo para um mecanismo de autoatenção aprimorado;
    - Um módulo de atenção causal que permite que os LLMs gerem um token por vez;
    - Mascaramento de pesos de atenção selecionados aleatoriamente com dropout para reduzir o overfitting;
    - Empilhamento de múltiplos módulos de atenção causal em um módulo de atenção multicabeça.
    
- **Capítulo 4 - Implementando um Modelo GPT do zero para gerar texto**[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1s0-_-PpUFQZLPGOqrCw7aK6SZQ_E4BcZ?usp=sharing):
    - Codificação de um modelo de linguagem grande (LLM) semelhante ao GPT que pode ser treinado para gerar texto semelhante ao humano;
    - Normalização de ativações de camadas para estabilizar o treinamento de redes neurais;
    - Adição de conexões de atalho em redes neurais profundas;
    - Implementação de blocos transformadores para criar modelos GPT de vários tamanhos;
    - Cálculo do número de parâmetros e dos requisitos de armazenamento dos modelos GPT.
  
- **Capítulo 5 - Pré-Treinamento em Dados Não Rotulados**[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-hPj8EfBttqcRZnlg55_TWsB7FtL5tAY?usp=sharing):
    - Calcular as perdas do conjunto de treinamento e validação para avaliar a qualidade do texto gerado pelo LLM durante o treinamento;
    - Implementar uma função de treinamento e pré-treinar o LLM;
    - Salvar e carregar pesos do modelo para continuar treinando um LLM;
    - Carregar pesos pré-treinados do OpenAI.
  
- **Capítulo 6 - Fine-tuning para Classificação**[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/16DSLc6QWZsfvF7ZsXjLC-DKbeA1izl13?usp=sharing):
    - Introdução de diferentes abordagens de ajuste fino de LLM;
    - Preparação de um conjunto de dados para classificação de texto;
    - Modificação de um LLM pré-treinado para ajuste fino;
    - Ajuste fino de um LLM para identificar mensagens de spam;
    - Avaliação da precisão de um classificador de LLM ajustado;
    - Utilização de um LLM ajustado para classificar novos dados.
  
- **Capítulo 7 - Fine-tuning para seguir instruções**[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1nU0Rj4jkmw8fAPv4jOno_t90TKjXAOsL?usp=sharing):
    - O processo de ajuste fino de instruções de LLMs;
    - Preparar um conjunto de dados para ajuste fino de instruções supervisionado;
    - Organizar dados de instruções em lotes de treinamento;
    - Carregar um LLM pré-treinado e ajustá-lo para seguir instruções humanas;
    - Extrair respostas de instruções geradas por LLM para avaliação;
    - Avaliar um LLM com ajuste fino de instruções.

