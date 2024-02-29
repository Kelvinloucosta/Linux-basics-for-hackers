# Adicionando e removendo Software

Uma das tarefas mais fundamentais no Linux ou em qualquer outro sistema operacional é adicionar e remover software. Alguns programas precisam de outros softwares para funcionar e, às vezes, você descobrirá que pode baixar tudo o que precisa de uma só vez em um pacote de software - um conjunto de arquivos ou bibliotecas, como o chamamos. Normalmente, as bibliotecas e outras dependências necessárias para que um software seja executado com êxito são incluídas. Quando você instala um pacote, todos os arquivos contidos nele são instalados juntos. Existem diferentes métodos para realizar essa tarefa, incluindo o uso do gerenciador de pacotes 'apt', instalação via interface gráfica e o uso do Git para baixar o código-fonte diretamente do repositório.

> **:memo:** Nas distribuições Linux baseadas no Debian, como Kali e Ubuntu, o gerenciador de pacotes padrão é o Advanced Packaging Tool, ou apt. Seu principal comando, apt-get, é usado para baixar e instalar novos pacotes de software, bem como para atualizar e fazer upgrade dos existentes. Embora o apt e o apt-get sejam semelhantes, o último oferece mais funcionalidades, sendo válido aprendê-lo desde o início, apesar da preferência de muitos usuários pelo primeiro.

---

Antes de baixar o pacote, é possível verificar se ele ainda está disponível no repositório, onde são guardadas as informações do sistema operacional.

![apt_search](images/apt-search.png)

Como podemos ver, tudo relacionado à palavra *snort* será exibido.

# Adição de Software

Agora que confirmamos a existência do pacote `snort`, podemos utilizar o apt-get para baixar o software. O `snort` é um sistema de detecção de intrusão de rede open-source amplamente utilizado para monitorar e analisar o tráfego de rede em tempo real. Para instalá-lo, basta executar o seguinte comando no terminal:

![apt_install](images/apt-get_install.png)

# Remocao de Software

Agora para remover basta executar o seguinte comando no terminal:

![apt_remove](images/apt-get_remove.png)

<font color="red">**Quando usamos o comando *remove*, ele não exclui o arquivo de configuração. Isso significa que você pode reinstalar o mesmo pacote sem precisar reconfigurar.**</font>

Para remover o arquivo de configuração e ao mesmo tempo o pacote usamos o comando *purge*.

![purge](images/purge.png)

Para remover dependencias ou bibliotecas que o *SNORT* voce pode remove-las usando o *autoremove*.

![autoremove](images/autoremove.png)

# Atualizando software
Sofwares sao periodicamente atualizados, mas no nosso sistema precisamos aplicar esse *update*, a atualização simplesmente atualiza a lista de pacotes disponíveis para download no repositório.

<font color="red">**Nao confuda *update* com *upgrade*, update simplesmente atualiza a lista de pacotes que estao disponiveis para download no repositorio, enquanto upgrade atualiza o pacote para versao mais recente do repositorio.**</font>

Para *update* sistemas individualmente utilizamos o comand *apt-get* seguido por *update*.

![update](images/update.png)

Agora para *upgrade* os pacotes existentes no seu sistema, usamos o comando *apt-get* seguido por *upgrade*. Esse comando irá atualizar cada pacote no seu sistema que o *apt* conhece.

![update](images/upgrade.png)

# Adicionando repositorios no arquivo sources.list
O servidor que contém o software para uma determinada distribuição do Linux é conhecido como repositórios. Cada distribuicao tem o seu próprio repositorio de software, desenvolvidade para aquela distribuicao, nao funciona muito bem com outras distribuicoes, pois podem ter o mesmo software, mas nao a mesma versao. Embora nao seja recomendado as vezes é necessario adicionar um repositorio como backup, caso nao encontre um programa especifico ele vai para o proximo repositorio, as vezes adicionamos o repositorio do Ubunto no Kali para encontrar algumas ferramentas especificas.

Para adicionarmos o repositorio de uma distribuicao precisamos encontrar o arquivo **sources.list**, que voce pode encontrar no caminho */etc/apt/sources.list*, vamos usar o *leafpad* para abrir esse arquivo.

![repository](images/repository.png)

Algumas distribuicoes dividi os repositorios em categorias, exemplo do Debian:

**main** contém software de código aberto compatível

**universe** contém software de código aberto mantido pela comunidade

**multiverse** contém software restrito por direitos autorais ou outras questões legais

**restricted** contém drivers de dispositivo proprietários

**backports** contém pacotes de versões posteriores








