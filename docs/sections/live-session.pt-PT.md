# Sessão live

A **Sessão live** é o contexto operativo da partida em curso. Não é simplesmente um temporizador, mas um sistema que mantém juntos:

- o tempo de jogo da sessão
- a timeline dos acontecimentos importantes
- as notas DM rápidas
- o estado dos locais visitados
- as missões ativas ou concluídas
- os combates realizados
- as estatísticas agregadas da sessão

Na prática, quando uma sessão live está ativa, o DnDino sabe qual é a campanha em curso e usa esse contexto para ligar entre si várias partes da aplicação.

## Para que serve

A sessão live é útil quando queres usar o DnDino durante uma sessão real à mesa, e não apenas na preparação.

Serve para:

- acompanhar o tempo da sessão
- ter uma timeline ordenada dos acontecimentos principais
- anotar rapidamente informação do DM
- marcar locais em visita ou já visitados
- ver um resumo dinâmico da sessão
- recolher automaticamente os dados provenientes do combate

## Onde se inicia

A sessão live é iniciada a partir do controlo no centro da **topbar** quando estás dentro de uma página da aventura, como dashboard, locais ou combate.

Se não existir uma sessão ativa, o controlo mostra a ação de início. Ao carregares nela, o DnDino pede confirmação e cria uma nova sessão live para a aventura atual.

Assim não precisas de voltar à dashboard só para iniciar a sessão: o comando fica disponível onde estás a trabalhar.

## Apenas uma sessão live de cada vez

O DnDino gere apenas uma sessão live ativa de cada vez.

Se já existir uma sessão aberta noutra aventura:

- a nova aventura não pode iniciar uma segunda
- o painel mostra um aviso a indicar que a sessão ativa pertence a outra campanha

## O que acontece quando uma sessão live está ativa

Quando uma sessão live está a decorrer:

- a barra superior mostra o seu estado
- o temporizador continua a atualizar-se
- os locais seguem esse contexto
- a timeline começa a recolher acontecimentos
- o combate também pode enviar dados para a sessão

A sessão live torna-se assim o fio condutor da partida em curso.

## Estado da sessão

A sessão live pode encontrar-se em três estados:

- ativa
- em pausa
- interrompida

### Ativa

É o estado normal enquanto a sessão está a decorrer. O temporizador continua a avançar e os acontecimentos são registados com o tempo decorrido correto.

### Em pausa

A sessão pode ser colocada em pausa a partir da topbar.

Quando está em pausa:

- o temporizador pára
- a sessão continua, ainda assim, aberta
- pode ser retomada mais tarde

### Interrompida

Se a aplicação for fechada enquanto a sessão ainda estiver ativa, o DnDino reabre-a como `interrompida` no arranque seguinte e regista um acontecimento próprio na timeline.

Isto permite:

- não perder a sessão
- perceber que houve uma interrupção
- retomar o trabalho manualmente

## Controlo Sessão live na topbar

Nas páginas da aventura, a topbar mostra o controlo da sessão live ao centro.

Se a sessão pertencer à aventura aberta, o controlo mostra:

- título da sessão
- temporizador em tempo real
- estado (`Em curso` ou `Em pausa`)
Se não existir nenhuma sessão live ativa:

- aparece o comando para iniciar a sessão live da aventura atual

Se existir uma sessão ativa, mas pertencer a outra aventura:

- o controlo mostra que a sessão live está ocupada noutro lado

## A sessão live na topbar

Quando uma sessão live está ativa, a barra superior da aplicação mostra um indicador dedicado.

Para a descrição completa da topbar, consulta a página `Topbar`.

![Sessão live ativa na topbar](../images/en_sessionelive_attiva_topbar.png){ .img-shot }

## O painel rápido da sessão live

No painel rápido da sessão podes fazer operações muito rápidas sem sair do ecrã atual.

Aqui encontras:

- `Pausa` ou `Retomar`
- `Fechar e guardar`
- editor rápido para `Nota DM`
- timeline da sessão
- ações rápidas sobre o local atualmente em visita
- resumo live compacto

## Nota DM rápida

No popover da sessão live podes escrever uma **Nota DM** e adicioná-la de imediato à timeline.

Isto é útil para apontar rapidamente:

- decisões dos jogadores
- ideias narrativas
- consequências a recordar
- ideias improvisadas surgidas durante a partida

As notas DM ficam registadas como acontecimentos da timeline.

## Timeline da sessão

A timeline é o registo cronológico da sessão live.

Cada acontecimento guarda:

- título
- detalhe
- momento da sessão em que aconteceu

A timeline pode conter acontecimentos de sistema e notas DM.

## Tipos de acontecimentos registados

Os acontecimentos mais importantes que o DnDino regista automaticamente incluem:

- `Sessão iniciada`
- `Sessão em pausa`
- `Sessão retomada`
- `Sessão interrompida por fecho da app`
- `Entrada no local`
- `Saída do local`
- `Estado do local atualizado`
- `Missão ativada`
- `Missão concluída`
- `Combate iniciado`
- `Combate terminado`
- `Nota DM`

## Ligação com os locais

A sessão live está diretamente ligada aos locais da aventura ativa.

Quando atualizas um local dentro do contexto da sessão:

- a alteração de estado é registada
- a timeline é atualizada
- o resumo live muda em conformidade

Os dados mais importantes acompanhados do lado dos locais são:

- locais em visita
- locais visitados
- missões ativas
- missões concluídas

## Fecho automático do local anterior em visita

Nas definições existe também uma lógica ligada à sessão live: quando um local é colocado em `Em visita`, o local que antes estava em visita pode ser marcado automaticamente como `Visitado`.

Esta função só se aplica quando existe uma sessão live ativa e é muito útil para manter coerente o acompanhamento da exploração.

## Recriar uma sessão live já jogada

Se te esqueceste de iniciar a sessão live durante a partida, podes recriá-la manualmente a partir do cartão **Sessões** no painel da aventura.

A sessão recriada não é uma simples nota: é guardada como sessão live e usa os dados reais que já existem na aventura.

Ao criá-la, podes indicar:

- hora de início e hora de fim
- locais visitados durante a sessão
- notas da sessão

DnDino inclui automaticamente os combates concluídos que começaram dentro do intervalo selecionado. Assim, as estatísticas da sessão podem usar dano, inimigos derrotados, duração dos combates e tempos médios dos turnos já registados pelos combates reais.

Esta função serve para recuperar uma sessão jogada sem perder o valor das estatísticas.

## Eliminar uma sessão

Na lista de sessões, cada linha tem um botão de eliminação. Antes de apagar, DnDino mostra uma confirmação, porque a operação remove definitivamente a sessão guardada.

## Resumo live

![Resumo da sessão live](../images/en_sessionelive_riepilogo_1.png){ .img-shot }
![Gráficos da sessão live](../images/en_sessionelive_riepilogo_2.png){ .img-shot }


O resumo live agrega os dados mais importantes recolhidos durante a sessão.

Entre os principais valores estão:

- locais visitados
- locais em visita
- missões ativas
- missões concluídas
- combates realizados
- inimigos derrotados
- heróis caídos
- duração total dos combates

A sessão live mantém também dois resumos muito úteis para as personagens:

- dano causado pelos heróis
- dano sofrido pelos heróis
- tempo médio dos turnos, quando vem de combates concluídos

## Integração com o combate

A sessão live e o combate estão fortemente ligados.

Quando inicias um combate durante uma sessão live, o DnDino regista:

- `Combate iniciado`

Durante o combate, pode recolher:

- dados agregados úteis para o resumo e as estatísticas

Quando fechas o combate, regista:

- `Combate terminado`
- duração do confronto
- inimigos derrotados
- heróis caídos

## Dano causado e dano sofrido

A sessão live acompanha o dano com duas classificações separadas:

- `Dano causado pelas personagens`
- `Dano sofrido pelas personagens`

Esta contagem foi pensada apenas para os heróis da aventura, não para todos os participantes do confronto.

O detalhe da sessão guardada também pode mostrar gráficos dos combates concluídos durante essa sessão:

- dano causado por combate
- dano sofrido por combate
- tempo médio dos turnos por combate

Cada combate fica no eixo horizontal em ordem cronológica. As personagens que participaram aparecem mesmo quando num combate causaram ou sofreram `0` dano, para manter a série coerente. Se uma personagem não participou num combate, não é adicionada nesse ponto.

Estes gráficos ajudam a perceber quem teve mais impacto durante a sessão e quem absorveu mais dano ao longo dos encontros.

O gráfico do tempo dos turnos ajuda a perceber quanto tempo os heróis e o Mestre demoram em média durante os combates da sessão.

## Heróis caídos

Quando um combate termina, o resumo da sessão live também pode aumentar a contagem de **heróis caídos**.

Este dado é alimentado diretamente pelo resultado final do combate.

## Sessão live e Janela dos Jogadores

A sessão live não coincide com a **Janela dos Jogadores**, mas as duas coisas estão ligadas.

A sessão live fornece o contexto geral da partida, enquanto a janela dos jogadores é o canal de apresentação visual.

Em particular:

- durante o combate, a janela dos jogadores pode mostrar intro, turno atual e resumo final
- fora do combate, a janela dos jogadores pode continuar a ser usada para mostrar imagens e conteúdos do contexto ativo

## Fecho e gravação

Quando escolhes `Fechar e guardar`, o DnDino:

- finaliza a sessão
- guarda os dados recolhidos
- persiste a timeline na sessão ligada à aventura
- fecha o contexto live global

Depois do fecho, a sessão continua disponível como sessão guardada.

## Visualização de uma sessão guardada

Uma sessão live já concluída pode ser reaberta como detalhe.

No painel de detalhe encontras:

- resumo e timeline
- duração registada
- locais visitados
- combates realizados
- inimigos derrotados
- heróis caídos
- classificações de dano causado e sofrido pelas personagens
- gráficos de dano causado e sofrido nos combates da sessão
- gráfico do tempo médio dos turnos, quando disponível

## Quando vale a pena usar a sessão live

A sessão live é especialmente útil quando queres:

- manter o DnDino aberto durante a partida
- anotar rapidamente o que realmente acontece à mesa
- saber que locais foram visitados
- ter uma timeline ordenada dos acontecimentos-chave
- fazer com que o combate alimente automaticamente o resumo da sessão

## Na prática

A sessão live é a ponte entre:

- preparação
- gestão operativa da partida
- memória final da sessão

Quando bem usada, reduz muito o risco de perder informação importante durante o jogo e torna muito mais simples reconstruir depois o que realmente aconteceu na campanha.
