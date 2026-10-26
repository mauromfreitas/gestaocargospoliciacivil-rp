# Gestor de Cargos DGP

Ferramenta de apoio para movimentar cargos e apelidos dos membros no Discord da **Polícia Civil · Jaguaré RP**, sem bot.

A página não altera nada no Discord. Ela monta a movimentação e entrega:

- a lista de cargos para **tirar** e para **pôr**;
- o **apelido** no padrão `Prefixo Primeiro Último - CPF`, com limite de 32 caracteres;
- o **pedido para o Claude** da extensão do navegador aplicar os cliques, com confirmação antes e conferência depois;
- o **resumo** para postar no canal de registro;
- avisos do Regulamento Interno da DGP (medida disciplinar x promoção, TAT na ACADEPOL, ordem dos TAT, requisitos de ingresso).

## Movimentações

Ingresso, promoção, transferência, curso concluído, afastamento/retorno, medida disciplinar, exoneração e ajuste livre.

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
