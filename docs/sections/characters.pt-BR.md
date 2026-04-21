# Heróis, NPCs e Monstros

A seção **Heróis, NPCs e Monstros** reúne todas as fichas base dos personagens do aplicativo. É o lugar em que você cria, edita e clona os registros que depois podem ser vinculados a aventuras, lugares e combates.

Esta página é importante porque, no DnDino, existem **vários níveis de personagem**, cada um com um propósito diferente:

- a **ficha base**
- o **personagem de aventura**
- a **presença no lugar**
- o **participante de combate**

Não são duplicações inúteis: eles existem para manter **dados contextuais separados**, como nome exibido, pontos de vida, condições, iniciativa e notas do Mestre, sem perder a ligação com a ficha original.

## Ficha base

A **ficha base** é o registro principal salvo na seção `Heróis, NPCs e Monstros`.

Aqui você define tudo o que pertence ao personagem de forma geral:

- nome
- tipo: `Herói`, `NPC` ou `Monstro`
- raça, classe, tamanho, alinhamento
- atributos
- CA, PV máximos, velocidade, iniciativa
- descrição, habilidades e ataques
- imagens vinculadas
- magias vinculadas
- equipamento e outros dados de referência

A ficha base não representa automaticamente um personagem “presente” em uma aventura, em um lugar ou em um combate. Ela é o modelo de onde nascem os níveis seguintes.

## Criar, editar e clonar um personagem

Para criar uma nova ficha:

1. abra `Heróis, NPCs e Monstros`
2. pressione o botão de adicionar
3. preencha o formulário do personagem
4. salve o registro

Você pode criar:

- heróis
- NPCs
- monstros

O tipo escolhido influencia campos e comportamentos nas seções seguintes. Por exemplo:

- para os **heróis**, faz sentido falar de presença na aventura, inspiração e estado contextual
- para os **monstros**, ganham mais importância o ND, os ataques e o uso múltiplo em contextos operacionais

Ao abrir uma ficha existente, você pode editar o registro base em todos os detalhes. As mudanças feitas aqui atualizam o registro de origem, mas nem sempre sobrescrevem automaticamente todos os registros contextuais já criados em aventura, lugares ou combate. Isso é intencional.

A **clonagem** cria uma nova ficha base a partir de uma já existente, copiando também elementos vinculados como:

- campos da ficha
- magias vinculadas
- ataques estruturados
- imagens vinculadas

Ela é especialmente útil quando você quer:

- criar variantes parecidas do mesmo monstro
- partir de um NPC já preparado
- construir rapidamente várias fichas com estrutura semelhante

## Links internos nos textos do personagem

Uma das funções mais úteis da ficha base, especialmente para **NPCs** e **Monstros**, é o sistema de **links internos** nos campos rich text.

Essa função é especialmente valiosa na seção **Ataques**, porque transforma texto descritivo em ferramentas operacionais prontas para uso durante a sessão e no combate.

Na prática, você pode inserir links que abrem diretamente:

- uma rolagem de dados
- uma jogada de ataque
- um ataque completo com dano
- um personagem
- um lugar
- uma magia
- um talento
- uma regra do glossário

## Onde vale mais a pena usá-los

Os links internos são especialmente úteis em campos rich text como:

- `Ataques`
- `Habilidades especiais`
- `Descrição`
- outros campos descritivos em que você queira referências rápidas

O caso mais útil continua sendo **Ataques**, porque ele permite tornar imediatamente clicáveis:

- a jogada para atingir
- os dados de dano
- um ataque completo já preparado

Para monstros, isso é muito prático, porque reduz o tempo gasto lendo fórmulas ou reconstruindo jogadas manualmente.

## Como inserir um link

O fluxo correto é este:

1. abra um campo rich text da ficha
2. selecione o texto que quer transformar em link, ou posicione o cursor no lugar desejado
3. pressione o botão `Link`
4. escolha o tipo de ligação no seletor
5. confirme a criação

Dependendo do texto selecionado, o seletor pode já sugerir alguns links automáticos prontos para uso.

## Os quatro links mais úteis para rolagens

### Rolagem livre

`Rolagem livre` é o link mais flexível. Ele está sempre disponível no seletor e serve quando você quer criar uma rolagem configurável sem seguir uma estrutura rígida.

É útil para:

- uma fórmula completa como `1d6+3`
- um dado simples como `1d20`
- uma fórmula que você ainda queira ajustar antes de rolar

### Rolar dados

`Rolar dados` só aparece se o texto selecionado for uma **fórmula de dados válida**.

Exemplos válidos:

- `1d6`
- `2d8+4`
- `4d4 + 1`

Esse link é ideal para dano simples, dados de cura, efeitos aleatórios e rolagens rápidas separadas.

### Jogada de ataque

`Jogada de ataque` só aparece se o texto selecionado for um **modificador válido**, e não uma fórmula completa `1d20`.

Exemplos válidos:

- `+5`
- `-1`
- `0`
- `2`

Quando você cria esse link, o DnDino sabe que deve fazer um **1d20** com esse modificador. Ele é perfeito para linhas legíveis como:

- `Mordida +6`
- `Garras +4`

### Jogada de ataque e dano

`Jogada de ataque e dano` é o link mais poderoso para a seção **Ataques**.

Ele está sempre disponível no seletor e abre um configurador dedicado em que você pode definir:

- modificador da jogada de ataque
- eventual margem de crítico
- até três fórmulas de dano
- título de cada componente

É a melhor forma de construir um ataque completo de monstro ou NPC, porque um único link pode concentrar:

- a jogada de ataque
- o dano principal
- danos secundários
- dano adicional

No combate, esse link é particularmente útil porque o popover associado também pode ser usado para aplicar dano aos alvos escolhidos.

## Exemplo prático para Ataques

Uma forma muito eficiente de escrever um ataque de monstro é manter o texto legível para o Mestre e tornar clicáveis apenas os pontos realmente úteis.

Por exemplo:

- `Mordida +6, alcance 1,5 m, um alvo. Acerto: 1d8+4 perfurante.`

Depois você pode transformar:

- `+6` em `Jogada de ataque`
- `1d8+4` em `Rolar dados`

ou criar diretamente um único link `Jogada de ataque e dano` sobre o nome do ataque ou parte da linha.

## Vincular lugares, personagens e outras referências

O sistema de links não serve apenas para rolagens.

Nos campos descritivos você também pode criar ligações para outros conteúdos do aplicativo, como:

- um `Lugar`
- outro `Personagem`
- uma `Magia`
- um `Talento`
- uma `Regra`

Quando você pressiona `Link`, o seletor também tenta usar o texto selecionado como filtro inicial:

- se encontrar uma correspondência real no nome dos registros, ele já abre filtrado
- se não encontrar resultados reais, limpa o filtro inicial e mostra a lista completa

## Personagens de aventura

O **personagem de aventura** é o nível que liga uma ficha base a uma campanha específica.

Esse registro serve para gerenciar valores que só fazem sentido **dentro de uma aventura**, por exemplo:

- pontos de vida atuais
- pontos de vida temporários
- condições
- estado
- inspiração heroica

Em outras palavras:

- a ficha base diz **quem é** o personagem
- o personagem de aventura diz **como ele está** dentro daquela campanha

## Presenças nos lugares

A **presença no lugar** é outro registro diferente. Ela serve para dizer que um personagem ou criatura está presente em um lugar específico, com um nome e, se necessário, um estado local.

No formulário `Adicionar presença ao lugar` existem duas origens possíveis:

- `Personagem de aventura`
- `NPC / Monstro`

### Presença a partir de personagem de aventura

Se você escolher `Personagem de aventura`, o registro do lugar fica vinculado a um personagem já presente na campanha.

Nesse caso:

- a presença mantém o vínculo com o personagem de aventura
- não cria uma cópia autônoma do personagem
- no mesmo lugar você não pode adicionar o mesmo personagem de aventura mais de uma vez

### Presença a partir de NPC / Monstro

Se você escolher `NPC / Monstro`, o lugar cria uma **presença local clonada** a partir de uma ficha base do tipo `NPC` ou `Monstro`.

Esse registro passa a ter dados próprios para o lugar, como:

- nome exibido
- PV atuais
- PV temporários
- condições
- estado
- disposição
- notas do Mestre

Aqui o comportamento depende do tipo:

- os **Monstros** podem ter várias presenças locais no mesmo lugar
- os **NPCs** permanecem únicos dentro do mesmo lugar e não são oferecidos novamente no seletor

Quando você adiciona várias instâncias do mesmo monstro, o DnDino propõe automaticamente um nome incremental, por exemplo:

- `Goblin 2`

## Por que existe o nome exibido

Tanto as presenças dos lugares quanto os participantes de combate têm um campo `Nome exibido`.

Esse campo serve para manter um nome **contextual** sem renomear a ficha base. Ele é útil, por exemplo, quando você quer:

- distinguir cópias semelhantes da mesma criatura
- dar a um NPC um nome específico em um único lugar
- usar um nome diferente no combate sem alterar o registro de origem

## Participantes de combate

O **participante de combate** é o nível operacional usado durante o confronto.

Um participante pode nascer de três fontes diferentes:

- um **personagem de aventura**
- uma **presença do lugar**
- uma **ficha base**

Cada participante de combate tem seu próprio registro específico do confronto, com dados como:

- nome exibido
- iniciativa
- CA
- PV máximos
- PV atuais
- PV temporários
- condições
- estado
- testes de resistência contra a morte
- ordem na rodada

### Participantes a partir de personagens de aventura

Se o participante nasce de um personagem de aventura:

- continua vinculado ao personagem da campanha
- no fim do combate, os valores finais são sincronizados novamente com o registro da aventura

### Participantes a partir de presenças do lugar

Se o participante nasce de uma presença do lugar:

- continua vinculado a esse registro do lugar
- se essa presença usar estado local, o combate pode sincronizar novamente PV, condições e estado com o registro do lugar

### Participantes a partir de fichas base

Se o participante nasce diretamente de uma ficha base:

- o registro de combate usa essa ficha como origem
- o comportamento quanto a instâncias múltiplas depende do tipo

No seletor de combate:

- um registro base do tipo **Monstro** pode ser adicionado mais de uma vez
- um registro base do tipo **NPC** ou **Herói** não volta a ser oferecido dentro do mesmo combate

## Sincronização entre os níveis

Alguns valores são sincronizados entre níveis, mas nem tudo é sempre sobrescrito.

### Da ficha base para os contextos

A ficha base fornece:

- identidade do personagem
- estatísticas de referência
- magias
- ataques
- imagens

### Dos contextos para os registros vinculados

As camadas operacionais podem sincronizar dados situacionais, principalmente:

- PV
- condições
- estado
- algumas notas locais

No combate, por exemplo, os valores finais podem voltar para:

- o personagem de aventura vinculado
- a presença do lugar vinculada, se essa presença usar estado local

## Diferença prática entre os níveis

Uma forma simples de lembrar a lógica é esta:

- `Ficha base`: o **modelo geral** do personagem
- `Personagem de aventura`: o **estado do personagem dentro da campanha**
- `Presença no lugar`: a **presença contextual do personagem em um lugar específico**
- `Participante de combate`: a **versão operacional do personagem dentro do confronto**

## Quando vale a pena usar cada nível

### Use a ficha base quando:

- precisar criar o personagem
- quiser modificar dados estruturais
- precisar vincular imagens, magias ou ataques

### Use o personagem de aventura quando:

- quiser vincular um herói à campanha
- precisar acompanhar de forma persistente PV, estado, condições e inspiração dentro da aventura

### Use a presença no lugar quando:

- quiser povoar um lugar com personagens ou criaturas
- quiser dar nomes contextuais a NPCs e monstros
- quiser criar instâncias locais separadas dentro de um lugar

### Use o participante de combate quando:

- estiver preparando ou conduzindo um confronto
- precisar de iniciativa, PV e condições de batalha
- quiser que o combate trabalhe sobre registros contextuais sem alterar diretamente a ficha base

## Em resumo

A seção `Heróis, NPCs e Monstros` não é apenas um arquivo de fichas. Ela é o **nível de origem** a partir do qual nasce toda a gestão contextual dos personagens dentro do aplicativo.

A lógica geral é esta:

- a **ficha base** define o personagem
- o **personagem de aventura** o insere na campanha
- a **presença no lugar** o contextualiza em um lugar
- o **participante de combate** o torna operacional no confronto

!!! tip
    Se você quiser evitar confusão, lembre-se sempre desta distinção: a ficha base descreve o personagem, enquanto aventura, lugar e combate descrevem o seu estado em um contexto específico. Não é preciso se prender demais à separação teórica; o importante é entender que alguns campos só existem dentro do seu próprio contexto.
