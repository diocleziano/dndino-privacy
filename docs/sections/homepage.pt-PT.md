# Página inicial

A **página inicial** é o ecrã de entrada do DnDino. Não é um painel operativo pensado para gerir diretamente todos os módulos da aplicação, mas sim um **ponto de acesso rápido** criado para:

- retomar de imediato a última aventura usada
- voltar rapidamente às ferramentas principais
- ajudar-te a orientar quando abres a aplicação

A página inicial tem, por isso, duas funções principais:

- **retoma rápida**, se já tens uma campanha ativa
- **arranque guiado**, se estás a começar do zero

## Estrutura do ecrã

A Home é composta por três áreas principais:

1. cabeçalho de boas-vindas
2. painel principal dedicado à última aventura ou ao arranque inicial
3. grelha com as ferramentas principais da aplicação

## Cabeçalho de boas-vindas

Na parte superior do ecrã aparece uma saudação inicial.

Se o nome do Mestre tiver sido definido nas definições, a Home mostra uma mensagem personalizada, por exemplo:

- `Olá, Marco!`

Caso contrário, surge uma versão genérica:

- `Olá, DM!`

Por baixo da saudação há uma pequena frase que explica o objetivo do ecrã: retomar o trabalho onde ficou ou abrir de imediato uma das ferramentas principais.

## Painel principal

O painel principal muda conforme o estado da aplicação.

### Se já existir uma aventura recente

Quando a aplicação encontra uma aventura usada recentemente, a Home mostra um cartão grande dedicado à **última aventura**.

Este cartão contém:

- o título da aventura
- uma breve descrição, se existir
- um botão `Abrir aventura`
- um eventual botão para ir diretamente ao último local visitado
- algumas estatísticas de resumo
- uma secção visual com os heróis associados à aventura

Se a aventura tiver uma imagem de capa, essa imagem é usada como fundo do cartão. Caso contrário, o DnDino mostra um fundo gráfico predefinido.

#### Botão Abrir aventura

O botão principal do cartão abre diretamente a **dashboard da aventura**, que é o centro operativo da campanha.

É a forma mais rápida de retomar o trabalho.

#### Botão Ir para o último local visitado

Se a aplicação souber qual foi o último local aberto dentro da aventura, o cartão mostra também um segundo botão que te leva diretamente para esse local.

Isto é especialmente útil quando queres retomar logo a exploração ou continuar o trabalho numa zona narrativa específica da campanha.

## Estatísticas da aventura

No painel principal também são mostradas algumas métricas de resumo da última aventura.

As estatísticas visíveis são:

- `Missões`
- `Locais`
- `Sessões`
- `Combates`

Estes valores servem apenas como visão rápida para perceber quanto material já foi construído na campanha.

## Heróis da aventura

Se a aventura tiver heróis associados, a parte direita do cartão mostra uma secção dedicada a eles.

Esta área pode mostrar:

- o número total de heróis
- retratos, se existirem
- uma mensagem a sugerir que adiciones uma capa aos heróis, caso ainda não tenham imagem

Quando existe apenas um herói, o retrato aparece em tamanho maior. Quando existem vários, os retratos são apresentados num conjunto mais compacto.

Esta secção tem sobretudo uma função visual: ajuda-te a reconhecer a campanha num relance.

## Quando ainda não existe nenhuma aventura

Se o utilizador ainda não tiver aventuras disponíveis, a Home mostra um painel alternativo pensado para acompanhar o primeiro arranque.

Neste caso o ecrã apresenta:

- o título `Pronto para começar`
- uma breve descrição introdutória
- o botão `Ir para aventuras`
- três passos sugeridos para começar a usar o DnDino

Os três passos mostrados são:

1. criar uma aventura
2. adicionar personagens
3. construir locais e missões

Neste estado, a Home funciona como onboarding e acompanha a criação da primeira campanha.

## Ferramentas principais

Debaixo do painel principal existe uma grelha de cartões que representam as ferramentas principais da aplicação.

As secções acessíveis a partir da Home são:

- `Aventuras`
- `Heróis, NPC e Monstros`
- `Equipamento`
- `Regras`
- `Gerador de nomes`
- `Definições`

Cada cartão contém:

- título
- breve subtítulo descritivo
- ícone
- fundo ilustrado dedicado

### Aventuras

Abre a lista de campanhas e permite:

- criar uma nova aventura
- abrir uma campanha existente
- retomar o trabalho de preparação

### Heróis, NPC e Monstros

Abre a secção que reúne as fichas das criaturas. A partir daqui podes trabalhar com:

- heróis
- NPC
- monstros
- dados base associados às fichas

!!! tip
    Com o tempo vais notar que muitas personagens também podem ser abertas e editadas diretamente a partir de dentro da aventura, sem quebrar o teu fluxo de preparação.

### Equipamento

Abre a secção dedicada a:

- armas
- armaduras
- ferramentas
- equipamento

### Regras

Abre a área de consulta rápida das regras e referências. É útil para:

- consultar material de apoio
- procurar regras
- abrir conteúdos relacionados com o jogo

### Gerador de nomes

Abre a ferramenta para gerar rapidamente nomes úteis durante a preparação ou improvisação, por exemplo para:

- NPC
- monstros
- encontros inesperados

!!! tip
    Durante a sessão, o mini gerador de nomes da topbar costuma ser ainda mais prático, porque te permite gerar nomes sem sair do ecrã onde estás a trabalhar.

### Definições

Abre o painel das preferências globais da aplicação e da gestão local da base de dados.

## Quando usar a Home

A Home é especialmente útil quando queres:

- retomar rapidamente a última campanha
- abrir a dashboard da aventura mais recente
- voltar ao último local visitado
- aceder rapidamente às principais ferramentas da aplicação
- começar uma nova campanha se a base de dados ainda estiver vazia

!!! tip
    Se trabalhas quase sempre na mesma campanha, o cartão da última aventura é a forma mais rápida de regressar ao sítio certo sem teres de passar sempre pela lista completa de aventuras.
