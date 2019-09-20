# Instalação do Minix3 com Interface Gráfica

Relatório da Instalação do Sistema Operacional Minix3 para a disciplina de Laboratório de Sistemas Operacionais do Curso de Ciência da Computação da Universidade Tecnológica do Paraná (UTFPR-MD)

## 1. Imagem do MINIX
Para realizar a atividade de instalar o MINIX3 eu fiz uma pesquisa no [site do do minix](http://www.minix.org) onde está disponível a versão estável 3.3.0 para download. Porém como eu preciso de uma iso com interface gráfica, havia uma observação que dizia que a versão 3.4.0 vinha o Xorg instalado e configurado. Então pesquisando nos repositórios achei as [imagem do MINIX 3.4.0](http://download.minix3.org/iso/snapshot/). Então fiz o download da versão 3.4.0rc6.

## 2. Configuração do Ambiente de Virtualização
Inicialmente o SO MINIX3 foi feito para rodar em uma máquina física e real, ou seja, não virtualizada. Mas como eu não disponho de uma máquina física a qualquer momento para fazer isso, eu preferi seguir usando o [Oracle VM VirtualBox](https://www.virtualbox.org). Olhando a [documentação](https://wiki.minix3.org/doku.php?id=usersguide:runningonvirtualbox), configurei o VirtualBox.

![Figura 1 - Criar máquina virtual 1](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-01.png)

![Figura 2 - Criar máquina virtual 2](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-02.png)

![Figura 3 - Criar máquina virtual 3](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-03.png)

![Figura 4 - Criar máquina virtual 4](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-04.png)

![Figura 5 - Criar máquina virtual 5](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-05.png)

![Figura 6 - Criar máquina virtual 6](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-06.png)

![Figura 7 - Criar máquina virtual 7](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-07.png)

Para não ter problemas com a hora errada, irei habilitar fornecer o horário por UTC:
![Figura 8 - Configurar UTC](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-08.png)

![Figura 9 - Configurar UTC](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-09.png)

![Figura 10 - Configurar UTC](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-10.png)

![Figura 11 - Configurar UTC](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-11.png)

## 3. Instalação básica do sistema


Após feita as configurações básicas, iremos começar a Instalação. Por isso iniciemos a máquina virtual:
![Figura 12 - Iniciar a máquina virtual](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-12.png)

Ao aparecer essa tela, o virtualbox pede para adicionar uma imagem do sistema operacional. Então adicinemos a ISO [Minix 3.4rc6](http://download.minix3.org/iso/snapshot/minix_R3.4.0rc6-d5e4fc0.iso.bz2).

![Figura 13 - Iniciar a máquina virtual](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-14.png)

![Figura 14 - Iniciar a máquina virtual](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-15.png)

![Figura 15 - Iniciar a máquina virtual](https://raw.githubusercontent.com/felipebeskow/Minix-LSO/master/Imagens/0%20-%20Configura%C3%A7%C3%A3o-VirtualBox-16.png)

Após isso iremos iniciar a máquina virtual e ela irá dar o boot pela ISO. A primeira tela que aparecerá será a abaixo, apenas aperte enter:
![Figura 16 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2001.png)

Fazemos o login no usuário root. Não precisa de senha:
![Figura 17 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2002.png)

Logo você estara logado como root:
![Figura 18 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2003.png)

Entre com o comando setup para começar a instalação:
![Figura 19 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2004.png)

O resto da instação será apenas seguindo o default:
![Figura 21 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2005.png)
![Figura 22 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2006.png)
![Figura 23 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2007.png)
![Figura 24 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2008.png)
![Figura 25 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2009.png)
![Figura 26 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2010.png)
![Figura 27 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2011.png)
![Figura 28 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2012.png)
![Figura 29 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2013.png)
![Figura 30 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2014.png)
![Figura 31 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2015.png)
![Figura 32 - Instalação do Minix](https://github.com/felipebeskow/Minix-LSO/raw/master/Imagens/1%20-%20Instala%C3%A7%C3%A3o%20Minix%20-%2016.png)

https://sempreupdate.com.br/minix-veja-como-instalar-em-u/