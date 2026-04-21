# Combate

O modo **Combate** do DnDino foi pensado para ser o principal tracker operacional do confronto. Esta página descreve o modo de combate padrão do DnDino.

O combate nasce sempre no contexto de um **local** e leva consigo os personagens, as presenças locais e os possíveis monstros ou NPCs ligados àquela cena.

Esta página explica todo o fluxo:

- preparação do pré-combate
- gestão dos participantes
- início do confronto
- uso do painel do turno atual
- aplicação de dano, cura, condições e testes de resistência
- integração com a **Janela dos Jogadores**
- encerramento do confronto e resumo final

## Uso com uma ou duas telas

O combate do DnDino funciona muito bem também em **uma única tela**: toda a parte operacional fica no painel principal e você pode gerenciar participantes, turnos, dano, condições e o resumo final sem precisar de um segundo monitor.

Dito isso, se você tiver uma configuração com duas telas, pode usar:

- uma tela principal para o painel de controle do DM
- uma segunda tela ou monitor para a **Janela dos Jogadores**

Nessa configuração o fluxo fica ainda mais confortável:

- na tela do DM permanecem visíveis a lista de participantes, os controles do round, o turno atual, os textos de ataque, as notas DM e as edições rápidas
- na tela dos jogadores é mostrada uma apresentação limpa do participante ativo, com imagem e overlay contextual

Na prática:

- em tela única você usa todo o combate a partir da tela principal
- com duas telas você separa o painel técnico do DM da apresentação para os jogadores

!!! tip
    A segunda tela não é obrigatória. Ela é apenas um reforço muito útil quando você quer mostrar imagens e informações do turno atual aos jogadores sem expor o painel técnico do DM.

## Como funciona a Janela dos Jogadores durante o combate

Quando o combate é iniciado, o DnDino pode abrir ou atualizar automaticamente a **Janela dos Jogadores**.

Se a apresentação para os jogadores estiver ativa:

- no início do combate pode aparecer uma breve **intro** com os participantes
- durante o combate a janela se atualiza para o **participante do turno atual**
- no fim do confronto pode aparecer um **resumo final**

Durante o combate, a Janela dos Jogadores não mostra o painel técnico do DM, e sim uma apresentação visual com:

- imagem do participante ativo
- nome mostrado aos jogadores
- informações de overlay, se estiverem ativadas

O overlay pode incluir:

- round atual
- PV atuais, máximos e temporários
- condições
- próximo turno

Algumas informações sobre inimigos podem ser tratadas de forma separada em relação às dos heróis.

## Configurações da Janela dos Jogadores e da segunda tela

As opções mais importantes ficam em **Configurações**, na área dedicada à apresentação do combate e da janela dos jogadores.

### Abertura e comportamento geral

As principais configurações são:

- `Abrir janela dos jogadores mesmo com um só monitor`
- `Mostrar controles da janela dos jogadores na barra superior`
- `Mostrar intro de combate aos jogadores`
- `Mostrar resumo final aos jogadores`

#### Abrir janela dos jogadores mesmo com um só monitor

Se essa opção estiver ativa, o DnDino pode abrir automaticamente a Janela dos Jogadores mesmo quando você estiver trabalhando com apenas um monitor.

Se estiver desativada:

- com um único monitor a janela não se abre automaticamente
- se ela já estiver aberta, continuará mesmo assim a ser atualizada

#### Mostrar controles da janela dos jogadores na barra superior

Se você ativar essa opção, aparecem botões na barra superior para:

- abrir manualmente a janela dos jogadores
- fechá-la manualmente

#### Mostrar intro de combate aos jogadores

Quando você pressiona `Iniciar confronto`, a Janela dos Jogadores pode mostrar uma breve introdução com:

- título do confronto
- participantes envolvidos
- quantidade de participantes

Se você desativar essa opção, o combate passa direto para a apresentação do primeiro participante ativo.

#### Mostrar resumo final aos jogadores

Quando o combate termina, a Janela dos Jogadores pode mostrar um resumo final.

O resumo voltado aos jogadores mostra apenas dados úteis para eles, como:

- dano causado pelos heróis
- dano sofrido pelos heróis
- imagem do pior inimigo

O resumo final dos jogadores permanece visível até você mudar o conteúdo da janela ou fechá-la.

### Informação mostrada durante o turno

As configurações que controlam o overlay do participante ativo são:

- `Mostrar round na janela dos jogadores`
- `Mostrar PV na janela dos jogadores`
- `Mostrar condições na janela dos jogadores`
- `Mostrar próximo turno na janela dos jogadores`

### Informação sobre inimigos, monstros e NPCs

Para participantes que não são heróis existem controles dedicados:

- `Mostrar detalhes de NPCs e monstros aos jogadores`
- `Mostrar condições dos inimigos aos jogadores`
- `Mostrar nomes dos inimigos aos jogadores`

Isso permite decidir se a Janela dos Jogadores deve:

- mostrar a criatura de forma mais evocativa
- ou mostrar também dados mais técnicos

## Onde o combate é aberto

O combate é criado a partir do contexto de um **local**. Depois de aberto, o DnDino mostra uma tela dividida em duas colunas principais:

- à esquerda, o tracker operacional do combate
- ao centro, o painel principal da cena ou do turno atual

Antes do combate começar, o painel central mostra o **Resumo pré-combate**.

Quando o confronto está ativo, esse mesmo painel se transforma na área do **Turno atual**.

Quando o combate termina, o painel central mostra o **Resumo final do confronto** para o DM.

## Estrutura geral da tela

### Coluna esquerda

A coluna esquerda contém:

- `Controle de combate`
- cabeçalho da lista de participantes
- lista ordenada de participantes

A lista é enquadrada por duas linhas decorativas e funcionais:

- `Início do round`
- `Fim do round`

### Painel central

O painel central muda conforme o estado do combate:

- **antes do início** mostra o resumo pré-combate
- **durante o confronto** mostra o participante do turno atual
- **no final do combate** mostra o resumo final do DM

## Pré-combate

O pré-combate serve para preparar o confronto antes de iniciar o primeiro turno.

É a fase em que mais vale a pena ajustar três coisas:

- o nome dos monstros, quando você quer distingui-los melhor na mesa
- as iniciativas dos heróis, inserindo-as manualmente
- as iniciativas de NPCs e monstros, rolando automaticamente ou digitando manualmente

## Resumo pré-combate

O cartão inicial mostra uma visão rápida com métricas como:

- participantes
- heróis
- aliados
- inimigos
- PV totais dos inimigos
- participantes já em condição crítica

## Iniciativa dos personagens

A seção `Iniciativa dos personagens` reúne os heróis principais e permite alterar rapidamente a iniciativa antes de ordenar o confronto.

Em cada linha você encontra:

- nome do participante
- subtítulo contextual
- campo de iniciativa
- botão `Excluir`

## NPCs e monstros

A seção `NPCs e monstros` é dedicada aos participantes não heróis.

Aqui você pode:

- alterar rapidamente a iniciativa
- renomear monstros e NPCs rapidamente para diferenciá-los melhor
- usar `Init NPCs/Monstros` para rolar a iniciativa automaticamente
- inserir manualmente o valor da iniciativa se preferir usar uma rolagem feita fora do aplicativo
- remover rapidamente um participante com `Excluir`

## Ações principais do pré-combate

No resumo pré-combate, as ações principais são:

- `Adicionar`
- `Ordenar`
- `Iniciar confronto`

Se pelo menos um participante ainda tiver iniciativa `0`, o DnDino pede confirmação antes de começar.

## De onde os participantes podem vir

O painel de adicionar participantes pode puxar participantes de três origens:

- `Heróis`
- `Presenças do local`
- `Globais`

### Heróis

Aqui aparecem os personagens de aventura já vinculados à campanha. Cada herói só pode entrar no combate uma vez.

### Presenças do local

Aqui aparecem os personagens que já estão presentes no local de onde o combate nasce. O estado local deles pode ser reutilizado como base para o confronto.

### Globais

Aqui aparecem fichas base que ainda não estão vinculadas como heróis da aventura.

No caso dos globais:

- os `Monstros` podem ser adicionados várias vezes
- `Heróis` e `NPCs` globais não podem ser duplicados como fichas globais puras

## Controle de combate

Depois que o confronto começa, o painel `Controle de combate` permanece fixo acima da lista e contém as ações principais do round.

As linhas de botões são:

1. `Adicionar` e `Ordenar`
2. `Iniciar/Pausar` ou `Retomar` e `Encerrar`
3. `Ant.` e `Próx.`

Se existir um último ataque reversível, também aparece:

- `Desfazer último ataque`

## Lista de participantes

A lista da esquerda é o coração do acompanhamento tático.

Cada linha recolhida mostra:

- posição na ordem do turno, por exemplo `1/8`
- nome do participante
- até três ícones de condições
- selo `Turno` se for o participante ativo
- CA
- PV
- PV temporários
- iniciativa

O participante ativo fica muito mais destacado do que os demais:

- faixa lateral colorida
- borda mais forte
- fundo mais quente
- rolagem automática para mantê-lo visível

A linha também usa efeitos de impacto quando o participante:

- sofre dano
- morre
- é restaurado por um undo

## Menu contextual de uma linha

Com **clique direito** no cartão do participante você pode abrir o menu contextual.

No momento, a ação disponível é:

- `Excluir`

## Expansão da linha do participante

Ao clicar em uma linha, o participante se expande e mostra seus controles rápidos.

Na parte expandida você encontra:

- nome editável
- campos numéricos rápidos:
  - iniciativa
  - PV
  - PV temporários
  - CA
- botões de ação
- bloco de condições
- acesso a habilidades, especiais e magias, quando existirem

## Botões rápidos da linha

As ações rápidas podem incluir:

- `Atacar`
- `Dano`
- `Curar`
- `TR`
- `Notas DM`
- `Editar`
- `Condições`

Alguns botões só aparecem quando fazem sentido para aquele participante.

## Atacar

`Atacar` abre um popover onde você pode selecionar:

- um ou mais alvos
- o dano a aplicar

O seletor de alvos usa uma lista compacta com:

- nome
- CA
- PV
- condições

A ordem dos alvos não é aleatória. O DnDino tenta sugerir primeiro os participantes mais lógicos com base em quem está atacando.

Em geral:

- se ataca um **Herói**, são sugeridos primeiro os **inimigos**, depois aliados, depois neutros e por fim monstros menos prioritários
- se ataca um participante que não é herói, são sugeridos primeiro os **heróis**, depois aliados, depois neutros e por fim inimigos menos adequados

Dentro de cada grupo, os nomes são então ordenados alfabeticamente.

O popover nunca pré-seleciona automaticamente um alvo: a escolha precisa ser manual.

Quando você aplica um ataque a vários alvos:

- o dano é aplicado a todos os selecionados
- o banner superior mostra várias linhas, uma para cada alvo atingido
- o undo do último ataque mantém todo o grupo

## Dano e Cura

`Dano` aplica dano direto ao participante.

`Curar` aplica cura direta.

## TR

`TR` abre o popover do **Teste de Resistência** com base nas características do participante.

## Condições

O botão `Condições` abre o popover dedicado à gestão dos estados ativos.

A partir daí você pode:

- adicionar condições
- escolher duração e regras de expiração
- ligar o fim de uma condição ao turno de outro participante

## Notas DM

O botão `Notas DM` está sempre visível.

Ele abre um popover editável onde você pode escrever notas contextuais sobre o participante. O conteúdo é salvo ao fechar o popover.

## Editar

`Editar` abre o painel de edição do participante.

Ele serve quando você precisa intervir de forma mais profunda em:

- iniciativa
- CA
- PV máximos, atuais e temporários
- papel no combate
- dados contextuais vinculados

## Turno atual

Quando o combate está ativo, o painel central se concentra totalmente no participante cujo turno está em andamento.

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

Debaixo do resumo do turno aparecem apenas os painéis que têm conteúdo real.

As seções possíveis são:

- `Ataques`
- `Habilidades especiais`
- `Habilidades`
- `Descrição`
- `Magias`

Todos esses painéis são recolhíveis.

Além disso, usam um leve acento visual:

- `Ataques` vermelho
- `Habilidades` amarelo
- `Habilidades especiais` verde
- `Magias` azul-claro
- `Descrição` cinza

## Ataques e links internos

A seção `Ataques` é um dos pontos mais fortes do combate flat.

Se você preparou links internos dentro dos ataques da ficha base, pode usá-los diretamente durante o combate.

Em especial, o link **Ataque completo** é muito útil porque:

- executa a rolagem de ataque e dano no mesmo popover
- permite selecionar um ou mais alvos
- sugere automaticamente `Dano a aplicar`
- permite excluir linhas individuais de dano se você rolou vários componentes e quer aplicar apenas alguns
- fecha o popover assim que o dano é aplicado

Isso torna os ataques dos monstros muito rápidos de usar na mesa.

## Personagens com 0 PV ou menos

Em combate, os **Heróis** seguem uma regra diferente da de NPCs e monstros.

### Heróis

Os heróis podem descer abaixo de `0` PV.

A regra é:

- entre `0` e `-(PV máximos - 1)`, o personagem fica **Inconsciente**
- a `-PV máximos` ou menos, o personagem morre definitivamente

Quando um herói está com `0` PV ou menos, mas ainda não morreu de forma definitiva:

- ele permanece no confronto
- no painel central aparece o cartão `Testes de resistência contra a morte`

Esse cartão acompanha:

- sucessos
- falhas

e permite registrar rapidamente:

- `Sucesso`
- `Falha`

Ao atingir 3 sucessos, o personagem volta a `1` PV. Ao atingir 3 falhas, morre.

### NPCs e Monstros

Para os não heróis, o comportamento é mais simples:

- com `0` PV ou menos, estão mortos

## Turnos, rounds e participantes excluídos do ciclo

Dentro do ciclo de turnos:

- heróis mortos definitivamente são excluídos
- NPCs e monstros com `0` PV ou menos são excluídos

Isso significa que um herói **Inconsciente** ainda pode ter turno, justamente porque os testes de resistência contra a morte precisam ser gerenciados.

## Banner de impacto e feedback visual

Quando um ataque acerta, o DnDino mostra um grande banner no topo com um resumo imediato.

Por exemplo:

- quem acertou
- quem foi atingido
- quanto dano foi aplicado
- se o golpe matou o alvo

Se houver vários alvos, o banner mostra várias linhas dentro do mesmo quadro.

A **Janela dos Jogadores** também pode mostrar a animação do golpe, incluindo todos os alvos envolvidos no mesmo ataque multi-alvo.

## Desfazer último ataque

Quando você aplica um ataque, aparece o painel:

- `Desfazer último ataque`

Debaixo do botão aparece um pequeno resumo do que acabou de acontecer.

Se o último ataque tiver acertado vários alvos, o painel mostra a lista completa das linhas que serão restauradas.

Quando você confirma o undo:

- os alvos voltam ao estado anterior
- aparece uma notificação de restauração
- o feedback visual dos cartões também é atualizado

## Resumo final do confronto

Quando o combate termina, o painel central passa para o **Resumo final do confronto** do DM.

Essa tela mostra:

- rounds totais
- duração
- inimigos abatidos
- dano causado
- dano sofrido

## O que é sincronizado no final

Quando você fecha o combate, o DnDino grava o resultado nos registros vinculados.

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

Além disso, o combate atualiza também os dados vinculados à **sessão ao vivo**, incluindo:

- dano causado
- dano sofrido
- heróis caídos

## Quando o combate rende mais

O combate do DnDino rende melhor quando você o usa assim:

1. prepara bem o pré-combate
2. usa duas telas com a **Janela dos Jogadores**
3. aproveita os links em `Ataques` para monstros e NPCs
4. mantém o DM no tracker e os jogadores na apresentação

!!! tip
    Mesmo que o combate ofereça muitas automatizações para rolagens, ataques completos e aplicação rápida de dano, o DnDino continua deixando espaço para um uso mais clássico dos dados. Você pode continuar rolando fisicamente ou resolvendo a rolagem fora do aplicativo e usar o combate principalmente para aplicar os valores de forma rápida e consistente, evitando só a parte mais chata: recalcular manualmente as diferenças e atualizações dos pontos de vida a cada lance.
