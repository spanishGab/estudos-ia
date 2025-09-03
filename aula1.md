# Tópicos

## Context window e tokens

Context window: o número máximo de tokens que o modelo pode processar em uma única request. Isto inclui:

* Input tokens: os tokens no seu prompt
* Output tokens: os tokens que serão gerados pelo modelo
* Máximo de output tokens: o número máximo de tokens que o modelo pode gerar em uma única request

> Tipicamente, um token é aproximadamente equivaliente a 4 caracteres de um texto em inglês ou 3/4 de uma palavra, por exemplo 100 tokens ~= 75 palavras. A mesma palavra pode gerar tokens diferentes dependendo do contexto em que ela está escrita.Normalmente, outros idiomas produzem um maior número de tokens por palavra, o que pode afetar custo e limites do modelo.

## Reasoning

É o processo de, baseado em informações disponíveis, gerar predições, inferências e tirar conclusões. O Reasoning permite que o modelo reflita sobre o que ele tem de informações até aquele momento, e quebre sua análise em partes menores.

## Componentes do Reasoning

* Base de conhecimento: contém grafos de conhecimento, ontologias, redes semânticas. Ela mapeia entidades do mundo real, como conceitos, informações de domínio, eventos, fatos, objetos, relacionamentos, regras e situações. E deve ser modelada de uma forma que a IA consiga entender e utilizar.
* "Motor" de inferência: o modelo de IA que utiliza a base de conhecimento para gerar predições, inferências e tirar conclusões.

> [Comparação de modelos de IA](https://docs.github.com/en/copilot/reference/ai-models/model-comparison)

Thinking
Chain of thought
Tree of thought
Mixture of experts

api ninjas

Um júnior tem que conseguir ler seu prompt e executar a task

https://promptmetheus.com/resources/llm-knowledge-base
