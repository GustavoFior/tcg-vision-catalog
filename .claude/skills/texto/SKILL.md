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

O `~/.claude/CLAUDE.md` já manda carregá-la sozinho; este ponteiro existe para ela também
aparecer na lista de skills quando a sessão abre dentro deste repo.

A skill é o manual: o antes/depois de cada texto que o Gustavo recusou, a lista de termos
proibidos e o checklist de fechamento. A régua resumida também está na Seção 3 do `CLAUDE.md`
do app e na seção "Texto de tela humano" do `CLAUDE.md` do site.

<!-- Gerado por .claude/skills/sync-pointers.py; não edite à mão. -->
