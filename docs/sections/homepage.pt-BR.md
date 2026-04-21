# Página inicial

A **página inicial** é a tela de entrada do DnDino. Ela não é um painel operacional pensado para gerenciar diretamente todos os módulos do aplicativo, mas sim um **ponto de acesso rápido** criado para:

- retomar imediatamente a última aventura usada
- voltar rapidamente às ferramentas principais
- ajudar você a se orientar ao abrir o aplicativo

A página inicial tem, portanto, duas funções principais:

- **retomada rápida**, se você já tem uma campanha ativa
- **início guiado**, se está começando do zero

## Estrutura da tela

A Home é composta por três áreas principais:

1. cabeçalho de boas-vindas
2. painel principal dedicado à última aventura ou ao primeiro início
3. grade com as ferramentas principais do aplicativo

## Cabeçalho de boas-vindas

Na parte superior da tela aparece uma saudação inicial.

Se o nome do Mestre tiver sido definido nas configurações, a Home mostra uma mensagem personalizada, por exemplo:

- `Olá, Marcos!`

Caso contrário, aparece uma versão genérica:

- `Olá, DM!`

Logo abaixo há uma frase curta explicando o objetivo da tela: retomar o trabalho de onde ele parou ou abrir imediatamente uma das ferramentas principais.

## Painel principal

O painel principal muda de acordo com o estado do aplicativo.

### Se já existir uma aventura recente

Quando o aplicativo encontra uma aventura usada recentemente, a Home mostra um cartão grande dedicado à **última aventura**.

Esse cartão contém:

- o título da aventura
- uma breve descrição, se existir
- um botão `Abrir aventura`
- um possível botão para ir direto ao último lugar visitado
- algumas estatísticas de resumo
- uma seção visual com os heróis vinculados à aventura

Se a aventura tiver uma imagem de capa, essa imagem é usada como fundo do cartão. Caso contrário, o DnDino mostra um fundo gráfico padrão.

#### Botão Abrir aventura

O botão principal do cartão abre diretamente o **painel principal da aventura**, que é o centro operacional da campanha.

É a forma mais rápida de retomar o trabalho.

#### Botão Ir para o último lugar visitado

Se o aplicativo souber qual foi o último lugar aberto dentro da aventura, o cartão também mostra um segundo botão que leva você diretamente para esse lugar.

Isso é especialmente útil quando você quer retomar imediatamente a exploração ou continuar o trabalho em uma área narrativa específica da campanha.

## Estatísticas da aventura

No painel principal também aparecem algumas métricas de resumo da última aventura.

As estatísticas visíveis são:

- `Missões`
- `Lugares`
- `Sessões`
- `Combates`

Esses valores servem como um panorama rápido para entender quanto material já foi construído na campanha.

## Heróis da aventura

Se a aventura tiver heróis vinculados, a parte direita do cartão mostra uma seção dedicada a eles.

Essa área pode exibir:

- o número total de heróis
- retratos, se disponíveis
- uma mensagem sugerindo adicionar uma imagem de capa se eles ainda não tiverem uma

Quando existe apenas um herói, o retrato aparece em tamanho maior. Quando existem vários, os retratos são organizados em um conjunto mais compacto.

Essa seção tem uma função principalmente visual: ajuda você a reconhecer a campanha de imediato.

## Quando ainda não existe nenhuma aventura

Se o usuário ainda não tiver aventuras disponíveis, a Home mostra um painel alternativo pensado para acompanhar o primeiro uso.

Nesse caso a tela apresenta:

- o título `Pronto para começar`
- uma breve descrição introdutória
- o botão `Ir para aventuras`
- três passos sugeridos para começar a usar o DnDino

Os três passos exibidos são:

1. criar uma aventura
2. adicionar personagens
3. construir lugares e missões

Nesse estado, a Home funciona como onboarding e acompanha a criação da primeira campanha.

## Ferramentas principais

Abaixo do painel principal existe uma grade de cartões que representam as ferramentas principais do aplicativo.

As seções acessíveis a partir da Home são:

- `Aventuras`
- `Heróis, NPCs e Monstros`
- `Equipamentos`
- `Regras`
- `Gerador de nomes`
- `Configurações`

Cada cartão contém:

- título
- um breve subtítulo descritivo
- ícone
- fundo ilustrado dedicado

### Aventuras

Abre a lista de campanhas e permite:

- criar uma nova aventura
- abrir uma campanha existente
- retomar o trabalho de preparação

### Heróis, NPCs e Monstros

Abre a seção que reúne as fichas das criaturas. A partir daqui você pode trabalhar com:

- heróis
- NPCs
- monstros
- dados base vinculados às fichas

!!! tip
    Com o tempo você vai perceber que muitos personagens também podem ser abertos e editados diretamente de dentro da aventura, sem quebrar seu fluxo de preparação.

### Equipamentos

Abre a seção dedicada a:

- armas
- armaduras
- ferramentas
- equipamentos

### Regras

Abre a área de consulta rápida de regras e referências. Ela é útil para:

- consultar material de apoio
- buscar regras
- abrir conteúdos relacionados ao jogo

### Gerador de nomes

Abre a ferramenta para gerar rapidamente nomes úteis durante a preparação ou a improvisação, por exemplo para:

- NPCs
- monstros
- encontros inesperados

!!! tip
    Durante a sessão, o mini gerador de nomes da barra superior costuma ser ainda mais prático, porque permite criar nomes sem sair da tela em que você está trabalhando.

### Configurações

Abre o painel de preferências globais do aplicativo e de gerenciamento local do banco de dados.

## Quando usar a Home

A Home é especialmente útil quando você quer:

- retomar rapidamente a última campanha
- abrir o painel principal da aventura mais recente
- voltar ao último lugar visitado
- acessar rapidamente as principais ferramentas do aplicativo
- começar uma nova campanha se o banco de dados ainda estiver vazio

!!! tip
    Se você trabalha quase sempre na mesma campanha, o cartão da última aventura é a forma mais rápida de voltar ao lugar certo sem passar toda vez pela lista completa de aventuras.
