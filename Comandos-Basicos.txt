## pwd
O comando pwd te mostra onde voce está, em qual diretorio voce se encontra.

## whoami
para verificar qual usuario esta logado.

## cd 
para mudar de diretorio, é essencial saber como navegar pelos diretorios e o comando cd nos ajuda com isso. para subir um nível na estrutura do arquivo use cd .., por exemplo estou na pasta cd /etc e quero voltar para pasta /, use cd .. e teste o pwd para verificar o diretorio que se encontra.

## ls
para ver conteudos de um diretorio(arquivos e subdiretorios) usamos o comando ls, semelhante ao dir do Windows.
para obter mais informacoes sobre arquivos e diretorios, por exemplo, permissoes, proprietário, tamanho e quando foi modificado, voce pode adicionar o -l depois do ls. l significa longo, grande, extenso, como achar melhor.
temos tambem a opcao ls -la onde voce consegue ver arquivos ocultos.

## --help
fornece um guia mais focado em como utilizar cada comando, aplicação ou utilitarios.
aircrack-ng --help
nmap -h
Podemos utilizar essas 3 opcoes:
--help, -h, e -?

## man
ja o man fornece documentação abrangente na forma de páginas de manual, cobrindo todos os aspectos de um comando ou tópico em detalhes.

man aircrack-ng

## locate
comando para que percorrerá todo o seu sistema de arquivos e localizará todas as ocorrências dessa palavra

locate aircrack-ng

O comando locate tem algumas limitacoes, os resultados podem ser grandes, a base de dados do locate é geralmente atualizado uma vez ao dia, entao se voce criar um arquivo há alguns minutos atrás somente no proximo dia voce irá localizar.

## whereis 
Se voce estiver localizando por arquivos executaveis, voce pode utilizar o comando whereis para isso. Esse comando retorna ate o arquivo onde se encontra a pagina do manual. Nesse caso ele só retorna apenas os executaveis da aplicação que voce esta tentando localizar e mais a pagina do manual, mais eficiente, nao acha?

## which
ainda mais especifico, ele retorna somente a localizacao do executavel na variavel path no Linux. 

## find 
o comando find é o mais avançado e flexível dos utilitários de busca. Ele é capaz de iniciar sua pesquisa em qualquer diretório designado e procurar vários parâmetros diferentes, incluindo, é claro, o nome do arquivo, mas também a data de criação ou modificação, o proprietário, o grupo, as permissões e o tamanho.

Aqui está a sintax básica para encontrar.

find directory opção expressao

Se quiséssemos encontrar um arquivo com o nome apache2 que é servidor web de código aberto iniciando no diretorio root, seria assim

find / -type f -name apache2

/ -> diretorio onde eu quero iniciar minha busca
f -> especificar que tipo de arquivo buscar, f indica um arquivo comum.
apache2 -> o nome do arquivo que estamos procurando.

como podemos imaginar essa busca demoraria, uma forma de acelerar é colocar um diretorio mais especifico para busca, por exemplo em vez de / colocariamos /etc, ai buscaria abaixo dele, somente os seus subdiretorios.

Devemos nos atentar é que o comando find mostra somente o nome exato do arquivo, por exemplo se voce estiver tentando encontrar apache2.conf essa busca anterior nao encontraria, nesse caso teriamos que usar "wildcards" nos permite a dar match em varios caracteres, por exemplo: * . , ? and [].

find /etc -type f -name apache2.

agora ele retorna o que se encaixa no padrão apache2.*

## grep e ps 
o comando grep nos auxiliar buscando palavras chaves como um filtro de busca, o comando ps é usado para mostrar informacoes sobre os processo que estao rodando na maquina, nesse caso podemos usar o comando "ps aux" junto com o grep para filtra um processo.

ps aux | grep apache2 ->  nesse caso só vai mostrar informacoes desse processo, lembre sempre de usar o "|" depois do comando seguido de grep.

# Modificando arquivos e Diretorios.

Existem varias maneiras de criar arquivos no Linux, vamos ver algumas delas.

# cat
o cat é um comando geralmente utilizado para exibir conteudos de um arquivo, mas ele tambem pode ser usado para criar arquivos pequenos. Para arquivos maiores é melhor digitar o código em um editor de texto, como o vim, emacs, leafpad, gedit ou kate e assim salva-los.

Mas para criar com cat, seria:

XXXXX

Parece confuso, mas quando voce estiver criando usando o cat ele vai entrar no modo interativo ai para finalizar o comando voce precisa pressionar CTRL-D.

Para ver o conteudo utilize o cat seguido o nome do arquivo.

Para adicionar mais conteudo no arquivo, voce pode utilizar o comando com >> e digitar o que voce quer adicionar e pressionar CTRL-D. Entao voce tera uma nova frase adicionado por exemplo.

Se voce quiser substituir é só repetir como se estivesse criando.

XXXXX

## touch
originalmente criado para que um usuário pudesse simplesmente "touch" em um arquivo para alterar alguns de seus detalhes, como a data em que foi criado ou modificado, mas se o arquivo nao existir ele irá criar o arquivo.

touch novoarquivo

## mkdir
abreviacao de make directory, comando para criar diretorios.

mkdir novodiretorio

## cp 
comando para copiar arquivos. Ele cria um arquivo duplicado na nova localizacao, ele nao move o arquivo.

XXXXX

Voce pode renomear o arquivo ao copiar se voce quiser.

XXXXX

## mv
Linux nao tem um comando especifico para renomear arquivos, com isso utilizamos o comando mv que serve tanto para mover um arquivo como para renomear.

XXXXX

## rm 
para remover um arquivo voce utiliza o comando rm.

XXXXX

## rmdir
para remover diretorios, utilizamos o rmdir, importante ressaltar que nao conseguimos remover diretorios que nao estao vazios, isso serve como segurança para nao apagar arquivos sem o conhecimento. Caso voce queira remover com conteudo no diretorio voce acrescenta o -r na frente do rmdir, tenha bastante cuidado ao utilizar.