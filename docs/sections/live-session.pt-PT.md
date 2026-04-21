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

A sessão live é iniciada a partir do **painel da aventura**, no painel `Sessão Live`.

Se não existir uma sessão ativa, o painel mostra:

- estado pronto
- botão `Iniciar Sessão Live`

Quando carregas no botão, o DnDino cria uma nova sessão do tipo live e define-a como sessão global ativa.

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

A sessão pode ser colocada em pausa a partir do painel da aventura ou da barra superior.

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

## O painel Sessão Live no painel da aventura

No painel da aventura, este bloco mostra o estado atual da sessão.

Se a sessão pertencer à aventura aberta, o painel mostra:

- título da sessão
- temporizador em tempo real
- estado (`Em curso` ou `Em pausa`)
- indicação de que o player é global
- botões:
  - `Pausa` ou `Retomar`
  - `Fechar e guardar`

Se não existir nenhuma sessão live ativa:

- aparece o botão `Iniciar Sessão Live`

Se existir uma sessão ativa, mas pertencer a outra aventura:

- o painel mostra que a sessão live está ocupada noutro lado

## A sessão live na topbar

Quando uma sessão live está ativa, a barra superior da aplicação mostra um indicador dedicado.

Este elemento contém:

- título da sessão
- temporizador
- indicador de estado

Ao clicares nele, abre-se um popover de controlo rápido.

## O popover da sessão live na topbar

No popover da topbar podes fazer operações muito rápidas sem sair do ecrã atual.

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
- `Dano causado em combate`
- `Dano sofrido em combate`
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

## Resumo live

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

## Integração com o combate

A sessão live e o combate estão fortemente ligados.

Quando inicias um combate durante uma sessão live, o DnDino regista:

- `Combate iniciado`

Durante o combate, pode registar:

- `Dano causado em combate`
- `Dano sofrido em combate`

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
