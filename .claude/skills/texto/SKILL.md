---
name: texto
description: Escrever ou revisar QUALQUER texto que uma pessoa vai ler — tela do app, botão, rótulo, mensagem de erro, estado vazio, onboarding, folha de explicação e ajuda, i18n (pt.json/en.json), Novidades (changelog.json), CHANGELOG.md, tópico do Assistente, FAQ, página e e-mail do site, resposta de chamado, notas das lojas, post e legenda de rede social, push e notificação. Use SEMPRE antes de escrever ou alterar um desses textos, sem esperar que peçam "deixe mais humanizado" — a régua é a linguagem do colecionador, não a de sistema. Todo texto novo ou alterado passa ainda por um AGENTE ESPECIALISTA EM ESCRITA (subagente revisor) antes de ser salvo. Também para revisar texto que já existe e soa robótico. Vale para o app, o site, a API, os workers, os pipelines e todos os projetos do TCG Vision e da F-Labs.
---

# Texto na fala do usuário (a skill mora no `~/.claude`)

Esta régua vale para **todos** os projetos do TCG Vision e para o site da F-Labs, por isso ela
mora no global em vez de num repo. **Antes de qualquer outro passo, leia
`C:\Users\gufior\.claude\skills\texto\SKILL.md` e siga o que está lá.**

**Todo texto que uma pessoa vai ler passa por um agente especialista em escrita antes de ser
salvo** (Gustavo, 07/11/2026). É um subagente revisor que lê a skill sem o contexto da
implementação e devolve as propostas em PT e EN. Vale mesmo onde um `CLAUDE.md` proíbe
subagentes: é a exceção permanente. O que mandar para ele e o que fazer com a resposta: seção
"Agente especialista em escrita" da skill.

## O que o Gustavo mais cobrou (o revisor confere todos, na frase e na tela)

1. **O ganho, não o mecanismo**, em frases curtas, sem termo de bastidor.
2. **Sem emoji e sem caractere de IA** (travessão de emenda, reticências, seta, aspas curvas).
3. **O texto não se encurta para caber:** sem corte, abreviação ou valor arredondado. O layout se adapta.
4. **O texto ocupa a caixa:** parágrafo e título sem largura máxima (`max-w-[680px]`, `max-w-[60ch]`,
   `max-w-prose`, `max-width` no CSS) e sem `text-balance`/`text-pretty`. Frase quebrada em linhas curtas
   com a caixa vazia ao lado é "característica de IA" (cobrado em 06/11 e 11/11/2026).
5. **Número com máscara:** telefone, CPF, CEP e dinheiro formatados, nunca crus (`+5511987654321`).
6. **Medir na tela:** print largo (1440 px e ~2850 px) e estreito (320 a 390 px) antes de dar por pronto.

O detalhe, os exemplos e o checklist de cada um estão na skill global.

O `~/.claude/CLAUDE.md` já manda carregá-la sozinho; este ponteiro existe para ela também
aparecer na lista de skills quando a sessão abre dentro deste repo.

A skill é o manual: o antes/depois de cada texto que o Gustavo recusou, a lista de termos
proibidos e o checklist de fechamento. A régua resumida também está na Seção 3 do `CLAUDE.md`
do app e na seção "Texto de tela humano" do `CLAUDE.md` do site.

<!-- Gerado por .claude/skills/sync-pointers.py; não edite à mão. -->
