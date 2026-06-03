# Importação e exportação

DnDino permite exportar e importar conteúdos para os mover entre instalações, criar cópias de trabalho ou partilhar material com outros Dungeon Masters.

As importações não substituem automaticamente os dados existentes: antes de guardar, podes rever o que será adicionado, substituído ou ignorado.

## Feitiços

Os feitiços podem ser exportados num ficheiro JSON.

Durante a importação, DnDino distingue:

- feitiços novos
- feitiços com o mesmo nome já presentes na base de dados

Para cada feitiço, podes escolher se queres:

- importar como novo registo
- substituir um registo existente
- ignorar

Quando já existe um feitiço com o mesmo nome, o ecrã de revisão mostra uma comparação entre o registo presente e o importado. Assim podes verificar nível, escola, manual, classes, tempo de lançamento e duração antes de decidir.

Também existem ações em massa para gerir conflitos, por exemplo ignorar todos os feitiços já existentes ou importar todos como novos.

## Personagens

As personagens são exportadas num pacote ZIP que pode incluir:

- ficha da personagem
- imagens associadas
- ligações aos feitiços
- dados necessários para reconstruir o registo noutra instalação

Durante a importação, personagens com o mesmo nome não são substituídas automaticamente. Podes importá-las como novas, substituir um registo existente ou ignorá-las.

Se a personagem importada tiver feitiços associados, DnDino tenta ligá-los aos feitiços já existentes usando o nome. Se encontrar vários feitiços compatíveis, escolhes qual usar.

Ao importar personagens para uma base de dados já preenchida, revê sempre as ligações aos feitiços: dois feitiços podem ter o mesmo nome mas vir de manuais ou versões diferentes.

## Aventuras

As aventuras são exportadas num pacote ZIP com os dados necessários para reconstruir a aventura.

Uma aventura importada é sempre criada como **nova aventura**. DnDino não substitui uma aventura existente, evitando perder locais, personagens ou sessões de uma campanha ativa.

O fluxo recomendado é por etapas:

1. importar ou associar feitiços
2. importar ou associar personagens
3. importar a aventura

Na revisão da aventura, DnDino separa as partes principais:

- feitiços incluídos no pacote
- personagens incluídas no pacote
- estrutura da aventura

Para feitiços e personagens, decides como gerir os registos já existentes. Depois disso, a aventura é importada associando as personagens corretas aos locais, presenças e restantes conteúdos do pacote.

## Equipamento, talentos e glossário

Equipamento, talentos e entradas do glossário também podem ser exportados e importados separadamente.

A exportação cria ficheiros JSON dedicados, úteis para partilhar apenas uma parte do material sem exportar uma aventura completa.

Durante a importação, o DnDino separa registos novos daqueles que já têm uma correspondência na base de dados. Para cada registo, podes importá-lo como novo, substituir o existente ou ignorá-lo.

Para equipamento, a correspondência usa nome e categoria, mantendo armas, armaduras, ferramentas e equipamento separados. Para talentos, o tipo de talento também é considerado. Para o glossário, a referência principal é o nome da entrada.

Quando já existe um registo semelhante, o ecrã de revisão compara o conteúdo atual com o importado. Usa ações em massa para ignorar, importar ou substituir vários registos de uma vez quando o ficheiro contém muitos elementos.

## Verificações antes da importação

Antes de importar pacotes com imagens, DnDino verifica se o ficheiro é legível e se existe espaço livre suficiente para copiar os media para o contentor da app.

Se o ficheiro estiver danificado, incompleto ou incompatível, a importação é interrompida com uma mensagem de erro em vez de criar dados parciais.

## Boas práticas

Antes de importar conteúdos importantes:

- cria uma cópia de segurança da app
- importa primeiro os feitiços se muitas personagens os usarem
- revê os registos com o mesmo nome antes de os substituir
- usa a comparação entre antigo e novo quando tiveres dúvidas
- importa aventuras como novas e depois verifica ligações, locais e imagens

A importação foi pensada para proteger a base de dados: em caso de dúvida, escolhe `Importar como novo` ou `Ignorar` em vez de substituir.
