# Criando um plano de desenvolvimento com IA

## Qual é o problema?

* Repetição de instruções
* Definir quais regras se aplicam em cada tipo de prompt
* Nem sempre é possível executar mais de um prompt em paralelo
* Pode acontecer de esquecermos de limpar o contexto e misturar tarefas diferentes
* Autorizar ou restringir determinadas ferramentas e MCPs
* Definir modelos específicos para diferentes tarefas

## Comandos ou Prompts

Os comandos são prompts pré definidos para não precisarmos repetir a escrita nos nossos prompts.

**Limitação dos comandos**: falta de isolamento de contexto e paralelismo.

### Exemplos de Comandos:

* Implement feature
* Troubleshoot error
* Review pull request

### Regra vs Comando

* Regra: vale para todas as atividades.
* Comando: é uma orientação para um tipo específico de atividade.

## Subagentes

* Personificação: atribui-se um papel para aquele subagente ao criá-lo
* Execução tem paralelo: vários subagente agindo ao mesmo tempo
* Isolamento de contexto: contextos não se misturam
* Definição de um modelo específico: cada subagente pode utilizar um LLM diferente
* Restrição de Tools e MCPs
* Um subagente pode invocar outros para ajudá-lo

### Como criar?

Um arquivo `.md` com as especificações e personalizações daquele agente.

## Recursos

> SuperClaude: para estudar exemplos de comandos.