# FAQ

Esta secção reúne respostas rápidas às perguntas mais comuns sobre o DnDino.

Se precisar de uma explicação completa de um ecrã específico, o melhor é abrir depois a página dedicada do guia. A FAQ serve sobretudo para os casos práticos mais frequentes.

## Como retomo rapidamente a minha última campanha?

Abra o `Início` e use o cartão da **última aventura**.

A partir daí pode:

- abrir diretamente o painel da aventura
- ir para o último local visitado, se estiver disponível

É a forma mais rápida de retomar o trabalho sem passar sempre pela lista completa de aventuras.

## Qual é a diferença entre ficha base, personagem de aventura, presença de local e participante em combate?

A **ficha base** é o registo geral da personagem ou criatura.

A partir dessa ficha, o DnDino pode criar registos contextuais separados:

- a **personagem de aventura**, usada dentro de uma campanha
- a **presença de local**, usada nos locais
- o **participante em combate**, usado no confronto

Este sistema serve para manter separados:

- nomes contextuais
- iniciativa
- PV atuais
- notas do DM
- estado local do combate ou do local

Por outras palavras, a ficha base continua a ser a referência geral, enquanto os registos contextuais permitem trabalhar de forma prática durante a sessão.

## Como adiciono um herói à aventura?

Abra o `Painel da Aventura` e vá ao painel `Personagens`.

A partir daí pode:

- adicionar uma personagem existente
- criar uma nova personagem com `Criar personagem`

Se criar uma nova personagem a partir do seletor, ao guardar volta ao painel de seleção e a lista é atualizada imediatamente.

## Como adiciono uma presença a um local?

Abra o local e vá ao painel `Presenças`.

A partir daí pode adicionar:

- um herói já ligado à aventura
- um `NPC`
- um `Monstro`

Lembre-se desta diferença importante:

- um `NPC` mantém-se único nesse local
- um `Monstro` pode ser adicionado mais do que uma vez

Isto permite ter várias instâncias do mesmo monstro no mesmo local, evitando ao mesmo tempo duplicações indesejadas de NPCs.

## Posso mudar o nome de um monstro sem alterar a ficha base?

Sim.

Essa é precisamente uma das razões pelas quais o DnDino usa registos contextuais.

Pode renomear um monstro:

- no pré-combate
- nas presenças dos locais
- noutros contextos locais em que o nome operativo precise de ser mais cómodo de ler

Isto não altera o nome da ficha base original.

## Como ligo rapidamente uma personagem ou um local dentro de uma descrição?

Nos campos de texto que suportam ligações internas, use o comando `Link`.

A partir daí pode criar ligações para:

- personagens
- locais
- feitiços
- regras
- talentos

Isto é especialmente útil:

- em `Locais`, para ligar outros locais ou personagens mencionados na descrição
- em `Personagens`, sobretudo em `Ataques`, para ligar jogadas ou referências úteis

## Para que servem as ligações nos Ataques dos monstros?

Servem para transformar um texto descritivo numa ferramenta prática.

Nos campos rich text dos ataques pode inserir ligações como:

- `Ataque completo`
- `Rolagem livre`
- `Lançar dados`
- `Rolagem de ataque`

Isto permite:

- lançar dados rapidamente
- aplicar dano aos alvos
- ligar outras entradas da aplicação

É uma das formas mais eficazes de tornar a ficha de um monstro realmente útil durante o combate.

## Sou obrigado a usar as rolagens automáticas no combate?

Não.

O DnDino oferece muitas automatizações, mas não obriga a utilizá-las.

Pode continuar a:

- lançar dados físicos à mesa
- ler os resultados da forma tradicional
- aplicar o dano manualmente

A aplicação ajuda sobretudo a retirar o trabalho repetitivo de atualizar PV e fazer contas mentais.

## O combate funciona bem também com apenas um monitor?

Sim.

O `Combate Flat` funciona bem mesmo num único ecrã.

O segundo ecrã com a `Janela dos Jogadores` é ótimo para apresentação, mas não é um requisito. Num só monitor pode usar o combate sem problemas e decidir nas definições como a janela dos jogadores se deve comportar.

## Posso decidir quanta informação os jogadores veem durante o combate?

Sim.

Em `Definições > Combate`, entre outras coisas, pode decidir se os jogadores veem:

- ronda
- PV
- condições
- próximo turno
- nome real dos inimigos
- detalhes de NPCs e monstros

Isto permite-lhe escolher entre um combate mais transparente ou mais ao estilo de ecrã de DM.

## Como funciona o resumo final do combate?

No final do combate, o DnDino encerra o confronto e sincroniza os dados contextuais com os registos ligados.

Além disso:

- o DM vê o resumo final dentro do combate
- os jogadores podem ver um resumo na `Janela dos Jogadores`, se a opção estiver ativa

O resumo público está centrado nas personagens e não nos inimigos.

## O que acontece se um herói descer abaixo de 0 PV?

Os heróis podem ficar com valores negativos.

A regra tratada pela aplicação é a seguinte:

- entre `0` e `-(PV máximos - 1)`, o herói fica `Inconsciente`
- com `-PV máximos` ou menos, o herói morre definitivamente

Durante o combate, quando um herói está inconsciente, o DnDino mostra também o painel de **testes de resistência contra a morte**.

## Como mostro uma imagem aos jogadores?

O DnDino usa uma janela dedicada para apresentação aos jogadores.

Pode usá-la:

- durante o combate
- nas imagens da aventura
- noutros fluxos que suportam apresentação

O comportamento desta janela é regulado em `Definições > Média` e, em parte, em `Definições > Combate`.

## Como faço cópias de segurança dos meus dados?

Vá a `Definições > Base de Dados`.

A partir daí pode:

- ver onde os dados da aplicação estão guardados
- abrir a pasta de dados
- abrir a pasta de cópias de segurança
- criar manualmente um snapshot
- restaurar um snapshot
- restaurar a partir do iCloud, se estiver configurado

Na mesma secção também pode decidir:

- a frequência das cópias automáticas
- o número máximo de snapshots mantidos

## Onde encontro informação técnica da base de dados se algo parecer errado?

Vá a `Definições > Diagnóstico`.

Aí pode verificar:

- o caminho da base de dados
- se o ficheiro existe
- o tamanho
- a data da última modificação
- a versão de SQLite
- as tabelas encontradas e o número de registos

É a secção certa para perceber se um problema é apenas visual ou se afeta realmente os dados guardados.

## Como contacto o suporte?

Abra `Definições > Suporte`.

A partir daí pode:

- enviar um pedido de suporte
- enviar uma sugestão
- copiar o email de contacto

Use `Suporte` quando algo não funciona ou não está claro. Use `Sugestão` quando quiser propor uma melhoria ou uma nova funcionalidade.

!!! tip
    Se uma resposta aqui lhe parecer demasiado curta, use a FAQ como ponto de partida e depois abra a página dedicada do guia, por exemplo `Personagens`, `Locais`, `Combate` ou `Definições`.
