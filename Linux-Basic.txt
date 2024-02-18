# Introducao dos Termos e Conceitos.

Antes de iniciarmos qualquer teoria sobre hacker e scripts, vamos aprender um pouco sobre alguns termos para facilitar cada passo.

## Binaries
Este termo se refere a arquivos que podem ser executados, parecidos com exe do Windows. Geralmente residem no diretório /usr/bin ou /usr/sbin que incluem utilitatios como ps, cat, ls e ifconfig.

## Case sensitivity
Diferente do Windows, o sistem de arquivos do Linux é case sensitive. Isso significa que Desktop é diferente de desktop.

## Directory
Mesma coisa que Arquivos do Windows.

## Home
Cada usuario tem o seu próprio /home, é onde os arquivos que você criar serão salvos por padrão.

## root
Como a maioria dos SO tem um Admin ou superuser, que só pode ser usado por pessoas especificas, a maioria dos programas precisa ser executados como root e claro com essa permissao voce pode alterar senha de usuarios, reconfigura sistema e adicionar usuarios, mas lembre-se como diria Tio Ben, como grandes poderes vem grandes responsabilidades.

## scripts
é uma serie de comandos executaveis em um ambiente interpretativo que converte cada linha em código-fonte. Os scripts podem ser executados com o interpretador bash ou com outras linguagens, especialmente Python, uma das mais utilizadas.

## Shell
Um ambiente e tradutor para rodar comandos no Linux. O shell mais usado é o bash.

## Terminal
É a interface de linha de comando (CLI)


==============================================================================================================================

Abra o terminal do Kali Linux que é a interface de linha de comando.

# O sistema de arquivos do Linux

A estrutura de arquivo do Linux é um pouco diferente do Windows, Linux nao tem uma unidade fisica C: na base do Sistema de arquivo mas, em vez disso, utiliza um sistema de arquivo logico. No topo do sistema de arquivos está a "/", que geralmente é chamado a raiz do sistema de arquivo. Com o tempo isso ficará mais claro na sua mente, vamos debater mais sobre isso.

/root -> O diretório home do usuario root.
/etc -> Em geral contem os arquivos de configuracao do Linux, arquivos que controla quando e como os programas são iniciados.
/home -> Diretório do usuario.
/mnt -> Onde outros sistemas de arquivos são anexados ou montados no sistema de arquivos.
/media -> Onde CDs e dispositivo USB sao geralmente anexados ou montados.
/bin -> Onde residem os binários dos aplicativos (O equivalente a executáveis no Microsoft Windows ou aplicativos no macOS).
/lib -> Onde você encontrará as bibliotecas, similar aos DLLs do Windows.







