# Mapas interativos

Os **mapas interativos** servem para navegar visualmente pelos locais da aventura sobre um verdadeiro mapa gráfico, usando marcadores clicáveis ligados aos registos dos locais.

São pensados para os casos em que a simples estrutura em árvore já não chega e queres mover-te pelo espaço da campanha de forma mais natural, por exemplo sobre:

- uma cidade
- um castelo
- um bairro
- um dungeon
- uma região

## Para que servem

Os mapas interativos são úteis quando queres:

- usar um mapa como superfície principal de navegação
- abrir locais clicando em marcadores visuais
- dar uma estrutura espacial mais clara à campanha
- passar de um mapa de detalhe para um mapa mais amplo

Não substituem os **Locais** nem substituem os **Mapas conceptuais**:

- os **Locais** continuam a ser os registos reais da campanha
- os **Mapas conceptuais** servem para mostrar relações lógicas e narrativas
- os **Mapas interativos** servem, em vez disso, para navegar locais reais sobre uma imagem de mapa

## De onde nascem

Os mapas interativos não são um tipo de registo separado criado num módulo à parte. Nascem a partir das **imagens de mapa** ligadas aos locais.

Na prática:

1. ligas uma ou mais imagens do tipo `Mapa` a um local
2. escolhes qual delas deve ser usada como mapa interativo por defeito
3. nessa mapa adicionas marcadores ligados a locais

## Onde são usados

Os mapas interativos vivem na secção **Locais e Missões**.

Podem ser usados de duas formas:

- como **modo interativo integrado** na dashboard dos locais
- como **painel de mapa grande** aberto a partir de `Média`

## Diferença entre modo integrado e painel grande

### Modo interativo integrado

Quando a aventura tem mapas disponíveis, na dashboard dos locais podes passar da vista normal para a vista `Interativa`.

Neste modo:

- a parte esquerda do ecrã mostra o mapa em vez da árvore clássica dos locais
- o painel da direita continua a mostrar o detalhe do local selecionado
- ao clicares nos marcadores navegas diretamente pelos locais

### Painel de mapa grande

A partir do painel `Média` de um local também podes abrir um mapa interativo num painel dedicado mais amplo.

Este modo é particularmente útil quando queres:

- editar marcadores
- corrigir ligações
- trabalhar com mais precisão sobre o mapa

## Como se prepara um mapa interativo

O fluxo correto é este:

1. abre o local que deve possuir o mapa
2. vai à secção `Média`
3. adiciona uma ou mais imagens do tipo `Mapa`
4. escolhe qual delas deve tornar-se o mapa interativo por defeito
5. abre o mapa interativo
6. cria os marcadores e liga-os aos locais

## Como é escolhido o mapa por defeito

Um local pode ter mais do que um mapa ligado. Entre eles, um pode ser marcado como mapa interativo de referência.

Quando o DnDino precisa de perceber que mapa mostrar para um local, usa esta lógica:

- se o local tiver um mapa selecionado explicitamente como mapa interativo, usa esse
- caso contrário usa o primeiro mapa disponível do local
- se o local não tiver mapas próprios, pode usar o mapa de um local pai

## Relação entre local e mapa

Cada mapa interativo pertence a um local.

O local proprietário do mapa não é obrigatoriamente o único local que pode ser aberto a partir dele: os marcadores podem ligar qualquer local da estrutura da aventura.

## Como entrar no modo interativo

Na dashboard `Locais`, quando existem mapas disponíveis, podes passar para a vista `Interativa`.

Nesse modo encontras:

- cabeçalho do mapa interativo
- seletor `Mapa`
- eventual botão `Voltar`
- eventual botão `Nível superior`
- toggle `Mostrar nomes dos marcadores`
- controlos de zoom
- canvas do mapa

## Seletor de mapa

O menu `Mapa` permite escolher qual mapa mostrar entre os disponíveis na aventura.

## Navegação entre mapas

O modo interativo suporta dois tipos de navegação entre mapas.

### Voltar

O botão `Voltar` devolve-te ao mapa mostrado anteriormente.

### Nível superior

Se o local atual tiver um local pai que possua um mapa interativo, pode aparecer o botão `Nível superior`.

Isto permite-te subir para um mapa mais amplo.

## O canvas do mapa

O canvas é a superfície central onde o mapa propriamente dito é mostrado.

Aqui podes:

- ver o mapa
- ver os marcadores
- clicar ou fazer duplo clique nos marcadores
- usar zoom e pan

## Zoom e deslocação

Os mapas interativos suportam:

- zoom aproximar e afastar
- reposição do zoom
- scroll horizontal e vertical
- pan arrastando o mapa
- gesto de pinch
- zoom com a roda do rato quando o cursor está sobre o mapa

## Mostrar nomes dos marcadores

Com o toggle `Mostrar nomes dos marcadores` podes decidir se queres ver também as etiquetas dos marcadores diretamente sobre o mapa.

Quando está ativo:

- cada marcador pode mostrar o seu próprio nome ou, se o título estiver vazio, o nome do local ligado

Quando está desativado:

- ficam visíveis apenas os ícones dos marcadores

## Como funcionam os marcadores

Um marcador contém:

- posição normalizada no mapa
- título opcional
- ligação opcional a um local

O marcador é guardado relativamente às coordenadas do mapa e, por isso, continua a ficar no ponto correto mesmo quando mudas o zoom.

Os marcadores também mudam de cor consoante o estado do local associado, para que o progresso da exploração fique mais legível de relance no mapa:

- uma cor para locais `Não visitados`
- uma cor para locais `Em visita`
- uma cor para locais `Visitados`

Estas cores são fixas e não mudam com o tema ativo, para que o significado se mantenha coerente em toda a aplicação.

## Comportamento dos marcadores em leitura

Quando não estás em modo de edição:

- um **clique simples** seleciona um marcador
- um **duplo clique** abre o local ligado

No modo interativo integrado, abrir um local significa atualizar de imediato o painel da direita.

No painel de mapa grande, abrir um local fecha o painel do mapa e devolve o foco ao local selecionado na dashboard.

## Como criar um marcador

Para criar um marcador no painel de mapa grande:

1. abre o mapa interativo a partir de `Média`
2. carrega em `Editar`
3. carrega em `Novo marcador`
4. escolhe o local a associar
5. clica num ponto do mapa

## Modo Edição

No painel grande existe um verdadeiro estado de edição.

Quando carregas em `Editar`:

- o mapa entra em modo de edição
- podes criar novos marcadores
- podes selecionar marcadores existentes para os editar
- podes arrastar os marcadores para os reposicionar

Quando carregas em `Bloquear`, sais do modo de edição.

## Novo marcador

Quando ativas `Novo marcador`:

- o DnDino pede-te primeiro para escolher o local a associar
- depois convida-te a clicar no mapa para o posicionar

## Escolha do local ligado

Quando estás a criar ou editar um marcador, o inspector à direita mostra o seletor de locais.

A partir daí podes:

- pesquisar por nome
- ver os locais organizados numa estrutura hierárquica
- atribuir o marcador ao local correto

## Modificar um marcador existente

Quando um marcador está selecionado em modo de edição, no inspector podes alterar:

- `Título do marcador`
- `Local ligado`

Se o título ficar vazio, o DnDino usa como fallback o nome do local ligado ou um título genérico.

## Mover um marcador

Em modo de edição podes arrastar um marcador para um novo ponto do mapa.

No final do arrastamento, o DnDino guarda:

- nova posição X
- nova posição Y

## Eliminar um marcador

Também a partir do inspector, quando um marcador está selecionado, podes usar:

- `Eliminar marcador`

## O inspector do mapa

O painel lateral do mapa grande muda consoante o estado atual.

### Em leitura

Se não estiveres a editar, o inspector mostra simplesmente a lista dos marcadores existentes.

### Durante a criação de um marcador

Se tiveres ativado `Novo marcador`, o inspector mostra:

- instruções
- campo de pesquisa
- lista dos locais selecionáveis

### Durante a modificação de um marcador

Se tiveres selecionado um marcador existente, o inspector mostra:

- campo de título
- seletor do local ligado
- resumo do local atual
- botão para eliminar o marcador

## Lista de marcadores

A lista de marcadores no inspector também pode ser usada para navegar.

Cada linha mostra:

- título do marcador
- local ligado, se existir

Em leitura, ao clicares na linha podes abrir o local ligado.

## Como o mapa se comporta no modo integrado

Quando usas o modo `Interativa` diretamente na dashboard dos locais:

- o mapa segue o local selecionado
- o DnDino tenta mostrar o mapa mais adequado para esse local
- se o local não tiver um mapa próprio, pode usar um mapa de um nível superior

## Herança do mapa a partir do local pai

Uma parte muito útil do sistema é que um local pode usar também um mapa de um nível superior.

Isto permite cenários como:

- o bairro usa o mapa da cidade
- a sala usa o mapa do castelo
- o ponto de interesse usa o mapa da região

## Como abrir um mapa interativo a partir de Média

No painel `Média` de um local, os mapas do tipo `Mapa` podem mostrar a ação:

- `Abrir mapa interativo`

## Quando vale a pena usar o modo integrado

Vale a pena usar o modo interativo integrado quando queres:

- navegar rapidamente entre locais
- trabalhar com mapa e painel do local lado a lado
- usar o mapa como alternativa à árvore clássica

## Quando vale a pena usar o painel grande

Vale a pena usar o painel grande quando queres:

- criar marcadores
- mover marcadores
- alterar ligações
- trabalhar com mais precisão

## Na prática

Os mapas interativos são a ferramenta certa quando queres dar aos locais uma verdadeira dimensão espacial.

A ideia-chave é simples:

- o **local** continua a ser o registo principal
- o **mapa** torna-se a superfície visual
- o **marcador** é a ligação operativa entre imagem e conteúdo
