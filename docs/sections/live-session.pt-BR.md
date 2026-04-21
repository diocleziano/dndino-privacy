# Sessão ao vivo

A **Sessão ao vivo** é o contexto operacional da partida em andamento. Ela não é apenas um temporizador, mas um sistema que mantém juntos:

- o tempo de jogo da sessão
- a timeline dos eventos importantes
- as notas DM rápidas
- o estado dos locais visitados
- as missões ativas ou concluídas
- os combates realizados
- as estatísticas agregadas da sessão

Na prática, quando uma sessão ao vivo está ativa, o DnDino sabe qual é a campanha em andamento e usa esse contexto para conectar entre si várias partes do aplicativo.

## Para que serve

A sessão ao vivo é útil quando você quer usar o DnDino durante uma sessão real em mesa, e não apenas na preparação.

Ela serve para:

- acompanhar o tempo da sessão
- ter uma timeline ordenada dos principais eventos
- anotar rapidamente informações do DM
- marcar locais em visita ou já visitados
- ver um resumo dinâmico da sessão
- recolher automaticamente os dados vindos do combate

## Onde ela é iniciada

A sessão ao vivo é iniciada a partir do **painel da aventura**, no bloco `Sessão ao vivo`.

Se não existir uma sessão ativa, o painel mostra:

- estado pronto
- botão `Iniciar Sessão ao vivo`

Quando você pressiona esse botão, o DnDino cria uma nova sessão do tipo live e a define como sessão global ativa.

## Apenas uma sessão ao vivo por vez

O DnDino gerencia apenas uma sessão ao vivo ativa por vez.

Se já existir uma sessão aberta em outra aventura:

- a nova aventura não pode iniciar uma segunda
- o painel mostra um aviso informando que a sessão ativa pertence a outra campanha

## O que acontece quando uma sessão ao vivo está ativa

Quando uma sessão ao vivo está em andamento:

- a barra superior mostra seu estado
- o temporizador continua sendo atualizado
- os locais seguem esse contexto
- a timeline começa a recolher eventos
- o combate também pode enviar dados para a sessão

A sessão ao vivo se torna, assim, o fio condutor da partida em andamento.

## Estado da sessão

A sessão ao vivo pode estar em três estados:

- ativa
- em pausa
- interrompida

### Ativa

É o estado normal enquanto a sessão está em andamento. O temporizador continua correndo e os eventos são registrados com o tempo decorrido correto.

### Em pausa

A sessão pode ser colocada em pausa a partir do painel da aventura ou da barra superior.

Quando está em pausa:

- o temporizador para
- a sessão ainda assim continua aberta
- ela pode ser retomada depois

### Interrompida

Se o aplicativo for fechado enquanto a sessão ainda estiver ativa, o DnDino a reabre como `interrompida` no próximo início e registra um evento dedicado na timeline.

Isso permite:

- não perder a sessão
- entender que houve uma interrupção
- retomar o trabalho manualmente

## O painel Sessão ao vivo no painel da aventura

No painel da aventura, esse bloco mostra o estado atual da sessão.

Se a sessão pertencer à aventura aberta, o painel mostra:

- título da sessão
- temporizador em tempo real
- estado (`Em andamento` ou `Em pausa`)
- indicação de que o player é global
- botões:
  - `Pausa` ou `Retomar`
  - `Fechar e salvar`

Se não houver uma sessão ao vivo ativa:

- aparece o botão `Iniciar Sessão ao vivo`

Se houver uma sessão ativa, mas ela pertencer a outra aventura:

- o painel mostra que a sessão ao vivo está ocupada em outro lugar

## A sessão ao vivo na barra superior

Quando uma sessão ao vivo está ativa, a barra superior do aplicativo mostra um indicador dedicado.

Esse elemento contém:

- título da sessão
- temporizador
- indicador de estado

Ao clicar nele, abre-se um popover de controle rápido.

## O popover da sessão ao vivo na barra superior

Pelo popover da barra superior você pode fazer operações muito rápidas sem sair da tela atual.

Aqui você encontra:

- `Pausa` ou `Retomar`
- `Fechar e salvar`
- editor rápido para `Nota DM`
- timeline da sessão
- ações rápidas sobre o local atualmente em visita
- resumo compacto da sessão ao vivo

## Nota DM rápida

No popover da sessão ao vivo você pode escrever uma **Nota DM** e adicioná-la imediatamente à timeline.

Isso é útil para anotar rapidamente:

- decisões dos jogadores
- ganchos narrativos
- consequências a lembrar
- ideias improvisadas que surgiram durante a partida

As notas DM são registradas como eventos da timeline.

## Timeline da sessão

A timeline é o registo cronológico da sessão ao vivo.

Cada evento guarda:

- título
- detalhe
- momento da sessão em que aconteceu

A timeline pode conter eventos do sistema e notas DM.

## Tipos de eventos registrados

Os eventos mais importantes que o DnDino registra automaticamente incluem:

- `Sessão iniciada`
- `Sessão em pausa`
- `Sessão retomada`
- `Sessão interrompida por fechamento do app`
- `Entrada no local`
- `Saída do local`
- `Estado do local atualizado`
- `Missão ativada`
- `Missão concluída`
- `Combate iniciado`
- `Combate encerrado`
- `Dano causado em combate`
- `Dano sofrido em combate`
- `Nota DM`

## Ligação com os locais

A sessão ao vivo está diretamente ligada aos locais da aventura ativa.

Quando você atualiza um local dentro do contexto da sessão:

- a mudança de estado é registrada
- a timeline é atualizada
- o resumo da sessão muda em consequência

Os dados mais importantes acompanhados do lado dos locais são:

- locais em visita
- locais visitados
- missões ativas
- missões concluídas

## Fechamento automático do local anterior em visita

Nas configurações também existe uma lógica ligada à sessão ao vivo: quando um local é colocado como `Em visita`, o local que antes estava em visita pode ser marcado automaticamente como `Visitado`.

Essa função só vale quando existe uma sessão ao vivo ativa e é muito útil para manter coerente o acompanhamento da exploração.

## Resumo da sessão ao vivo

O resumo da sessão ao vivo agrega os dados mais importantes recolhidos durante a sessão.

Entre os principais valores estão:

- locais visitados
- locais em visita
- missões ativas
- missões concluídas
- combates realizados
- inimigos derrotados
- heróis caídos
- duração total dos combates

A sessão ao vivo também mantém dois resumos muito úteis para os personagens:

- dano causado pelos heróis
- dano sofrido pelos heróis

## Integração com o combate

A sessão ao vivo e o combate estão fortemente ligados.

Quando você inicia um combate durante uma sessão ao vivo, o DnDino registra:

- `Combate iniciado`

Durante o combate, ele pode registrar:

- `Dano causado em combate`
- `Dano sofrido em combate`

Quando você encerra o combate, ele registra:

- `Combate encerrado`
- duração do confronto
- inimigos derrotados
- heróis caídos

## Dano causado e dano sofrido

A sessão ao vivo acompanha o dano com dois rankings separados:

- `Dano causado pelos personagens`
- `Dano sofrido pelos personagens`

Essa contagem foi pensada apenas para os heróis da aventura, e não para todos os participantes do confronto.

## Heróis caídos

Quando um combate termina, o resumo da sessão ao vivo também pode aumentar a contagem de **heróis caídos**.

Esse dado é alimentado diretamente pelo resultado final do combate.

## Sessão ao vivo e Janela dos Jogadores

A sessão ao vivo não é a mesma coisa que a **Janela dos Jogadores**, mas as duas coisas estão ligadas.

A sessão ao vivo fornece o contexto geral da partida, enquanto a janela dos jogadores é o canal de apresentação visual.

Em particular:

- durante o combate, a janela dos jogadores pode mostrar intro, turno atual e resumo final
- fora do combate, a janela dos jogadores ainda pode ser usada para mostrar imagens e conteúdos do contexto ativo

## Fechamento e salvamento

Quando você escolhe `Fechar e salvar`, o DnDino:

- finaliza a sessão
- salva os dados recolhidos
- persiste a timeline na sessão ligada à aventura
- fecha o contexto live global

Depois do fechamento, a sessão continua disponível como sessão salva.

## Visualização de uma sessão salva

Uma sessão ao vivo já concluída pode ser reaberta como detalhe.

No painel de detalhe você encontra:

- resumo e timeline
- duração registrada
- locais visitados
- combates realizados
- inimigos derrotados
- heróis caídos
- rankings de dano causado e sofrido pelos personagens

## Quando vale a pena usar a sessão ao vivo

A sessão ao vivo é especialmente útil quando você quer:

- manter o DnDino aberto durante a partida
- anotar rapidamente o que realmente acontece na mesa
- saber quais locais foram visitados
- ter uma timeline ordenada dos eventos-chave
- fazer o combate alimentar automaticamente o resumo da sessão

## Na prática

A sessão ao vivo é a ponte entre:

- preparação
- gestão operacional da partida
- memória final da sessão

Quando é bem usada, reduz muito o risco de perder informações importantes durante o jogo e torna muito mais simples reconstruir depois o que realmente aconteceu na campanha.
