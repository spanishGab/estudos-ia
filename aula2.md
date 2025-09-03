# Prompt Engineering

## Tipos de Prompting

### Zero shot

Somente uma instrução básica.

### Few shot

- Fornece exemplos para a IA entender o que fazer, e pode ter mais de uma interação.

### One shot

- Uma entrada e uma saída

## Gold Tips

- Como fazer um prompt que funciona?

### Dica 01: Comece simples

- Inicie um arquivo .md e tente não usar muito LLM inicialmente.
- Para tarefas grandes, divida em tarefas menores.
- Documente os padrões bem-sucedidos.

### Dica 02: Intruções claras

- Use comandos específicos: "Escrever", "Classificar", "Resuma".
- Use ordens no imperativo: "Você deve...", "Você precisa...", "Você vai fazer agora...".
- Adicione consequências: "Se não fizer X, sua tarefa sera rejeitada".

### Dica 03: Seja espeficico

- Forneça exemplos no prompt para formatos específicos.
- Considere limitações da janela de contexto (não seja redundante).
- Inclua detalhes relevantes para a tarefa (arquivos dependentes, estrutura de pastas, etc)
- Especifique os detalhes técnicos necessários (ferramentas, libs, padrões, etc).
- Use Markdown + XML para formatacao e variáveis.

### Dica 04

- Diga o que fazer... mas tambem diga o que não fazer.
- Repita limitações críticas, se necessário.

## Formatos de Prompt

### Markdown Puro

```md
# Task
# Instructions
# Requirements
# Context
# Input
# Output
```

### XML

```xml
<task>
<instructions>
<requirements>
<context>
<input>
<output>
</task>
```

### Markdown com XML

```md
<task>
<requirements>
# Instructions
# Context
# Output
```

## Roles em Chat Models

### System prompt

Define o comportamento geral e as instruções de alto nível do assistente.

### User prompt

Representa a mensagem do usuário (pergunta ou instrução).

### Assistant prompt

Representa a resposta gerada pelo modelo.

### Exemplo

```json
{
    "messages": [
        {
            "role": "system",
            "content": "Você é um assistente de codificação útil"
        },
        {
            "role": "user",
            "content": "Escreva uma fução para ordenar um array em javascript"
        }
    ]
}
```

## Refinamento de prompt

console.anthropic.com/dashboard

## Context Engineering

A Evolucao do Prompt Engineering

- Agentes de IA sao o futuro do desenvolvimento de software.
- Principais falhas de agentes: falhas de contexto.
- Não são mais falhas de modelo, mas de informação.
- Qualidade do contexto determina o sucesso do agente.
- Sistemas mais complexos exigem abordagem sistematica.

## Componentes do Contexto

1. Instructions / System Prompt
    - Define o comportamento geral do agente.
    - Estabelece o papel, tom e limitações.
    - Inclui exemplos e regras de condutas.
    - Fornece contexto temporal (data/hora).
    - Define objetivos de alto nivel.
2. User prompt
    - A pergunta ou instrucao especifica do usuário.
3. State/History (short-term memory)
    - A conversa atual entre o usuário e o modelo.
    - Respostas anteriores do modelo.
    - Decisões e raciocónios prévios.
    - Informações temporárias relevantes.
    - Gerenciada dentro da janela de contexto.
4. Long-Term Memory
    - Base de conhecimento persistente e preferência do usuário.
    - Decisoes importantes.
5. Available Tools
    - Ferramentas disponíveis para o agente.

## Retrieved Information (RAG)

- Transformar um arquivo em vetor de tokens para poder ser inserido no contexto.

## Gerenciamento de Contexto ruim vs Contexto Bom

### Contexto ruim

- Sem informações adicionais, o modelo não tem como dar uma resposta precisa e útil.

### Contexto bom

- Com acesso a dados e ferramentas, a resposta se torna personalizada e acionavel.

## Obs

1. Quando citamos um arquivo ou referenciamos tem um resultado diferente
    - Referenciar: a IA lê antes o arquivo e usa como referencia no contexto. (@, #). Injeta arquivo no contexto.
    - Citar: Ela vai ler o arquivo, gasta mais tokens de entrada e saida.
2. Peça para a IA gerar um plano antes de pedir para ela executar.
