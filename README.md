# Desvendando Sentimentos em Reviews

Este projeto implementa um sistema simplificado de análise de sentimentos para reviews de filmes e séries. Utilizando listas predefinidas de palavras positivas e negativas, o script analisa o texto dos reviews e classifica o sentimento geral como positivo, negativo ou neutro. O objetivo é demonstrar o conceito fundamental de como a Inteligência Artificial pode ser aplicada para entender a opinião expressa em linguagem natural, mesmo com uma abordagem básica.

## Funcionalidade

O script Python realiza as seguintes etapas:

* Define um Vocabulário de Sentimentos: Mantém duas listas estáticas de palavras: uma para sentimentos positivos e outra para sentimentos negativos.
* Analisa o Texto do Review: Para cada review fornecida em uma lista, o script converte o texto para minúsculas e o divide em palavras individuais.
* Calcula uma Pontuação de Sentimento: Itera pelas palavras do review e atribui uma pontuação: +1 para cada palavra encontrada na lista de palavras positivas e -1 para cada palavra encontrada na lista de palavras negativas.
* Classifica o Sentimento: Com base na pontuação total do review, o sentimento é classificado como:
    * **Positivo:** Pontuação maior que zero.
    * **Negativo:** Pontuação menor que zero.
    * **Neutro:** Pontuação igual a zero.
* Gera um Resumo: Após analisar todos os reviews na lista de exemplo, o script calcula e exibe a porcentagem de reviews classificados como positivos, negativos e neutros.

## Como Usar

1.  Clone o Repositório: Se você estiver visualizando este projeto no GitHub, clone-o para o seu ambiente local.
2.  Execute o Script no Google Colab (ou Python): O código foi desenvolvido em Python e pode ser facilmente executado no Google Colaboratory ou em um ambiente Python local.
3.  Visualize a Análise: Ao executar o script, ele primeiro analisará uma lista predefinida de reviews de filmes e séries, exibindo o sentimento classificado para cada um.
4.  Observe o Resumo: Ao final da análise individual, um resumo estatístico mostrará a porcentagem de reviews classificados como positivos, negativos e neutros.
5.  Explore e Modifique: Sinta-se à vontade para modificar a lista de `reviews_melhorados` no código para analisar outros textos. Você também pode expandir as listas `palavras_positivas` e `palavras_negativas` para melhorar a capacidade de detecção de sentimentos.

## Observações

Abordagem simplificada baseada em correspondência de palavras. Não considera contexto ou nuances da linguagem. Propósito demonstrativo do conceito de análise de sentimentos.

## Próximos Passos (Melhorias Futuras)

* Expandir o Vocabulário: Aumentar a abrangência das listas de palavras positivas e negativas para cobrir mais termos e nuances.
* Implementação de Negação: Adicionar lógica para identificar e tratar negações (e.g., "não é bom").
* Consideração de Intensidade: Atribuir pesos diferentes às palavras para refletir a intensidade do sentimento (e.g., "excelente" vs. "bom").
* Integração com Bibliotecas de PLN: Explorar o uso de bibliotecas mais avançadas como NLTK (se os problemas de configuração forem resolvidos) ou spaCy para uma análise de sentimentos mais sofisticada.
