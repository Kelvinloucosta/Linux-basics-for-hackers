# Virtual Machine

Vamos utilizar o Virtual Box para usar o Kali Linux.

1 - Acesse https://www.virtualbox.org/ e faça o download do Virtual Box.
2 - Clique em Next ate instalar o programa, nao precisa alterar nada.
3 - Clique em "New", dê o nome para sua maquina, escolha onde será hospedada e escolha Linux e depois Debian 64 Bits.
4 - Aloca sua memoria, nao recomendo mais do que 25% da sua RAM total.
5 - Tamanho do disco, recomendo entre 20-25 GB se voce nao escolher o modo Dynamically Allocated.
6 - Clique em Create.

# Instalar Kali na VM 

1 - Clique em "Start"
2 - O Virtual Box irá te perguntar onde encontrar o disco de inicialização, como ja fizemos o download da .ISO buscaremos essa imagem.
3 - A maquina irá reiniciar e aparecer a parte da instalaçao do Kali, sugiro istalar o Graphical Install para iniciantes.
4 - Caso dê algum erro pode ser que sua maquina nao esteja com Virtualização ativa na BIOS. Alem disso você provavelmente precisará desativar qualquer software de virtualização concorrente, como o Hyper-V.
5 - Com isso confirmado, irá te perguntar qual linguagem utilizar, recomendo sempre Ingles, localização e Keyboard, depois disso irá iniciar a instalação.
6 - De o nome ao seu host, Domain Name deixe em branco, voce precisará criar um user non-root, escolha de sua preferencia e depois a senha.
7 - partition disk, como estamos utilizando uma virtual machine escolha "Guided use entire disk" ira receber um aviso que o disco será apagado, clique em continue.
8 - Kali irá te perguntar se voce quer tudo em uma unica partição, como isso é lab, escolheremos essa opcao.
9 - Seleciona "YES" para confirmar a alteração.
10 - Clique em Next, para instalar as ferramentas.
11 - Kali demora um tempo para instalar.
12 - Depois, será perguntado se você deseja usar um network mirror. Clica em "No"
13 - Depois, será perguntado se você deseja instalar o GRUB, para caso voce queira selecionar outro SO ao iniciar. Clica em "Yes"
14 - Na proxima pagina, será perguntado se você deseja instalar o GRUB automatically ou Manually, se escolher Manualmente O Kali tende a travar e exibir uma tela em branco após a instalação, selecione o drive onde o GRUB bootloader será instalado, provavelmente será algo como /dev/sda, clique em continue e pronto o Kali foi instalado.
15 - Se voce estiver usando Kali 2020 ou posterior, voce precisará usar o comando sudo antes de qualquer comando.