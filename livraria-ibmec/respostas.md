ETAPA 2.4

Quantas colunas aparecem com a janela em ~800px de largura:
Aparecem aproximadamente 4 colunas, dependendo do espaço disponível e do gap.

Quantas colunas aparecem com a janela em ~400px de largura:
Aparecem aproximadamente 2 colunas.

O que acontece quando nao ha largura suficiente nem para uma coluna de 160px:
A coluna ocupa toda a largura disponível e o conteúdo se ajusta automaticamente.

------------------------------------------------------------

ETAPA 3.4

justify-items (no container) vs justify-self (no item):
justify-items define o alinhamento horizontal de todos os itens dentro do container grid.
justify-self altera o alinhamento horizontal apenas de um item específico.

align-items vs align-content:
align-items alinha os itens dentro de suas células.
align-content alinha o conjunto das linhas da grid dentro do container quando sobra espaço.

------------------------------------------------------------

ETAPA 4.4

Por que redefinimos grid-template-areas na media query em vez de apenas grid-template-columns?
Porque apenas mudar o número de colunas não altera a posição das áreas.
Ao redefinir grid-template-areas conseguimos reorganizar a ordem dos elementos para o layout mobile.

------------------------------------------------------------

REVISAO FINAL

Questao 1

Qual e a funcao do -1 na notacao grid-column: 1 / -1?
O -1 representa a última linha da grid.
Isso é mais robusto porque funciona mesmo se a quantidade de colunas mudar futuramente.

------------------------------------------------------------

Questao 2

Diferencie auto-fill de auto-fit dentro de repeat().
auto-fill cria o máximo de colunas possíveis, mesmo vazias.
auto-fit também cria colunas, mas expande as existentes para ocupar o espaço sobrando quando há colunas vazias.

------------------------------------------------------------

Questao 3

O que acontece se voce criar uma grid-template-areas nao-retangular?
O navegador considera a declaração inválida e ignora completamente o grid-template-areas.

------------------------------------------------------------

Questao 4

Qual e o problema:
Os nomes usados em grid-area não correspondem aos nomes definidos em grid-template-areas.

Como corrigir o header:
header { grid-area: cabecalho; }

Como corrigir o footer:
footer { grid-area: rodape; }