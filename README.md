# Gestor de Cargos DGP

Ferramenta de apoio para movimentar cargos e apelidos dos membros no Discord da **Polícia Civil · Jaguaré RP**, sem bot.

A página não altera nada no Discord. Ela monta a movimentação e entrega:

- a lista de cargos para **tirar** e para **pôr**;
- o **apelido** no padrão `Prefixo Primeiro Último - CPF`, com limite de 32 caracteres;
- o **pedido para o Claude** da extensão do navegador aplicar os cliques, com confirmação antes e conferência depois;
- o **resumo** para postar no canal de registro;
- avisos do Regulamento Interno da DGP (medida disciplinar x promoção, TAT na ACADEPOL, ordem dos TAT, requisitos de ingresso).

## Movimentações

Ingresso, promoção, transferência, curso concluído, afastamento/retorno, medida disciplinar, exoneração e ajuste livre. Dá para combinar várias na mesma pessoa; exoneração e ajuste livre ficam sozinhas.

## Lote

Até 5 membros por lote, uma linha por pessoa. O Claude confere todos os perfis, mostra um plano único e executa com pausa de cerca de 20 segundos entre membros. O relatório (`#1 REALIZADO`, `#2 PENDENTE: motivo`…) é colado de volta na ferramenta: realizados vão para o Registro, pendentes e falhas ficam na fila.

## Prefixos de apelido

| Cargo | Prefixo |
|---|---|
| Delegado Titular / Adjunto | `Del.` / `Adj.` |
| Delegado Geral / Geral Adjunto | `DG.` / `DGA.` |
| Escrivão | `Esc.` |
| Investigador-Chefe / Classe Especial | `InvC.` / `InvE.` |
| Investigador 1ª, 2ª, 3ª | `Inv1.` `Inv2.` `Inv3.` |
| Agente Classe Especial | `AgE.` |
| Agente 1ª, 2ª, 3ª | `Ag1.` `Ag2.` `Ag3.` |
| Médico Legista / Perito / Fotógrafo | `Leg.` `Per.` `Fot.` |
| Aluno ACADEPOL | `Al.` |
| Exonerado | `Exon.` |

Se o apelido passar de 32 caracteres, o último nome vira inicial.

## Como usar

Abra `index.html` no navegador (ou publique pelo GitHub Pages). O estado e o registro ficam salvos só no navegador de quem usa.

## Observação

Automatizar contas de usuário vai contra os termos do Discord. Aplique um membro por vez, com conferência, e evite ações em lote.

## Versão

A versão aparece no topo da página e na primeira linha do pedido para o Claude (`[Gestor de Cargos DGP v1.5.2]`). Pelo GitHub Pages, a página compara a própria versão com `version.json` e mostra um aviso quando existe uma mais nova.

Ao publicar uma mudança, suba a versão em `index.html` (`VERSION`) e em `version.json`.

| Versão | Data | Mudanças |
|---|---|---|
| 1.5.2 | 27/10/2026 | Pedido: clicar no cargo com nome exato (nunca o primeiro da busca) e conferir o apelido antes de salvar |
| 1.5.1 | 27/10/2026 | Correções: etiquetas escondidas apareciam no GitHub Pages; espaço vazio no campo da Promoção |
| 1.5 | 26/10/2026 | Movimentações combinadas (ex.: Promoção + Curso) e lote de até 5 membros com fila, status e retorno do resultado do Claude |
| 1.4 | 26/10/2026 | Fluxos de exceção no pedido (regras 1 a 10), medalhas ficam na exoneração, CPF no pedido, indicador de versão |
| 1.3 | 26/10/2026 | Regra para não repetir cargo ou apelido que já existe |
| 1.2 | 26/10/2026 | Nomes exatos dos cargos do servidor |
| 1.1 | 26/10/2026 | Campo "Membro no Discord" e botão "Copiar para o Claude" |
| 1.0 | 26/10/2026 | Primeira versão |
