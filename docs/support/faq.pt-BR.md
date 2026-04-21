# FAQ

Esta seção reúne respostas rápidas para as dúvidas mais comuns sobre o DnDino.

Se você precisar de uma explicação completa de uma tela específica, o ideal é abrir depois a página dedicada do guia. A FAQ serve principalmente para os casos práticos mais frequentes.

## Como volto rapidamente para a minha última campanha?

Abra a tela `Início` e use o cartão da **última aventura**.

A partir daí você pode:

- abrir diretamente o painel da aventura
- ir para o último local visitado, se ele estiver disponível

Essa é a forma mais rápida de retomar o trabalho sem passar toda vez pela lista completa de aventuras.

## Qual é a diferença entre ficha base, personagem de aventura, presença no local e participante de combate?

A **ficha base** é o registro geral do personagem ou da criatura.

A partir dessa ficha, o DnDino pode criar registros contextuais separados:

- o **personagem de aventura**, usado dentro de uma campanha
- a **presença no local**, usada nos locais
- o **participante de combate**, usado no confronto

Esse sistema serve para manter separados:

- nomes contextuais
- iniciativa
- PV atuais
- notas do DM
- estado local do combate ou do local

Em outras palavras, a ficha base continua sendo a referência geral, enquanto os registros contextuais permitem trabalhar de forma prática durante a sessão.

## Como adiciono um herói à aventura?

Abra o `Painel da Aventura` e vá para a seção `Personagens`.

A partir daí você pode:

- adicionar um personagem existente
- criar um novo personagem com `Criar personagem`

Se você criar um novo personagem a partir do seletor, ao salvar volta para o painel de seleção e a lista é atualizada imediatamente.

## Como adiciono uma presença a um local?

Abra o local e vá para a seção `Presenças`.

A partir daí você pode adicionar:

- um herói já vinculado à aventura
- um `NPC`
- um `Monstro`

Lembre-se desta diferença importante:

- um `NPC` continua único naquele local
- um `Monstro` pode ser adicionado mais de uma vez

Isso permite ter várias instâncias do mesmo monstro no mesmo local, evitando duplicações indesejadas de NPCs.

## Posso mudar o nome de um monstro sem alterar a ficha base?

Sim.

Essa é justamente uma das razões pelas quais o DnDino usa registros contextuais.

Você pode renomear um monstro:

- no pré-combate
- nas presenças dos locais
- em outros contextos locais em que o nome operacional precise ser mais fácil de ler

Isso não altera o nome da ficha base original.

## Como faço um link rápido para um personagem ou um local dentro de uma descrição?

Nos campos de texto que aceitam links internos, use o comando `Link`.

A partir daí você pode criar links para:

- personagens
- locais
- magias
- regras
- talentos

Isso é especialmente útil:

- em `Locais`, para ligar outros locais ou personagens citados na descrição
- em `Personagens`, principalmente em `Ataques`, para ligar jogadas ou referências úteis

## Para que servem os links nos Ataques dos monstros?

Eles servem para transformar um texto descritivo em uma ferramenta prática.

Nos campos rich text dos ataques você pode inserir links como:

- `Ataque completo`
- `Rolagem livre`
- `Rolar dados`
- `Rolagem de ataque`

Isso permite:

- rolar dados rapidamente
- aplicar dano aos alvos
- ligar outras entradas do aplicativo

É uma das formas mais eficazes de tornar a ficha de um monstro realmente útil durante o combate.

## Sou obrigado a usar as rolagens automáticas no combate?

Não.

O DnDino oferece muitas automações, mas não obriga você a usá-las.

Você pode continuar:

- rolando dados físicos na mesa
- lendo os resultados do jeito tradicional
- aplicando o dano manualmente

O aplicativo ajuda principalmente a tirar o trabalho repetitivo de atualizar PV e fazer contas mentais.

## O combate funciona bem mesmo com apenas um monitor?

Sim.

O `Combate Flat` funciona bem mesmo em uma única tela.

Usar uma segunda tela com a `Janela dos Jogadores` é ótimo para apresentação, mas não é obrigatório. Em um monitor só você ainda consegue usar o combate sem dificuldade e decidir nas configurações como a janela dos jogadores deve se comportar.

## Posso decidir quanta informação os jogadores veem durante o combate?

Sim.

Em `Configurações > Combate`, entre outras coisas, você pode decidir se os jogadores veem:

- rodada
- PV
- condições
- próximo turno
- nome real dos inimigos
- detalhes de NPCs e monstros

Isso permite escolher entre um combate mais transparente ou mais no estilo de escudo do mestre.

## Como funciona o resumo final do combate?

No fim do combate, o DnDino encerra o confronto e sincroniza os dados contextuais com os registros vinculados.

Além disso:

- o DM vê o resumo final dentro do combate
- os jogadores podem ver um resumo na `Janela dos Jogadores`, se a opção estiver ativada

O resumo público é focado nos personagens, e não nos inimigos.

## O que acontece se um herói cair abaixo de 0 PV?

Os heróis podem ficar com valores negativos.

A regra tratada pelo aplicativo é a seguinte:

- entre `0` e `-(PV máximos - 1)`, o herói fica `Inconsciente`
- com `-PV máximos` ou menos, o herói morre definitivamente

Durante o combate, quando um herói está inconsciente, o DnDino também mostra o painel de **testes de resistência contra a morte**.

## Como mostro uma imagem para os jogadores?

O DnDino usa uma janela dedicada para apresentação aos jogadores.

Você pode usá-la:

- durante o combate
- nas imagens da aventura
- em outros fluxos que suportam apresentação

O comportamento dessa janela é configurado em `Configurações > Mídia` e, em parte, em `Configurações > Combate`.

## Como faço backup dos meus dados?

Vá em `Configurações > Banco de dados`.

A partir daí você pode:

- ver onde os dados do aplicativo estão armazenados
- abrir a pasta de dados
- abrir a pasta de backups
- criar manualmente um snapshot
- restaurar um snapshot
- restaurar do iCloud, se estiver configurado

Na mesma seção você também pode decidir:

- a frequência dos backups automáticos
- o número máximo de snapshots mantidos

## Onde encontro informações técnicas do banco de dados se algo parecer errado?

Vá em `Configurações > Diagnóstico`.

Lá você pode verificar:

- o caminho do banco de dados
- se o arquivo existe
- o tamanho
- a data da última modificação
- a versão do SQLite
- as tabelas encontradas e o número de registros

Essa é a seção certa para entender se um problema é apenas visual ou se realmente afeta os dados salvos.

## Como entro em contato com o suporte?

Abra `Configurações > Suporte`.

A partir daí você pode:

- enviar um pedido de suporte
- enviar uma sugestão
- copiar o email de contato

Use `Suporte` quando algo não funciona ou não está claro. Use `Sugestão` quando quiser propor uma melhoria ou uma nova funcionalidade.

!!! tip
    Se uma resposta aqui parecer curta demais, use a FAQ como ponto de partida e depois abra a página dedicada do guia, como `Personagens`, `Locais`, `Combate` ou `Configurações`.
