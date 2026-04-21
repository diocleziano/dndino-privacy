# Locais

A seção **Locais** reúne tudo o que está relacionado aos espaços jogáveis de uma aventura: cidades, masmorras, salas, áreas narrativas, missões ligadas, presenças, combates, imagens, mapas e mapas interativos.

É uma das seções mais ricas do aplicativo, porque junta:

- estrutura narrativa
- estado de exploração
- conteúdo para mostrar aos jogadores
- presenças contextuais
- acesso rápido a combates

## Para que serve a seção Locais

O painel de locais serve para organizar a aventura tanto no plano espacial quanto no narrativo.

Aqui você pode:

- criar locais e missões
- construir hierarquias de locais e sublocais
- vincular imagens e mapas
- gerenciar as presenças em um local
- criar e reabrir combates ligados a um local específico
- manter descrições separadas para DM e jogadores
- usar um mapa interativo para se mover entre locais

## Como chegar lá

A seção é aberta a partir do **painel da aventura**, entrando no cartão `Locais e Missões`.

A partir desse cartão você pode:

- abrir todo o painel de locais
- usar atalhos rápidos para um local recente, quando existirem
- usar atalhos rápidos para um combate recente ligado a um local

## Estrutura da tela

O painel `Locais` é organizado em torno de dois modos principais:

- `Normal`
- `Interativo`

e de duas áreas:

- uma **coluna esquerda** com árvore, busca, filtros e ações rápidas
- um **painel direito** com o detalhe do local selecionado

## Modo Normal e Interativo

### Modo Normal

É o modo clássico, pensado para trabalhar diretamente sobre:

- a árvore de locais
- o detalhe do local selecionado
- presenças
- combates
- mídia
- notas

É o modo mais indicado para preparar e editar a aventura.

### Modo Interativo

O modo `Interativo` fica disponível quando a aventura possui mapas interativos prontos para uso.

Nesse modo, o foco muda para a navegação por mapa:

- a parte esquerda da tela mostra o mapa interativo no lugar da árvore clássica
- os marcadores podem ser selecionados
- com duplo clique é possível abrir o local vinculado no painel direito
- os nomes dos marcadores podem ser mostrados ou ocultados
- estão disponíveis zoom e deslocamento do mapa

A partir da aba `Mídia` você ainda pode abrir rapidamente o mapa interativo associado a um dos mapas do local, mas no modo `Interativo` o mapa passa a ser o conteúdo principal da parte esquerda do painel.

## A coluna esquerda

A coluna esquerda é o painel de navegação desta seção.

Aqui você encontra:

- busca
- filtros
- um resumo compacto
- a árvore de locais e missões

### Menu contextual sobre locais na árvore

No modo em árvore você pode **clicar com o botão direito em um local** para abrir um menu contextual com ações rápidas diretamente nesse nó.

As ações disponíveis são:

- `Remover vínculo`
- `Adicionar vínculo`
- `Adicionar sublocal`
- `Adicionar personagem`
- `Criar mapa conceitual`
- `Criar combate`
- `Editar`

Esse menu é uma das formas mais rápidas de construir a estrutura da aventura enquanto você trabalha na árvore.

### Filtros e resumo

A barra lateral também mostra um resumo compacto com:

- total de locais
- número de missões
- número de locais em visita

Dependendo do modo e do contexto, os filtros podem incluir:

- todos
- locais
- missões
- em visita
- ativas

## Criar um local ou uma missão

Para criar um novo registro, use o botão de criação no painel de locais.

O formulário é dividido em três grupos principais:

- `Informações principais`
- `Descrições`
- `Recursos do local`

## Informações principais do local

No formulário você pode preencher:

- `Nome`
- local pai ou vínculos com locais pai
- `Tipo`
- `Marcador`
- estado do local ou estado da missão

### Tipo: Local ou Missão

O campo `Tipo` permite escolher se o registro é um:

- `Local`
- `Missão`

Se o registro for um **Local**, ele usa o estado de visita:

- não visitado
- em visita
- visitado

Se o registro for uma **Missão**, ele usa em vez disso o estado de progressão:

- inativa
- indisponível
- ativa
- concluída

## Locais pai e hierarquia

O formulário dos locais suporta uma hierarquia avançada.

Você pode selecionar um ou mais locais pai, e o DnDino salva essa ligação como uma estrutura hierárquica real.

Isso significa que um local pode:

- estar na raiz da aventura
- existir como sublocal de outro local
- estar vinculado em mais de um ponto da estrutura, quando fizer sentido

O formulário ainda impede ciclos, excluindo automaticamente o próprio local e sua subárvore da lista de possíveis pais.

## Marcadores do local

Cada local pode ter um ou mais marcadores especiais, visíveis também no painel.

Os marcadores disponíveis incluem:

- perigoso
- importante
- secreto
- bloqueado

Eles servem como destaques visuais rápidos para você ler a aventura de imediato.

## Descrições do local

A seção `Descrições` do formulário é dividida em vários campos de texto formatado:

- `Descrição DM`
- `Descrição jogadores`
- `Pistas`
- `Tesouros`
- `Notas`

Essa separação é muito útil porque permite distinguir:

- o que o DM deve saber
- o que os jogadores podem ver ou descobrir
- informações de apoio, como pistas e tesouros

## Links internos nos textos do local

O sistema de **links internos** também é muito útil em `Locais`.

Aqui não se trata tanto de automatizar ataques, mas principalmente de tornar o texto do local **navegável** e mais rápido de usar à mesa.

Dentro dos campos de texto formatado de um local, você pode inserir links para:

- `Personagem`
- `Local`
- `Magia`
- `Talento`
- `Regra`
- e, quando fizer sentido, também links de rolagem

### Por que eles são úteis nos locais

As descrições dos locais costumam conter muitas referências:

- personagens presentes ou mencionados
- locais ligados
- objetos ou magias mencionadas no texto
- regras especiais da cena

Transformar essas referências em links internos permite:

- abrir imediatamente a ficha de um personagem citado
- saltar direto para outro local da aventura
- consultar uma magia ou uma regra sem sair do contexto
- escrever descrições mais densas, mas ainda fáceis de navegar

### Exemplos práticos

Você pode vincular um personagem mencionado no local, como `capitão Arven`, ou outro local citado no texto, como `Cripta Submersa`.

Assim, a descrição deixa de ser apenas narrativa: também vira um atalho de navegação.

### Onde eles funcionam melhor

As melhores partes da ficha de local para usar links internos são:

- `Descrição DM`
- `Descrição jogadores`
- `Pistas`
- `Notas`

### Busca inicial do seletor

Quando você clica em `Link`, o seletor tenta usar o texto selecionado como filtro inicial.

Se ele encontrar uma correspondência real no nome de um registro:

- abre já filtrado

Se não encontrar resultados reais:

- limpa o filtro inicial
- e mostra a lista completa

## Recursos do local

Cada local pode ter seus próprios recursos, divididos em:

- imagens
- mapas

No formulário você pode:

- adicionar imagens
- adicionar mapas
- escolher a capa do local
- remover a capa

Para cada recurso você pode configurar:

- nome exibido
- visibilidade para `Jogadores`
- visibilidade para `DM`
- texto de apresentação

## Área hero do local

Quando você seleciona um local, o painel direito mostra uma área hero com:

- a capa do local
- nome
- tipo (`Local` ou `Missão`)
- estado atual
- eventuais marcadores
- a cadeia hierárquica do local

Também aparece um resumo rápido com:

- `Presenças`
- `Sublocais`
- `Imagens`
- `Mapas`

## Abas de detalhe

O painel direito usa uma barra de foco com cinco seções principais:

- `Panorama`
- `Presenças`
- `Combates`
- `Mídia`
- `Notas`

### Panorama

A aba `Panorama` reúne:

- descrição DM
- descrição jogadores
- pistas
- tesouros
- mapas conceituais ligados ao local

### Presenças

A aba `Presenças` reúne os personagens presentes no local.

A partir daqui você pode:

- ver todas as presenças do local
- adicionar uma nova presença
- abrir o detalhe contextual dessa presença
- mudar seu papel no local
- ler ou editar `Notas DM`
- remover a presença

### Combates

A aba `Combates` mostra todos os confrontos ligados ao local.

A partir daqui você pode:

- criar um novo combate para o local
- reabrir um combate existente
- ver se ele ainda não começou, está em pausa ou foi concluído
- excluir um combate

### Mídia

A aba `Mídia` reúne:

- imagens do local
- mapas do local
- mapas herdados de locais pai, quando ativados

A partir daqui você pode:

- navegar pelas imagens
- navegar pelos mapas
- mostrá-los aos jogadores
- mostrá-los ao DM
- abrir diretamente um mapa interativo

### Notas

A aba `Notas` é dedicada às notas rápidas do DM para o local.

## Presenças do local

As presenças do local são gerenciadas de forma contextual e separada dos personagens de aventura e dos participantes de combate.

Isso permite manter:

- nomes exibidos contextuais
- papel no local
- notas DM locais
- estado local, quando necessário

## Duas origens possíveis para uma presença

Quando você adiciona uma presença a um local, o formulário pede a `Origem`.

As fontes possíveis são:

- `Personagem de aventura`
- `Ficha base`

### Personagem de aventura

Essa origem usa um personagem que já está ligado à aventura.

Nesse caso, a presença mantém o estado contextual da campanha.

### Ficha base

Essa origem clona um registro base do tipo:

- `NPC`
- `Monstro`

Registros do tipo `Herói` não podem ser selecionados nesse modo.

## Regras de unicidade das presenças

No painel de locais, o DnDino aplica regras bem claras:

- um `Personagem de aventura` só pode ser colocado uma vez no mesmo local
- um `NPC` base só pode ser adicionado uma vez no mesmo local
- um `Monstro` base pode ser adicionado várias vezes no mesmo local

Quando você adiciona várias instâncias do mesmo monstro, o nome exibido é numerado automaticamente, por exemplo:

- `Goblin`
- `Goblin 2`
- `Goblin 3`

## Dados da presença no local

No formulário da presença você pode definir:

- `Papel no encontro`
- `Nome exibido`
- `Condições`
- `Notas DM`

Se a presença vier de uma **ficha base** (`NPC` ou `Monstro`), você também terá um estado local do local, como:

- PV temporários
- PV atuais
- estado

Se a presença vier de um **Personagem de aventura**, o local continua referenciando esse estado contextual da campanha, em vez de duplicá-lo localmente da mesma forma.

## Papel no local

Cada presença tem um papel contextual:

- aliado
- neutro
- inimigo

Esse papel é importante tanto para ler a cena quanto para fluxos posteriores, como os combates.

## Combates ligados ao local

Os combates dentro dos locais são criados diretamente a partir do local selecionado.

Quando você cria um novo combate:

- o combate é salvo como encontro daquele local
- aparece imediatamente na aba `Combates`
- pode ser reaberto mais tarde

## Mídia do local

A área de mídia do local distingue claramente entre:

- imagens
- mapas

O painel também pode mostrar mapas herdados de locais pai por meio do seletor:

- `Mostrar mapas dos locais pai`

## Mapa interativo

Quando um mapa é escolhido como mapa interativo do local, você pode abri-lo diretamente a partir do painel.

O mapa interativo suporta:

- zoom
- deslocamento
- marcadores
- navegação entre locais

### Marcadores do mapa interativo

Cada marcador pode ter:

- uma posição no mapa
- um título
- um local de destino associado

Os marcadores podem ser:

- criados
- movidos
- renomeados
- associados a um local
- eliminados

Comportamento básico:

- clique simples: seleciona o marcador
- duplo clique: abre o local vinculado no painel direito

## Relação entre Locais, Mapas e Mapas interativos

Vale pensar nesses três elementos como camadas diferentes:

- o **local** é o contêiner narrativo e estrutural
- o **mapa** é um recurso visual ligado ao local
- o **mapa interativo** é um mapa escolhido como suporte navegável, enriquecido com marcadores

## Missões na seção Locais

As missões vivem na mesma seção que os locais, mas seguem um comportamento próprio.

Uma missão:

- aparece na árvore ao lado dos locais
- usa um estado de progressão em vez de um estado de visita
- ainda assim pode ter descrições, notas, imagens, mapas, presenças e links contextuais

## Quando usar a seção Locais

O painel `Locais` é o lugar certo quando você quer:

- construir a geografia da campanha
- definir sublocais e vínculos
- preparar missões e seu estado
- posicionar presenças no mundo
