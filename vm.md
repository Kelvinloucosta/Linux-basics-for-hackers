# Virtual Machine

Vamos usar o VirtualBox para configurar o Kali Linux em uma máquina virtual.

1. Acesse [o site do VirtualBox](https://www.virtualbox.org/) e faça o download do programa.
2. Siga as instruções de instalação, clicando em "Next" até concluir a instalação, sem a necessidade de fazer alterações.
3. No VirtualBox, clique em "New", dê um nome para sua máquina virtual, escolha onde ela será armazenada e selecione "Linux" como tipo e "Debian (64-bit)" como versão.
4. Atribua memória à sua máquina virtual, mas não ultrapasse 25% da sua RAM total.
5. Escolha o tamanho do disco rígido, recomendamos entre 20-25 GB se não optar pelo modo "Dynamically Allocated".
6. Clique em "Create".

# Instalando o Kali na VM

1. Clique em "Start" para iniciar a máquina virtual.
2. O VirtualBox solicitará o local da imagem de inicialização. Selecione a ISO do Kali Linux que você baixou.
3. A máquina virtual reiniciará e a instalação do Kali começará. Recomendamos escolher a opção "Graphical Install" para iniciantes.
4. Se ocorrer algum erro, verifique se a virtualização está ativada na BIOS do seu computador e desative qualquer outro software de virtualização concorrente, como o Hyper-V.
5. Selecione a linguagem, localização e layout do teclado, depois prossiga com a instalação.
6. Defina um nome para sua máquina, deixe o campo de nome de domínio em branco e crie um usuário não-root com uma senha.
7. Na parte de particionamento de disco, escolha "Guided - use entire disk" para uma instalação mais simples.
8. Confirme a seleção e aguarde a instalação do Kali.
9. Quando solicitado sobre o uso de um mirror de rede, selecione "No".
10. Opte por instalar o GRUB quando perguntado, para facilitar a inicialização de outros sistemas operacionais.
11. Selecione a opção de instalar o GRUB automaticamente para evitar problemas de travamento.
12. Após a instalação, sua máquina virtual reiniciará e o Kali estará pronto para uso.
13. Se estiver usando Kali 2020 ou posterior, lembre-se de usar o comando `sudo` antes de qualquer comando.

