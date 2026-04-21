# Combate

O modo **Combate** de DnDino foi pensado para ser o principal tracker operativo de um confronto. Esta página descreve o modo de combate padrão do DnDino.

O combate nasce sempre no contexto de um **local** e leva consigo as personagens, as presenças locais e os eventuais monstros ou PNJ ligados a essa cena.

Esta página explica todo o fluxo:

- preparação do pré-combate
- gestão dos participantes
- início do confronto
- utilização do painel do turno atual
- aplicação de dano, cura, condições e testes de resistência
- integração com a **Janela dos Jogadores**
- fecho do confronto e resumo final

## Utilização com um ou dois ecrãs

O combate do DnDino funciona muito bem também em **ecrã único**: toda a parte operacional fica no painel principal e podes gerir participantes, turnos, dano, condições e o resumo final sem precisares de um segundo monitor.

Dito isto, se tiveres uma configuração com dois ecrãs, podes usar:

- um ecrã principal para o painel de controlo do DM
- um segundo ecrã ou monitor para a **Janela dos Jogadores**

Nesta configuração o fluxo torna-se ainda mais confortável:

- no ecrã do DM ficam visíveis a lista de participantes, os controlos do round, o turno atual, os textos de ataque, as notas DM e as edições rápidas
- no ecrã dos jogadores é mostrada uma apresentação limpa do participante ativo, com imagem e overlay contextual

Na prática:

- em ecrã único usas todo o combate a partir do ecrã principal
- com dois ecrãs separas o painel técnico do DM da apresentação para os jogadores

!!! tip
    O segundo ecrã não é obrigatório. É simplesmente um reforço muito útil quando queres mostrar aos jogadores imagens e informação do turno atual sem expor o painel técnico do DM.

## Como funciona a Janela dos Jogadores durante o combate

Quando o combate é iniciado, o DnDino pode abrir ou atualizar automaticamente a **Janela dos Jogadores**.

Se a apresentação aos jogadores estiver ativa:

- no início do combate pode aparecer uma breve **intro** com os participantes
- durante o combate a janela atualiza-se para o **participante do turno atual**
- no fim do confronto pode aparecer um **resumo final**

Durante o combate, a Janela dos Jogadores não mostra o painel técnico do DM, mas uma apresentação visual com:

- imagem do participante ativo
- nome mostrado aos jogadores
- informação de overlay, se estiver ativada

O overlay pode incluir:

- round atual
- PV atuais, máximos e temporários
- condições
- próximo turno

Algumas informações sobre inimigos podem ser tratadas de forma separada da informação dos heróis.

## Definições da Janela dos Jogadores e do segundo ecrã

As opções mais importantes encontram-se em **Definições**, na área dedicada à apresentação do combate e da janela dos jogadores.

### Abertura e comportamento geral

As principais definições são:

- `Abrir janela dos jogadores mesmo com um só monitor`
- `Mostrar controlos da janela dos jogadores na topbar`
- `Mostrar intro de combate aos jogadores`
- `Mostrar resumo final aos jogadores`

#### Abrir janela dos jogadores mesmo com um só monitor

Se esta opção estiver ativa, o DnDino pode abrir automaticamente a Janela dos Jogadores mesmo quando trabalhas com apenas um monitor.

Se estiver desativada:

- com um só monitor a janela não se abre automaticamente
- se já estiver aberta, continua na mesma a atualizar-se

#### Mostrar controlos da janela dos jogadores na topbar

Se ativares esta opção, aparecem botões na barra superior para:

- abrir manualmente a janela dos jogadores
- fechá-la manualmente

#### Mostrar intro de combate aos jogadores

Quando carregas em `Iniciar confronto`, a Janela dos Jogadores pode mostrar uma curta introdução com:

- título do confronto
- participantes envolvidos
- número de participantes

Se desativares esta opção, o combate passa diretamente para a apresentação do primeiro participante ativo.

#### Mostrar resumo final aos jogadores

Quando o combate termina, a Janela dos Jogadores pode mostrar um resumo final.

O resumo destinado aos jogadores mostra apenas informação útil para eles, como:

- dano causado pelos heróis
- dano sofrido pelos heróis
- imagem do pior inimigo

O resumo final dos jogadores mantém-se visível até mudares o conteúdo da janela ou a fechares.

### Informação mostrada durante o turno

As definições que controlam o overlay do participante ativo são:

- `Mostrar round na janela dos jogadores`
- `Mostrar PV na janela dos jogadores`
- `Mostrar condições na janela dos jogadores`
- `Mostrar próximo turno na janela dos jogadores`

### Informação sobre inimigos, monstros e PNJ

Para participantes que não são heróis existem controlos dedicados:

- `Mostrar detalhes de PNJ e monstros aos jogadores`
- `Mostrar condições dos inimigos aos jogadores`
- `Mostrar nomes dos inimigos aos jogadores`

Isto permite decidir se a Janela dos Jogadores deve:

- mostrar a criatura de forma mais evocativa
- ou mostrar também dados mais técnicos

## Onde o combate se abre

O combate é criado a partir do contexto de um **local**. Depois de aberto, o DnDino mostra um ecrã dividido em duas colunas principais:

- à esquerda, o tracker operativo do combate
- ao centro, o painel principal da cena ou do turno atual

Antes do combate começar, o painel central mostra o **Resumo pré-combate**.

Quando o confronto está ativo, esse mesmo painel transforma-se na área do **Turno atual**.

Quando o combate termina, o painel central mostra o **Resumo final do confronto** para o DM.

## Estrutura geral do ecrã

### Coluna esquerda

A coluna esquerda contém:

- `Controlo de combate`
- cabeçalho da lista de participantes
- lista ordenada de participantes

A lista é enquadrada por duas linhas decorativas e funcionais:

- `Início do round`
- `Fim do round`

### Painel central

O painel central muda consoante o estado do combate:

- **antes do arranque** mostra o resumo pré-combate
- **durante o confronto** mostra o participante do turno atual
- **no fim do combate** mostra o resumo final do DM

## Pré-combate

O pré-combate serve para preparar o confronto antes de arrancar o primeiro turno.

É a fase em que vale mais a pena ajustar três coisas:

- o nome dos monstros, quando queres distingui-los melhor à mesa
- as iniciativas dos heróis, introduzindo-as manualmente
- as iniciativas de PNJ e monstros, lançando-as automaticamente ou escrevendo-as à mão

## Resumo pré-combate

O cartão inicial mostra uma panorâmica rápida com métricas como:

- participantes
- heróis
- aliados
- inimigos
- PV totais dos inimigos
- participantes já em estado crítico

## Iniciativa das personagens

A secção `Iniciativa das personagens` reúne os heróis principais e permite alterar rapidamente a iniciativa antes de ordenar o confronto.

Em cada linha encontras:

- nome do participante
- subtítulo contextual
- campo de iniciativa
- botão `Eliminar`

## PNJ e monstros

A secção `PNJ e monstros` é dedicada aos participantes não heróis.

Aqui podes:

- alterar rapidamente a iniciativa
- renomear à pressa monstros e PNJ para os distinguir melhor
- usar `Init PNJ/Monstros` para lançar automaticamente a iniciativa
- introduzir manualmente o valor da iniciativa se preferires usar uma rolagem feita fora da app
- remover rapidamente um participante com `Eliminar`

## Ações principais do pré-combate

No resumo pré-combate, as ações principais são:

- `Adicionar`
- `Ordenar`
- `Iniciar confronto`

Se pelo menos um participante ainda tiver iniciativa `0`, o DnDino pede confirmação antes de começar.

## De onde podem vir os participantes

O painel de adição pode ir buscar participantes a três origens:

- `Heróis`
- `Presenças do Local`
- `Globais`

### Heróis

Aqui encontras as personagens de aventura já ligadas à campanha. Cada herói só pode entrar no combate uma vez.

### Presenças do Local

Aqui encontras as personagens que já estão presentes no local de onde nasce o combate. O seu estado local pode ser reutilizado como base para o confronto.

### Globais

Aqui encontras fichas base que ainda não estão ligadas como heróis da aventura.

No caso dos globais:

- os `Monstros` podem ser adicionados várias vezes
- `Heróis` e `PNJ` globais não podem ser duplicados como fichas globais puras

## Controlo de combate

Depois do confronto começar, o painel `Controlo de combate` mantém-se fixo acima da lista e contém as ações principais do round.

As linhas de botões são:

1. `Adicionar` e `Ordenar`
2. `Iniciar/Pausa` ou `Retomar` e `Terminar`
3. `Ant.` e `Seg.`

Se existir um último ataque reversível, aparece também:

- `Anular último ataque`

## Lista de participantes

A lista da esquerda é o coração do acompanhamento tático.

Cada linha recolhida mostra:

- posição na ordem do turno, por exemplo `1/8`
- nome do participante
- até três ícones de condições
- badge `Turno` se for o participante ativo
- CA
- PV
- PV temporários
- iniciativa

O participante ativo fica muito mais destacado do que os restantes:

- faixa lateral colorida
- rebordo mais marcado
- fundo mais quente
- scroll automático para o manter visível

A linha também usa efeitos de impacto quando o participante:

- sofre dano
- é morto
- é restaurado por um undo

## Menu contextual de uma linha

Com **clique direito** sobre o cartão do participante podes abrir o menu contextual.

Neste momento, a ação disponível é:

- `Eliminar`

## Expansão da linha do participante

Ao clicares numa linha, o participante expande-se e mostra os seus controlos rápidos.

Na parte expandida encontras:

- nome editável
- campos numéricos rápidos:
  - iniciativa
  - PV
  - PV temporários
  - CA
- botões de ação
- bloco de condições
- acesso a capacidades, especiais e feitiços, quando existirem

## Botões rápidos da linha

As ações rápidas podem incluir:

- `Atacar`
- `Dano`
- `Curar`
- `TR`
- `Notas DM`
- `Editar`
- `Condições`

Alguns botões só aparecem quando fazem sentido para esse participante.

## Atacar

`Atacar` abre um popover onde podes selecionar:

- um ou mais alvos
- o dano a aplicar

O seletor de alvos usa uma lista compacta com:

- nome
- CA
- PV
- condições

A ordem dos alvos não é aleatória. O DnDino tenta propor primeiro os participantes mais lógicos em função de quem está a atacar.

Em geral:

- se ataca um **Herói**, são propostos primeiro os **inimigos**, depois aliados, depois neutros e, por fim, monstros menos prioritários
- se ataca um participante não herói, são propostos primeiro os **heróis**, depois aliados, depois neutros e, por fim, inimigos menos adequados

Dentro de cada grupo, os nomes são ordenados alfabeticamente.

O popover nunca pré-seleciona automaticamente um alvo: a escolha tem de ser manual.

Quando aplicas um ataque a vários alvos:

- o dano é aplicado a todos os selecionados
- o banner superior mostra várias linhas, uma por cada alvo atingido
- o undo do último ataque guarda todo o grupo

## Dano e Cura

`Dano` aplica dano direto ao participante.

`Curar` aplica cura direta.

## TR

`TR` abre o popover do **Teste de Resistência** baseado nas características do participante.

## Condições

O botão `Condições` abre o popover dedicado à gestão de estados ativos.

A partir daqui podes:

- adicionar condições
- escolher duração e regras de expiração
- ligar o fim de uma condição ao turno de outro participante

## Notas DM

O botão `Notas DM` está sempre visível.

Abre um popover editável onde podes escrever notas contextuais sobre o participante. O conteúdo é guardado ao fechar o popover.

## Editar

`Editar` abre o painel de edição do participante.

Serve quando precisas de intervir de forma mais profunda em:

- iniciativa
- CA
- PV máximos, atuais e temporários
- papel no combate
- dados contextuais ligados

## Turno atual

Quando o combate está ativo, o painel central concentra-se totalmente no participante cujo turno está em curso.

A carta superior mostra:

- imagem do participante
- nome
- subtítulo
- CA
- PV
- PV temporários
- iniciativa
- velocidade
- inspiração, se o participante for um herói da aventura
- condições ativas
- características principais

## Painéis centrais durante o turno

Por baixo do resumo do turno aparecem apenas os painéis que têm realmente conteúdo.

As secções possíveis são:

- `Ataques`
- `Capacidades especiais`
- `Capacidades`
- `Descrição`
- `Feitiços`

Todos estes painéis são colapsáveis.

Além disso, usam um ligeiro acento visual:

- `Ataques` vermelho
- `Capacidades` amarelo
- `Capacidades especiais` verde
- `Feitiços` azul claro
- `Descrição` cinzento

## Ataques e ligações internas

A secção `Ataques` é um dos pontos mais fortes do combate flat.

Se preparaste ligações internas nos ataques da ficha base, podes usá-las diretamente durante o combate.

Em particular, a ligação **Ataque completo** é muito útil porque:

- executa a rolagem de ataque e dano no mesmo popover
- permite selecionar um ou mais alvos
- propõe automaticamente `Dano a aplicar`
- deixa-te excluir linhas individuais de dano se tiveres rolado vários componentes e quiseres aplicar apenas alguns
- fecha o popover assim que aplicas o dano

Isto torna os ataques dos monstros muito rápidos de usar à mesa.

## Personagens com 0 PV ou menos

Em combate, os **Heróis** seguem uma regra diferente de PNJ e monstros.

### Heróis

Os heróis podem descer abaixo de `0` PV.

A regra é:

- entre `0` e `-(PV máximos - 1)`, a personagem fica **Inconsciente**
- a `-PV máximos` ou menos, a personagem morre definitivamente

Quando um herói está a `0` PV ou menos mas ainda não morreu de forma definitiva:

- mantém-se no confronto
- no painel central aparece a carta `Testes de resistência contra a morte`

Esta carta acompanha:

- sucessos
- falhanços

e permite registar rapidamente:

- `Sucesso`
- `Falhanço`

Ao atingir 3 sucessos, a personagem volta a `1` PV. Ao atingir 3 falhanços, morre.

### PNJ e Monstros

Para os não heróis, o comportamento é mais simples:

- a `0` PV ou menos, estão mortos

## Turnos, rounds e participantes excluídos do ciclo

Dentro do ciclo de turnos:

- os heróis mortos definitivamente são excluídos
- PNJ e monstros com `0` PV ou menos são excluídos

Isto significa que um herói **Inconsciente** ainda pode ter um turno, precisamente porque os testes de resistência contra a morte têm de ser geridos.

## Banner de impacto e feedback visual

Quando um ataque acerta, o DnDino mostra um grande banner no topo com um resumo imediato.

Por exemplo:

- quem atacou
- quem foi atingido
- quanto dano foi aplicado
- se o golpe matou o alvo

Se houver vários alvos, o banner mostra várias linhas no mesmo quadro.

A **Janela dos Jogadores** também pode mostrar a animação do golpe, incluindo todos os alvos envolvidos no mesmo ataque multi-alvo.

## Anular último ataque

Quando aplicas um ataque, aparece o painel:

- `Anular último ataque`

Por baixo do botão é mostrado um pequeno resumo do que acabou de acontecer.

Se o último ataque atingiu vários alvos, o painel mostra a lista completa das linhas que serão restauradas.

Quando confirmas a anulação:

- os alvos regressam ao estado anterior
- aparece uma notificação de restauro
- o feedback visual dos cartões também é atualizado

## Resumo final do confronto

Quando o combate termina, o painel central passa para o **Resumo final do confronto** do DM.

Este ecrã mostra:

- rounds totais
- duração
- inimigos mortos
- dano causado
- dano sofrido

## O que é sincronizado no fim

Quando fechas o combate, o DnDino guarda o resultado nos registos ligados.

Para os heróis da aventura são sincronizados:

- PV atuais
- PV temporários
- condições manuais
- estado final

Para as presenças do local com estado local são sincronizados:

- PV atuais
- PV temporários
- condições manuais
- estado final

Além disso, o combate atualiza também os dados ligados à **sessão live**, incluindo:

- dano causado
- dano sofrido
- heróis caídos

## Quando o combate rende mais

O combate do DnDino rende melhor quando o usas assim:

1. preparas bem o pré-combate
2. usas dois ecrãs com a **Janela dos Jogadores**
3. aproveitas as ligações nos `Ataques` para monstros e PNJ
4. manténs o DM no tracker e os jogadores na apresentação

!!! tip
    Mesmo que o combate ofereça muitas automatizações para rolagens, ataques completos e aplicação rápida do dano, o DnDino continua a deixar espaço para uma utilização mais clássica dos dados. Podes continuar a rolar fisicamente ou gerir a rolagem fora da app e usar o combate sobretudo para aplicar os valores de forma rápida e coerente, evitando apenas a parte mais incómoda: recalcular manualmente as diferenças e atualizações dos pontos de vida em cada lance.
