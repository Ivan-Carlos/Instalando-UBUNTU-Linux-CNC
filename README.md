# Instalando-UBUNTU-Linux-CNC.
Objetivo é fazer uma instalação do Ubuntu Linux extremamente compacta,  Com a versão correta e com a imagem apropriada do kernel,  para o  Linux CNC.

# CONSIDERAÇÕES INICIAIS: 
- Objetivo deste post, é fazer uma instalação do Linux extremamente compacta,
- Utilizando imagem i386, pois amd64 não é suportada pelo kernel do linuxcnc.
- Porém você poderá utilzar um kernel do proprio linux (rt-amd64).
- Sem a necessidade de instalar pacotes e depois subtrai-los, já com versão correta e com a imagem apropriada para kernel do LinuxCNC. 

# PRÉ REQUISITOS:
- Um pendriver 2 GB.
- Um PC. (pode ser uma máquina mais antiga,com boot para pendriver), com uma HD (formatada). de 10 GB. Placa de rede, uma entrada USB e porta paralela (COM).
- Acesso a Internet. 

# TRABALHOS INICIAIS.
- Baixe o Ubuntu
- O LinuxCNC será executado na versão do Ubuntu Precise-(i386). Você pode baixar aqui:
http://old-releases.ubuntu.com/ubuntu/dists/precise/main/installer-i386/current/images/netboot/mini.iso
- Crie uma unidade USB inicializável.
- Baixe Rufus, para a criação de pendrives USB inicializáveis.  Rufus é um excelente utilitário para a criação de pendrives USB. inicializáveis. Não requer instalação: https://rufus.akeo.ie/
- Selecione um pendrive USB de 2 Gb ou maior. Todas as informações nele contidas serão sobrescritas

![rufus](images/rufus.PNG)

# INICIANDO A INSTALAÇÃO.
- Apos instalar o pendriver com o boot , espete o em uma unidade USB  no  PC que será instalado o Linuxcnc, e de o boot na maquina, e inicie a instalação.
- Utilize a opção => Adavances Options = Comannd line expert install
- Primeira tela:

![Ubuntu](images/Ubuntu.PNG)
- Selecione o idioma de sua preferência:
- Segunda tela:
![Linguagen](images/Linguagen.PNG)
- Terceira tela:
![Linguagen_1](images/Linguagen_1.PNG)
- Quarta tela:
![Linguagen_2](images/Linguagen_2.PNG)
- Quinta tela:
![Linguagen_3](images/Linguagen_3.PNG)
- Sexta tela:
![Linguagen_4](images/Linguagen_4.PNG)
- Sétima tela:
![Linguagen_5](images/Linguagen_5.PNG)
- Oitava tela:
![Linguagen_6](images/Linguagen_6.PNG)
- Nona tela:
![Linguagen_7](images/Linguagen_7.PNG)
- Selecione o "layout" do teclado:
- Décima tela:
![keyboard](images/keyboard.PNG)
- Décima primeira tela:
![keyboard1](images/keyboard1.PNG)
- Décima segunda tela:
![keyboard2](images/keyboard2.PNG)
- Décima terceira tela:
![keyboard3](images/keyboard3.PNG)
- Localização de componentes da rede.
- Décima quarta tela:
![Network](images/Network.PNG)
- Descomente.
- Décima quinta tela:
![Network_1](images/Network_1.PNG)
- Configurando a rede.
- Décima sexta tela
![Network_2](images/Network_2.PNG)
- Seguramente você poderá utilizar a opção "yes" que o Linux configurará a rede automaticamente.
- Mas se você gosta de um desafio!
- Décima sétima tela:
![Network_3-5](images/Network_3-5.PNG)
- Pesquise com antecedência o número do IP do seu roteador, Servidores DNS IPv4.
- Este numero vocé poderá encontrar no Windows na barra status da rede, configurações, Servidores DNS IPv4: 192.168.2.1
- Crie o gatewai de sua máquina Linux:
- Copíe as tres primeiras faixas, invente um na quarta  faixa.
- Obs: Não utilize "1" que é o número do seu roteador, não utilize, o mesmo número da máquina Windons!

- Décima oitava tela
![Network_4](images/Network_4.PNG)
- A máscara de rede poderá ser a mesma sugerida pelo Linux.
- No caso da imagem:
- Décima nona tela
![Network_5](images/Network_5.PNG)
- Deixe como aparecer, que estará correto!
- Vigéssima  tela:
![Network_6](images/Network_6.PNG)
- Deixe como aparecer, que estará correto!
- Vigéssima primeira tela:
![Network_7](images/Network_7.PNG)
- Confira e confirme:
- Vigéssima segunda tela:
![Network_8](images/Network_8.PNG)
- De um nome para sua máquina:
- Vigéssima terceira tela:
![Hosts](images/Hosts.PNG)
- Deixe em branco:
- Vigéssima quarta tela.
![Hosts_1](images/Hosts_1.PNG)
- Procurando provedor Linux.
- Vigéssima quinta tela:
![Provedor](images/Provedor.PNG)
- Vigéssima sexta tela
![Provedor1](images/Provedor1.PNG)
- Selecione o país
- Vigéssima sétima tela
![Provedor2](images/Provedor2.PNG)
- De enter:
- Vigéssima oitava tela:
![Provedor3](images/Provedor3.PNG)
- Deixe em branco.
- Vigéssima nona tela:
![Provedor4](images/Provedor4.PNG)
- Começando a  baixar os pacotes.
- Trigéssima tela
![Componentes](images/Componentes.PNG)
- Deixe em branco.
- Trigéssima primeira tela
![Componentes1](images/Componentes1.PNG)
- Trigéssima segunda tela:
![Componentes2](images/Componentes2.PNG)
- Pular configuração de senhas. 
- Configurar o relógio.
- Trigéssima terceira tela
![horas](images/horas.PNG)
- Trigéssima quarta tela:
![horas1](images/horas1.PNG)
- Trigéssima quinta tela:
![horas2](images/horas2.PNG)
- Trigéssima sexta tela:
![horas3](images/horas3.PNG)
- Detectando os díscos:
- Trigéssima sétima tela:
![Discos0](images/Discos0.PNG)
- Trigéssima oitava tela:
![Discos1](images/Discos1.PNG)
- Descomente.
- Trigéssima nona tela:
![Discos2](images/Discos2.PNG)
- Particionar o disco.
- Quadragéssima tela:
![Discos](images/Discos.PNG)
- Se a HD. foi formatada aparerá assim.
- Selecione o modo guiado.
- Quadragéssima primeira tela:
![Discos3](images/Discos3.PNG)
- Quadragéssima segunda tela:
![Discos4](images/Discos4.PNG)
- Escolha este modo proposto, que é o mais simples.
- Quadragéssima terceira tela:
![Discos5](images/Discos5.PNG)
- Confirme as mudanças.
- Quadragéssima quarta tela:
![Discos6](images/Discos6.PNG)
- Quando aparecer esta tela,  vamos dar "O Pulo do gato"
- Apertar  as  teclas ctrl+alt+F2
- Quadragéssima quinta tela
![Final](images/Final.PNG)
- Neste ponto, estamos com a partição /dev/sda1 montada em /target,

      mount -t ext4 -o rw /dev/sda1 /mnt/
- A onde iremos propriamente instalar o linux.
- Quadragéssima sexta tela:
![Pulodogato](images/Pulodogato.PNG)
- Tecle: 
- ~# cd /target
- ~# apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6
- ~# apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 04EE7237B7D453EC
- ~# apt-get update
- ~# debootstrap --variant=minbase precise /target
- ~# mount -v --bind /dev  /target/dev
- ~# chroot /target /bin/bash
- ~# mount -vt tmpfs none /run
- ~# mount -vt proc none proc
- ~# mount -vt sysfs none /sys
- ~# mount -vt devpts devpts /dev/pts
- ~# mount -vt tmpfs none /tmp
- ~# export LC_ALL=C
- ~# apt-get update
- ~# apt-get install --no-install-recommends nano
- ~# nano /etc/apt/sources.list
- Edite sources.list com está fig

![sources](images/sources.PNG)
- Salve a edição: 
- Ctrl+x
- Y+enter
- Obs: o passo anterior, não poderá dar "erro", se houver algum erro, corriga novamente o arquivo editado.
- ~# apt-get update
- ~#  apt-get install --no-install-recommends netbase
- ~# apt-get install --no-install-recommends apt-utils dialog
- ~# apt-get install --no-install-recommends iputils-ping
- ~# apt-get install --no-install-recommends apt-file
- ~# apt-file update
- ~# apt-file search bin/ifconfig
- ~# apt-get install --no-install-recommends net-tools
- ~# apt-get install --no-install-recommends ifupdown
- ~# apt-get install --no-install-recommends isc-dhcp-client
- ~# apt-get install --no-install-recommends network-manager
- Edite /etc/hosts
- ~# nano /etc/hosts
- 127.0.0.1 localhost
- 127.0.1.1 Linux-cnc
- ctrl + x
- y + enter
- ~# apt-get install --no-install-recommends sudo
- ~# adduser user
- ~# password config
- ~# password confirm
- Full Name [ ]: user
- Room Number [ ]: enter
- Work Phone [ ]: enter
- Home Phone [ ]: enter
- Other [ ]: enter
- Is the information correct [Y/n}: y
- ~#  apt-get autoclean
- ~# usermod -a -G sudo user
- ~#  groups user
- O arquivo /etc/fstab deverá estar como na fig. abaixo.
- ~# cat /etc/fstab
- Obs: a numeração UUID aparecerá com outro valor  
![fstab](images/fstab.PNG)
- Atenção:
- Se deu tudo certo no começo, você pode pular esta parte da edição do fstab.
- ~# blkid > /etc/fstab
- ~# nano /etc/fstab
- proc	/proc	proc	nodev,noexec,nosuid	0	0 	
- #/dev/sda1
- UUID=************************** /ext4 errors=remount-ro 0 1
- #/dev/sda2
- UUID=**************************** none swap sw 0 0
- ctrl + x
- y + enter
- Lembre-se:  Não edite os valores da UUID, eles são únicos. se o fstab não estiver todo correto, pode causar problemas na sua inicialização.
- Continua........
- Instalando as chaves.
- ~# apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-key 3cb9fd148f374fef

![key](images/key.PNG)
- Edite /etc/apt/sources.list
- Acrecente a linha no fim do arquivo e salve.
- ~# nano /etc/apt/sources.list
- deb http://linuxcnc.org/ precise base 2.7-rtai
- deb-src http://linuxcnc.org/ precise base 2.7-rtai
- ctrl + x
- y + enter

![sources1](images/sources1.PNG)
- ~# apt-get update
- ~# apt-get install --no-install-recommends initramfs-tools linux-image-3.4-9-rtai-686-pae rtai-modules-3.4-9-rtai-686-pae grub-pc

![grub](images/grub.PNG)

- ~# uname -r

![uname](images/uname.PNG)
- ~#  passwd
- Enter new UNIX password:
- Retype  new UNIX password:
- ~# exit
- ~# cd /
- ~# umount -lfv /target 
- ~# shutdown -r  now
- Reinicie a máquina!
- ~# apt-get install xfce4 synaptic linux-firmware

![xfve41](images/xfce41.PNG)
- 
![xfve42](images/xfce42.PNG)
- 
![xfve43](images/xfce43.PNG)
- 
![xfve44](images/xfce44.PNG)

- ~# shutdown -r  now
- Reinicie a máquina!
- ~# startx

![xfce4](images/xfce4.PNG)
- Abra o synaptic
- Instale o linuxcnc

![linuxcnc](images/linuxcnc.PNG)
- Instale o leafpad

![leafpad](images/leafpad.PNG)

![latency](images/latency.PNG)
# EXTRA
- Se você tiver problemas para carregar "parport".
- Abra promt de comando, tecle: lsmod
- Procure por "parport".

![lsmod](images/lsmod.PNG)

- Se não estiver carregado, "parport". tente editar /etc/rc.local como na fig. a baixo.
- Reinicie a máquina!

![rclocal](images/rclocal.PNG)
- Não menos importante!
- Abra o CNC => Stepconf Wizart
- Na aba certa edite como está na fig.abaixo!(porta paralela COM1)
![stepper](images/stepper.PNG)
- Pinagem (out/in) porta paralela:

![paralela](images/paralela.PNG)

#EXTRA DO EXTRA
- Outro método de instalar a interface gráfica no lugar do xfce4 é com o icewm, 
- Eu o chamo de "método autoflagelação":
- ~# apt-get install xinit icewm linuxcnc gedit nautilus linux-firmware
- Acesse o patinho fe..digo o sistema gráfico.
- ~# startx
- Abra com o gedit o arquivo /etc/X11/icewm/programs
- Edite o arquivo como na figura a baixo:

![menu](images/menu.PNG)
- Se tudo correr direito o resultado será este:

![icewm](images/icewm.PNG)
- Com o editor aberto edite também
- /etc/shadow
- A linha do root e deixe assim:

![shadow](images/shadow.PNG)
- Edite também rc.local e acressente
- Uma linha como na figura abaixo

![rclocal1](images/rclocal1.PNG)
- Reinicie a maquina

Data do post: 05-06-2019

# AVISO LEGAL
- OS AUTORES DESTE SOFTWARE NÃO ACEITAM ABSOLUTAMENTE A RESPONSABILIDADE POR QUAISQUER DANOS OU PERDAS RESULTANTES DE SEU USO.
- É EXTREMAMENTE NÃO CONFIAR EM SOFTWARE APENAS POR SEGURANÇA.

- Qualquer maquinário capaz de ferir pessoas deve ter provisões para remover completamente a energia de todos os motores, etc, antes que as pessoas entrem em qualquer área de perigo.
- Todas as máquinas devem ser projetadas para estar em conformidade com os códigos de segurança locais e nacionais, e os autores deste software não podem, e não assumem, qualquer responsabilidade por tal conformidade.
- Este software é lançado sob a GPLv2, com algumas partes sob a LGPL. Veja o arquivo COPYING para mais detalhes.
Instalando-UBUNTU-Linux-CNC


