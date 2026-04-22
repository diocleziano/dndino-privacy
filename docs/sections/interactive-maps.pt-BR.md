# Mapas interativos

Os **mapas interativos** servem para navegar visualmente pelos locais da aventura sobre um mapa gráfico real, usando marcadores clicáveis ligados aos registros dos locais.

Eles são pensados para os casos em que a simples estrutura em árvore já não basta e você quer se mover pelo espaço da campanha de forma mais natural, por exemplo sobre:

- uma cidade
- um castelo
- um bairro
- uma masmorra
- uma região

## Para que servem

Os mapas interativos são úteis quando você quer:

- usar um mapa como superfície principal de navegação
- abrir locais clicando em marcadores visuais
- dar uma estrutura espacial mais clara à campanha
- passar de um mapa de detalhe para um mapa mais amplo

Eles não substituem os **Locais** e não substituem os **Mapas conceituais**:

- os **Locais** continuam sendo os registros reais da campanha
- os **Mapas conceituais** servem para mostrar relações lógicas e narrativas
- os **Mapas interativos** servem, em vez disso, para navegar locais reais sobre uma imagem de mapa

## De onde nascem

Os mapas interativos não são um tipo de registro separado criado em um módulo à parte. Eles nascem a partir das **imagens de mapa** vinculadas aos locais.

Na prática:

1. você liga uma ou mais imagens do tipo `Mapa` a um local
2. escolhe qual delas deve ser usada como mapa interativo padrão
3. nessa mapa adiciona marcadores ligados a locais

## Onde são usados

Os mapas interativos vivem na seção **Locais e Missões**.

Podem ser usados de duas formas:

- como **modo interativo integrado** no dashboard dos locais
- como **painel de mapa grande** aberto a partir de `Mídia`

## Diferença entre modo integrado e painel grande

### Modo interativo integrado

Quando a aventura tem mapas disponíveis, no dashboard dos locais você pode passar da vista normal para a vista `Interativa`.

Nesse modo:

- a parte esquerda da tela mostra o mapa no lugar da árvore clássica dos locais
- o painel da direita continua mostrando o detalhe do local selecionado
- ao clicar nos marcadores você navega diretamente pelos locais

### Painel de mapa grande

A partir do painel `Mídia` de um local você também pode abrir um mapa interativo em um painel dedicado maior.

Esse modo é especialmente útil quando você quer:

- editar marcadores
- ajustar vínculos
- trabalhar com mais precisão sobre o mapa

## Como se prepara um mapa interativo

O fluxo correto é este:

1. abra o local que deve possuir o mapa
2. vá até a seção `Mídia`
3. adicione uma ou mais imagens do tipo `Mapa`
4. escolha qual delas deve se tornar o mapa interativo padrão
5. abra o mapa interativo
6. crie os marcadores e ligue-os aos locais

## Como o mapa padrão é escolhido

Um local pode ter mais de um mapa vinculado. Entre eles, um pode ser marcado como mapa interativo de referência.

Quando o DnDino precisa de entender qual mapa mostrar para um local, usa esta lógica:

- se o local tiver um mapa selecionado explicitamente como mapa interativo, usa esse
- caso contrário usa o primeiro mapa disponível do local
- se o local não tiver mapas próprios, pode usar o mapa de um local pai

## Relação entre local e mapa

Cada mapa interativo pertence a um local.

O local proprietário do mapa não é necessariamente o único local que pode ser aberto a partir dele: os marcadores podem ligar qualquer local da estrutura da aventura.

## Como entrar no modo interativo

No dashboard `Locais`, quando existem mapas disponíveis, você pode passar para a vista `Interativa`.

Nesse modo você encontra:

- cabeçalho do mapa interativo
- seletor `Mapa`
- eventual botão `Voltar`
- eventual botão `Nível superior`
- toggle `Mostrar nomes dos marcadores`
- controles de zoom
- canvas do mapa

## Seletor de mapa

O menu `Mapa` permite escolher qual mapa mostrar entre os disponíveis na aventura.

## Navegação entre mapas

O modo interativo suporta dois tipos de navegação entre mapas.

### Voltar

O botão `Voltar` leva você de volta ao mapa mostrado anteriormente.

### Nível superior

Se o local atual tiver um local pai que possua um mapa interativo, pode aparecer o botão `Nível superior`.

Isso permite subir para um mapa mais amplo.

## O canvas do mapa

O canvas é a superfície central onde o mapa propriamente dito é mostrado.

Aqui você pode:

- ver o mapa
- ver os marcadores
- clicar ou dar duplo clique nos marcadores
- usar zoom e pan

## Zoom e deslocamento

Os mapas interativos suportam:

- zoom para aproximar e afastar
- reposição do zoom
- scroll horizontal e vertical
- pan arrastando o mapa
- gesto de pinça
- zoom com a roda do mouse quando o cursor está sobre o mapa

## Mostrar nomes dos marcadores

Com o toggle `Mostrar nomes dos marcadores` você pode decidir se quer ver também as etiquetas dos marcadores diretamente sobre o mapa.

Quando está ativo:

- cada marcador pode mostrar o seu próprio nome ou, se o título estiver vazio, o nome do local ligado

Quando está desativado:

- ficam visíveis apenas os ícones dos marcadores

## Como funcionam os marcadores

Um marcador contém:

- posição normalizada no mapa
- título opcional
- ligação opcional a um local

O marcador é guardado em relação às coordenadas do mapa e, por isso, continua a ficar no ponto correto mesmo quando você muda o zoom.

Os marcadores também mudam de cor de acordo com o estado do local vinculado, para que o progresso da exploração fique mais fácil de entender de relance no mapa:

- uma cor para locais `Não visitados`
- uma cor para locais `Em visita`
- uma cor para locais `Visitados`

Essas cores são fixas e não mudam com o tema ativo, para que o significado continue consistente em todo o aplicativo.

## Comportamento dos marcadores em leitura

Quando você não está em modo de edição:

- um **clique simples** seleciona um marcador
- um **duplo clique** abre o local ligado

No modo interativo integrado, abrir um local significa atualizar imediatamente o painel da direita.

No painel de mapa grande, abrir um local fecha o painel do mapa e devolve o foco ao local selecionado no dashboard.

## Como criar um marcador

Para criar um marcador no painel de mapa grande:

1. abra o mapa interativo a partir de `Mídia`
2. pressione `Editar`
3. pressione `Novo marcador`
4. escolha o local a associar
5. clique em um ponto do mapa

## Modo Edição

No painel grande existe um verdadeiro estado de edição.

Quando você pressiona `Editar`:

- o mapa entra em modo de edição
- você pode criar novos marcadores
- pode selecionar marcadores existentes para editá-los
- pode arrastar os marcadores para os reposicionar

Quando você pressiona `Bloquear`, sai do modo de edição.

## Novo marcador

Quando você ativa `Novo marcador`:

- o DnDino pede primeiro que escolha o local a associar
- depois convida você a clicar no mapa para o posicionar

## Escolha do local ligado

Quando você está criando ou editando um marcador, o inspetor à direita mostra o seletor de locais.

A partir daí você pode:

- pesquisar por nome
- ver os locais organizados em estrutura hierárquica
- atribuir o marcador ao local correto

## Modificar um marcador existente

Quando um marcador está selecionado em modo de edição, no inspetor você pode alterar:

- `Título do marcador`
- `Local ligado`

Se o título ficar vazio, o DnDino usa como fallback o nome do local ligado ou um título genérico.

## Mover um marcador

Em modo de edição você pode arrastar um marcador para um novo ponto do mapa.

No fim do arrastamento, o DnDino grava:

- nova posição X
- nova posição Y

## Eliminar um marcador

Também a partir do inspetor, quando um marcador está selecionado, você pode usar:

- `Eliminar marcador`

## O inspetor do mapa

O painel lateral do mapa grande muda conforme o estado atual.

### Em leitura

Se você não estiver editando, o inspetor mostra simplesmente a lista dos marcadores existentes.

### Durante a criação de um marcador

Se você tiver ativado `Novo marcador`, o inspetor mostra:

- instruções
- campo de pesquisa
- lista dos locais selecionáveis

### Durante a modificação de um marcador

Se você tiver selecionado um marcador existente, o inspetor mostra:

- campo de título
- seletor do local ligado
- resumo do local atual
- botão para eliminar o marcador

## Lista de marcadores

A lista de marcadores no inspetor também pode ser usada para navegar.

Cada linha mostra:

- título do marcador
- local ligado, se existir

Em leitura, ao clicar na linha você pode abrir o local ligado.

## Como o mapa se comporta no modo integrado

Quando você usa o modo `Interativa` diretamente no dashboard dos locais:

- o mapa segue o local selecionado
- o DnDino tenta mostrar o mapa mais adequado para esse local
- se o local não tiver um mapa próprio, pode usar um mapa de um nível superior

## Herança do mapa a partir do local pai

Uma parte muito útil do sistema é que um local também pode usar um mapa de um nível superior.

Isso permite cenários como:

- o bairro usa o mapa da cidade
- a sala usa o mapa do castelo
- o ponto de interesse usa o mapa da região

## Como abrir um mapa interativo a partir de Mídia

No painel `Mídia` de um local, os mapas do tipo `Mapa` podem mostrar a ação:

- `Abrir mapa interativo`

## Quando vale a pena usar o modo integrado

Vale a pena usar o modo interativo integrado quando você quer:

- navegar rapidamente entre locais
- trabalhar com mapa e painel do local lado a lado
- usar o mapa como alternativa à árvore clássica

## Quando vale a pena usar o painel grande

Vale a pena usar o painel grande quando você quer:

- criar marcadores
- mover marcadores
- alterar vínculos
- trabalhar com mais precisão

## Na prática

Os mapas interativos são a ferramenta certa quando você quer dar aos locais uma verdadeira dimensão espacial.

A ideia-chave é simples:

- o **local** continua sendo o registro principal
- o **mapa** torna-se a superfície visual
- o **marcador** é a ligação operacional entre imagem e conteúdo
