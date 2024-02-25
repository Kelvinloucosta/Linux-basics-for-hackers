# Introdução aos Termos e Conceitos

Antes de mergulharmos em qualquer teoria sobre hackers e scripts, é importante entender alguns termos básicos que facilitarão nossa jornada.

## Binários

Esses são arquivos executáveis, semelhantes aos .exe do Windows. Normalmente estão localizados nos diretórios /usr/bin ou /usr/sbin e incluem utilitários como ps, cat, ls e ifconfig.

## Sensibilidade a Maiúsculas e Minúsculas

Ao contrário do Windows, o sistema de arquivos do Linux é sensível a maiúsculas e minúsculas. Isso significa que "Desktop" é diferente de "desktop".

## Diretório

Similar aos "Arquivos" no Windows, são locais onde os arquivos são armazenados.

## Diretório Home

Cada usuário tem seu próprio diretório /home, onde os arquivos que eles criam são salvos por padrão.

## Root

Assim como a maioria dos sistemas operacionais tem um administrador ou superusuário, o Linux possui o "root". Este usuário tem permissões elevadas e pode realizar tarefas como alterar senhas, reconfigurar o sistema e adicionar usuários. No entanto, é importante lembrar que, como disse Tio Ben, "com grandes poderes vêm grandes responsabilidades".

## Scripts

São conjuntos de comandos executáveis em um ambiente interpretativo, que convertem cada linha em código-fonte. Os scripts podem ser executados com o interpretador Bash ou outras linguagens, como Python, uma das mais utilizadas.

## Shell

É um ambiente e tradutor para executar comandos no Linux. O shell mais comumente usado é o Bash.

## Terminal

É a interface de linha de comando (CLI).

---

Para começar, abra o terminal do Kali Linux, que é a interface de linha de comando.

# Sistema de Arquivos do Linux

A estrutura de arquivos do Linux difere um pouco do Windows. O Linux não possui uma unidade física como C:, mas sim um sistema de arquivos lógico. Na raiz do sistema de arquivos está "/", geralmente chamada de raiz do sistema. Com o tempo, isso ficará mais claro, conforme exploramos mais sobre o assunto.

- `/root`: O diretório home do usuário root.
- `/etc`: Contém, geralmente, arquivos de configuração do Linux, que controlam quando e como os programas são iniciados.
- `/home`: Diretório dos usuários.
- `/mnt`: Onde outros sistemas de arquivos são anexados ou montados no sistema de arquivos.
- `/media`: Onde CDs e dispositivos USB são geralmente anexados ou montados.
- `/bin`: Onde residem os binários dos aplicativos (equivalente aos executáveis no Microsoft Windows ou aplicativos no macOS).
- `/lib`: Onde você encontrará as bibliotecas, semelhantes aos DLLs do Windows.

