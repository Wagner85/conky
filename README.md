Como instalar o Conky
O Conky está incluso no repositório padrão do Ubuntu, portanto, instalá-lo é muito fácil. Basta abrir uma janela de terminal e executar o seguinte comando:

$ sudo apt install conky-all
Uma vez instalado, você deve rodar o Conky pelo terminal:

$ conky
Por padrão, o Conky exibe informações em uma janela própria e bem sem graça. Agora você pode pressionar CTRL + C no terminal para parar o Conky.

Como configurar o Conky manualmente
Para alterar a aparência da Conky em sua área de trabalho, você pode editar o arquivo de configuração do sistema no local:

/etc/conky/conky.conf
Uma abordagem mais segura é criar um arquivo de configuração Conky específico do usuário no diretório inicial:

 ~/.conkyrc
Você pode usar o /etc/conky/conky.conf como um modelo para sua configuração específica do usuário copiando seu conteúdo.

cp /etc/conky/conky.conf ~/.conkyrc
A partir deste arquivo você pode efetuar as configurações manualmente.

Conky Manager ao resgate
Configurar o Conky manualmente não é a melhor tarefa que você gostaria de fazer. Em vez disso, você pode rapidamente obter um bonito Conky em sua área de trabalho com o Conky Manager.
Para instalar o Conky Manager no Ubuntu 16.04, use os seguintes comandos.

$ sudo apt-add-repository -y ppa:teejee2008/ppa
$ sudo apt update
$ sudo apt install conky-manager
O PPA acima não suporta o Ubuntu 17.04 ainda. Se você usar o PPA acima no Ubuntu 17.04, você verá o seguinte erro:

unable to locate package conky-manager
Os usuários do Ubuntu 17.04 podem baixar o arquivo .deb do Conky Manager.

64 bit
$ wget https://launchpad.net/~teejee2008/+archive/ubuntu/ppa/+files/conky-manager_2.4~136~ubuntu16.04.1_amd64.deb
 

32 bit
$ wget https://launchpad.net/~teejee2008/+archive/ubuntu/ppa/+files/conky-manager_2.4~136~ubuntu16.04.1_i386.deb
Em seguida, instale-o com gdebi, que manipulará automaticamente dependências de pacotes.

$ sudo apt install gdebi
$ sudo gdebi conky-manager*.deb
Uma vez instalado, inicie-o no Unity Dash ou no menu da sua aplicação.
conky




# conky
Custom Desktop Utility

OPEN .conkyrc FILE AND CHANGE ETH ADP, WIFI ADP and HOME location, accordingly!
DO CUSTOMIZE BEFORE USING IT
$ cd conky
$ cp -r ./* ~/

Execute Conky
$ conky -c ~/.conkyrc
$ conky
