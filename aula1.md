# Tópicos

## Context window e tokens

Context window: o número máximo de tokens que o modelo pode processar em uma única request. Isto inclui:

* Input tokens: os tokens no seu prompt
* Output tokens: os tokens que serão gerados pelo modelo
* Máximo de output tokens: o número máximo de tokens que o modelo pode gerar em uma única request

> Tipicamente, um token é aproximadamente equivaliente a 4 caracteres de um texto em inglês ou 3/4 de uma palavra, por exemplo 100 tokens ~= 75 palavras. A mesma palavra pode gerar tokens diferentes dependendo do contexto em que ela está escrita.Normalmente, outros idiomas produzem um maior número de tokens por palavra, o que pode afetar custo e limites do modelo.

## Reasoning

É o processo de, baseado em informações disponíveis, gerar predições, inferências e tirar conclusões. O Reasoning permite que o modelo reflita sobre o que ele tem de informações até aquele momento, e quebre sua análise em partes menores.

### Componentes do Reasoning

* Base de conhecimento: contém grafos de conhecimento, ontologias, redes semânticas. Ela mapeia entidades do mundo real, como conceitos, informações de domínio, eventos, fatos, objetos, relacionamentos, regras e situações. E deve ser modelada de uma forma que a IA consiga entender e utilizar.
* "Motor" de inferência: o modelo de IA que utiliza a base de conhecimento para gerar predições, inferências e tirar conclusões.

[Artigo IBM](https://www.ibm.com/think/topics/ai-reasoning)

> [Comparação de modelos de IA](https://docs.github.com/en/copilot/reference/ai-models/model-comparison)

### Token bias

Descreve o fato de que cada token no prompt pode influenciar a resposta final do modelo. POr isso é muito importante que o prompt seja escrito da forma mais assertiva possível, para que ele direcione o modeloo exatamente para a resposta esperada.

## AI frameworks

[AI Thinking](https://royalsocietypublishing.org/doi/10.1098/rsos.241482)

## Chain of thought

É a criação de uma linha de raciocínio que leva a respostas mais estruturadas. Ele se baseia na estratégia cognitiva de dividir problemas elaborados em pensamentos intermediários, que sequencialmente levam a uma resposta conclusiva.

Ele exige que a IA construa um argumento lógico completo, incluindo premissas e uma conclusão. Através do fornecimento de exemplos que simulam um raciocínio para resolução de um problema, a IA consegue entender a estrutura lógica e aplicá-la para outros cenários.

É uma abordagem mais direta, onde cada token anterior é utilizado para gerar o próximo token "da esquerda para a direita", seguindo um caminho lógico único.

[Artigo IBM](https://www.ibm.com/br-pt/think/topics/chain-of-thoughts)

## Tree of thought

É uma abordagem hierárquica onde o prompt indica um "nó central" de onde partem diversos outros nós, onde o modelo pode interagir com cada um deles, ir e voltar entre os caminhos iterativamente para poder chegar a uma conclusão.

[Artigo IBM](https://www.ibm.com/br-pt/think/topics/tree-of-thoughts)

## Mixture of experts

## Random

api ninjas

Um júnior tem que conseguir ler seu prompt e executar a task

[Glossário](https://promptmetheus.com/resources/llm-knowledge-base)
