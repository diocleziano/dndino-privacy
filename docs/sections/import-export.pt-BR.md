# Importação e exportação

DnDino permite exportar e importar conteúdo para mover entre instalações, criar cópias de trabalho ou compartilhar material com outros Dungeon Masters.

As importações não substituem automaticamente os dados existentes: antes de salvar, você pode revisar o que será adicionado, substituído ou ignorado.

## Magias

As magias podem ser exportadas em um arquivo JSON.

Durante a importação, DnDino separa:

- magias novas
- magias com o mesmo nome já presentes no banco de dados

Para cada magia, você pode escolher se deseja:

- importar como novo registro
- substituir um registro existente
- ignorar

Quando já existe uma magia com o mesmo nome, a tela de revisão mostra uma comparação entre o registro atual e o importado. Assim você pode conferir nível, escola, manual, classes, tempo de conjuração e duração antes de decidir.

Também há ações em massa para lidar com conflitos, por exemplo ignorar todas as magias já existentes ou importar todas como novas.

## Personagens

Os personagens são exportados em um pacote ZIP que pode incluir:

- ficha do personagem
- imagens vinculadas
- links para magias
- dados necessários para reconstruir o registro em outra instalação

Durante a importação, personagens com o mesmo nome não são substituídos automaticamente. Você pode importá-los como novos, substituir um registro existente ou ignorá-los.

Se o personagem importado tiver magias vinculadas, DnDino tenta associá-las às magias já existentes usando o nome. Se encontrar várias magias compatíveis, você escolhe qual usar.

Ao importar personagens para um banco de dados já cheio, revise sempre os links de magias: duas magias podem ter o mesmo nome, mas vir de manuais ou versões diferentes.

## Aventuras

As aventuras são exportadas em um pacote ZIP com os dados necessários para reconstruir a aventura.

Uma aventura importada é sempre criada como **nova aventura**. DnDino não substitui uma aventura existente, evitando perda de lugares, personagens ou sessões de uma campanha ativa.

O fluxo recomendado é por etapas:

1. importar ou vincular magias
2. importar ou vincular personagens
3. importar a aventura

Na revisão da aventura, DnDino separa as partes principais:

- magias incluídas no pacote
- personagens incluídos no pacote
- estrutura da aventura

Para magias e personagens, você decide como lidar com registros já existentes. Depois disso, a aventura é importada vinculando os personagens corretos aos lugares, presenças e demais conteúdos do pacote.

## Equipamento, talentos e glossário

Equipamento, talentos e entradas do glossário também podem ser exportados e importados separadamente.

A exportação cria arquivos JSON dedicados, úteis para compartilhar apenas uma parte do material sem exportar uma aventura inteira.

Durante a importação, o DnDino separa registros novos daqueles que já têm uma correspondência no banco de dados. Para cada registro, você pode importá-lo como novo, substituir o existente ou ignorá-lo.

Para equipamento, a correspondência usa nome e categoria, mantendo armas, armaduras, ferramentas e equipamentos separados. Para talentos, o tipo de talento também é considerado. Para o glossário, a referência principal é o nome da entrada.

Quando já existe um registro semelhante, a tela de revisão compara o conteúdo atual com o importado. Use ações em massa para ignorar, importar ou substituir vários registros de uma vez quando o arquivo contém muitos itens.

## Verificações antes da importação

Antes de importar pacotes com imagens, DnDino verifica se o arquivo pode ser lido e se há espaço livre suficiente para copiar os arquivos de mídia para o contêiner do app.

Se o arquivo estiver danificado, incompleto ou incompatível, a importação é interrompida com uma mensagem de erro em vez de criar dados parciais.

## Boas práticas

Antes de importar conteúdo importante:

- crie um backup do app
- importe primeiro as magias se muitos personagens forem usá-las
- revise os registros com o mesmo nome antes de substituí-los
- use a comparação entre antigo e novo quando estiver em dúvida
- importe aventuras como novas e depois revise links, lugares e imagens

A importação foi pensada para proteger o banco de dados: em caso de dúvida, escolha `Importar como novo` ou `Ignorar` em vez de substituir.
