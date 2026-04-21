# Heróis, NPC e Monstros

A secção **Heróis, NPC e Monstros** reúne todas as fichas base das personagens da aplicação. É o ponto onde se criam, modificam e clonam os registos que depois podem ser ligados a aventuras, locais e combates.

Esta página é importante porque, no DnDino, existem **vários níveis de personagem**, cada um com um objetivo diferente:

- a **ficha base**
- a **personagem de aventura**
- a **presença no local**
- o **participante no combate**

Não são duplicações inúteis: servem para manter **dados contextuais separados**, como nome apresentado, pontos de vida, condições, iniciativa e notas do Mestre, sem perder a ligação à ficha original.

## Ficha base

A **ficha base** é o registo principal guardado na secção `Heróis, NPC e Monstros`.

Aqui defines tudo o que pertence à personagem de forma geral:

- nome
- tipo: `Herói`, `NPC` ou `Monstro`
- raça, classe, tamanho, alinhamento
- atributos
- CA, PV máximos, velocidade, iniciativa
- descrição, habilidades e ataques
- imagens associadas
- feitiços associados
- equipamento e outros dados de referência

A ficha base não representa automaticamente uma personagem “presente” numa aventura, num local ou num combate. É o modelo de onde nascem os níveis seguintes.

## Criar, modificar e clonar uma personagem

Para criar uma nova ficha:

1. abre `Heróis, NPC e Monstros`
2. prime o botão de adicionar
3. preenche o formulário da personagem
4. guarda o registo

Podes criar:

- heróis
- NPC
- monstros

O tipo escolhido influencia campos e comportamentos nas secções seguintes. Por exemplo:

- para os **heróis**, faz sentido falar de presença na aventura, inspiração e estado contextual
- para os **monstros**, ganham mais importância o ND, os ataques e o uso múltiplo em contextos operacionais

Ao abrir uma ficha existente, podes modificar o registo base em todos os aspetos. As alterações feitas aqui atualizam o registo de origem, mas nem sempre substituem automaticamente todos os registos contextuais já criados em aventura, locais ou combate. Isto é intencional.

A **clonagem** cria uma nova ficha base a partir de uma já existente, copiando também elementos associados como:

- campos da ficha
- feitiços associados
- ataques estruturados
- imagens associadas

É especialmente útil quando queres:

- criar variantes semelhantes do mesmo monstro
- partir de um NPC já preparado
- construir rapidamente várias fichas com estrutura parecida

## Links internos nos textos da personagem

Uma das funções mais úteis da ficha base, sobretudo para **NPC** e **Monstros**, é o sistema de **links internos** nos campos rich text.

Esta função é especialmente valiosa na secção **Ataques**, porque transforma texto descritivo em ferramentas operacionais prontas a usar durante a sessão e no combate.

Na prática, podes inserir links que abrem diretamente:

- um lançamento de dados
- um ataque
- um ataque completo com dano
- uma personagem
- um local
- um feitiço
- um talento
- uma regra do glossário

## Onde faz mais sentido usá-los

Os links internos são particularmente úteis em campos rich text como:

- `Ataques`
- `Habilidades especiais`
- `Descrição`
- outros campos descritivos com referências rápidas

O caso mais útil continua a ser **Ataques**, porque te permite tornar imediatamente clicáveis:

- o ataque
- os dados de dano
- um ataque completo já preparado

Para monstros, isto é muito cómodo, porque reduz o tempo gasto a reler fórmulas ou a reconstruir lançamentos manualmente.

## Como inserir um link

O fluxo correto é este:

1. abre um campo rich text da ficha
2. seleciona o texto que queres transformar em link, ou posiciona o cursor no sítio pretendido
3. prime o botão `Link`
4. escolhe o tipo de ligação no seletor
5. confirma a criação

Consoante o texto selecionado, o seletor pode já propor alguns links automáticos prontos a usar.

## Os quatro links mais úteis para lançamentos

### Lançamento livre

`Lançamento livre` é o link mais flexível. Está sempre disponível no seletor e serve quando queres criar um lançamento configurável sem seguir uma estrutura rígida.

É útil para:

- uma fórmula completa como `1d6+3`
- um dado simples como `1d20`
- uma fórmula que ainda queres ajustar antes do lançamento

### Lançar dados

`Lançar dados` só aparece se o texto selecionado for uma **fórmula de dados válida**.

Exemplos válidos:

- `1d6`
- `2d8+4`
- `4d4 + 1`

Este link é ideal para dano simples, dados de cura, efeitos aleatórios e lançamentos rápidos separados.

### Ataque

`Ataque` só aparece se o texto selecionado for um **modificador válido**, e não uma fórmula completa `1d20`.

Exemplos válidos:

- `+5`
- `-1`
- `0`
- `2`

Quando crias este link, o DnDino sabe que deve fazer um **1d20** usando esse modificador. É perfeito para linhas legíveis como:

- `Mordida +6`
- `Garras +4`

### Ataque e dano

`Ataque e dano` é o link mais poderoso para a secção **Ataques**.

Está sempre disponível no seletor e abre um configurador dedicado onde podes definir:

- modificador do ataque
- eventual margem de crítico
- até três fórmulas de dano
- título de cada componente

É a melhor forma de construir um ataque completo de monstro ou NPC, porque um único link pode concentrar:

- o ataque
- o dano principal
- danos secundários
- dano adicional

No combate, este link é particularmente útil porque o popover associado também pode ser usado para aplicar dano aos alvos escolhidos.

## Exemplo prático para Ataques

Uma forma muito eficaz de escrever um ataque de monstro é manter o texto legível para o Mestre e tornar clicáveis apenas os pontos úteis.

Por exemplo:

- `Mordida +6, alcance 1,5 m, um alvo. Acerto: 1d8+4 perfurante.`

Depois podes transformar:

- `+6` em `Ataque`
- `1d8+4` em `Lançar dados`

ou criar diretamente um único link `Ataque e dano` sobre o nome do ataque ou parte da linha.

## Ligar locais, personagens e outras referências

O sistema de links não serve apenas para lançamentos.

Nos campos descritivos também podes criar ligações para outros conteúdos da aplicação, como:

- um `Local`
- outra `Personagem`
- um `Feitiço`
- um `Talento`
- uma `Regra`

Quando prime `Link`, o seletor também tenta usar o texto selecionado como filtro inicial:

- se encontrar uma correspondência real no nome dos registos, abre já filtrado
- se não encontrar resultados reais, limpa o filtro inicial e mostra a lista completa

## Personagens de aventura

A **personagem de aventura** é o nível que liga uma ficha base a uma campanha específica.

Este registo serve para gerir valores que só fazem sentido **dentro de uma aventura**, por exemplo:

- pontos de vida atuais
- pontos de vida temporários
- condições
- estado
- inspiração heroica

Por outras palavras:

- a ficha base diz **quem é** a personagem
- a personagem de aventura diz **como está** essa personagem dentro de determinada campanha

## Presenças nos locais

A **presença no local** é outro registo distinto. Serve para dizer que uma personagem ou criatura está presente num local específico, com nome e eventualmente estado locais.

No formulário `Adicionar presença ao local` existem duas origens possíveis:

- `Personagem de aventura`
- `NPC / Monstro`

### Presença a partir de Personagem de aventura

Se escolheres `Personagem de aventura`, o registo do local fica ligado a uma personagem já presente na campanha.

Nesse caso:

- a presença mantém a ligação à personagem de aventura
- não cria uma cópia autónoma da personagem
- não podes adicionar a mesma personagem de aventura mais do que uma vez ao mesmo local

### Presença a partir de NPC / Monstro

Se escolheres `NPC / Monstro`, o local cria uma **presença local clonada** a partir de uma ficha base do tipo `NPC` ou `Monstro`.

Este registo tem dados próprios para o local, como:

- nome apresentado
- PV atuais
- PV temporários
- condições
- estado
- disposição
- notas do Mestre

Neste caso, o comportamento depende do tipo:

- os **Monstros** podem ter várias presenças locais no mesmo local
- os **NPC** permanecem únicos no mesmo local e não voltam a ser propostos no seletor

Quando adicionas várias instâncias do mesmo monstro, o DnDino propõe automaticamente um nome incremental, por exemplo:

- `Goblin 2`

## Porque existe o nome apresentado

Tanto as presenças dos locais como os participantes no combate têm um campo `Nome apresentado`.

Este campo serve para manter um nome **contextual** sem renomear a ficha base. É útil, por exemplo, quando queres:

- distinguir cópias semelhantes da mesma criatura
- dar um nome específico a um NPC apenas num local
- usar um nome diferente no combate sem alterar o registo de origem

## Participantes no combate

O **participante no combate** é o nível operacional usado durante o confronto.

Um participante pode nascer de três fontes diferentes:

- uma **personagem de aventura**
- uma **presença do local**
- uma **ficha base**

Cada participante no combate tem o seu próprio registo específico do confronto, com dados como:

- nome apresentado
- iniciativa
- CA
- PV máximos
- PV atuais
- PV temporários
- condições
- estado
- testes de salvamento contra a morte
- ordem no round

### Participantes a partir de personagens de aventura

Se o participante nasce de uma personagem de aventura:

- mantém-se ligado à personagem da campanha
- no final do combate, os valores finais são sincronizados novamente com o registo da aventura

### Participantes a partir de presenças do local

Se o participante nasce de uma presença do local:

- mantém-se ligado a esse registo do local
- se essa presença usar estado local, o combate pode sincronizar novamente PV, condições e estado com o registo do local

### Participantes a partir de fichas base

Se o participante nasce diretamente de uma ficha base:

- o registo de combate usa essa ficha como origem
- o comportamento em relação a instâncias múltiplas depende do tipo

No seletor de combate:

- um registo base do tipo **Monstro** pode ser adicionado mais do que uma vez
- um registo base do tipo **NPC** ou **Herói** não volta a ser proposto no mesmo combate

## Sincronização entre níveis

Alguns valores são sincronizados entre níveis, mas nem tudo é sempre substituído.

### Da ficha base para os contextos

A ficha base fornece:

- identidade da personagem
- estatísticas de referência
- feitiços
- ataques
- imagens

### Dos contextos para os registos ligados

Os níveis operacionais podem sincronizar dados situacionais, sobretudo:

- PV
- condições
- estado
- algumas notas locais

No combate, por exemplo, os valores finais podem voltar para:

- a personagem de aventura ligada
- a presença do local ligada, se essa presença usar estado local

## Diferença prática entre os níveis

Para decorar melhor a lógica, podes lê-la assim:

- `Ficha base`: o **modelo geral** da personagem
- `Personagem de aventura`: o **estado da personagem dentro da campanha**
- `Presença no local`: a **presença contextual da personagem num local específico**
- `Participante no combate`: a **versão operacional da personagem no confronto**

## Quando convém usar cada nível

### Usa a ficha base quando:

- precisas de criar a personagem
- queres modificar dados estruturais
- precisas de ligar imagens, feitiços ou ataques

### Usa a personagem de aventura quando:

- queres ligar um herói à campanha
- precisas de acompanhar de forma persistente PV, estado, condições e inspiração na aventura

### Usa a presença no local quando:

- queres povoar um local com personagens ou criaturas
- queres dar nomes contextuais a NPC e monstros
- queres criar instâncias locais separadas dentro de um local

### Usa o participante no combate quando:

- estás a preparar ou gerir um confronto
- precisas de iniciativa, PV e condições de batalha
- queres que o combate trabalhe sobre registos contextuais sem mexer diretamente na ficha base

## Em resumo

A secção `Heróis, NPC e Monstros` não é apenas um arquivo de fichas. É o **nível de origem** a partir do qual nasce toda a gestão contextual das personagens dentro da aplicação.

A lógica geral é esta:

- a **ficha base** define a personagem
- a **personagem de aventura** insere-a na campanha
- a **presença no local** contextualiza-a num local
- o **participante no combate** torna-a operacional no confronto

!!! tip
    Se quiseres evitar confusão, lembra-te sempre desta distinção: a ficha base descreve a personagem, enquanto aventura, local e combate descrevem o seu estado num contexto específico. Não precisas de te fixar demasiado na separação teórica; o importante é perceber que alguns campos só existem no seu próprio contexto.
