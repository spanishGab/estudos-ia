# Context memory management

Problema: não é viável (e as vezes nem possível) fazer a IA analisar toda a sua codebase. Por isso, referencie, tente dizer onde está a informação dentro do código.

Sempre limpe (ou compacte) a context window.

## Rules

As Rules entram na Long-Term Memory do modelo.
Existem algumas instruções que sempre serão necessárias. Exemplos:

* Responda sempre em português.
* Seja claro e conciso.
* Padrão de nomenclatura de usuário.

Podem ser definidas a nível de usuário ou de projeto.

Faça suas própris rules, não copie e cole.

Evite regras desnecessárias. Menos é mais.

Cuidado com a quantidade de exemplos e detalhes que vai dar ao escrever as rules para não encher a context window.

