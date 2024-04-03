--------------LINUX------------------- 
- $ sudo - root
- $ / - diretorio
- $ cd - acessar diretorio (cd /pasta)
- $ mkdir - {novo diredorio}
- $ dir - mostra diretórios
- $ touch - {novo file.txt}
- $ clear - limpa o terminal
- $ exit - sai do terminal
- $ w - Mostra quem está conectado e o que está fazendo.
- $ watis - Mostra um resumo sobre um ou mais comandos.
- $ mv - renomeia/move file ou diretorios
- $ pwd - diretório atual
- $ ls - Listar arquivos
- $ ls -l - Lista os arquivos e diretórios no diretório atual
- $ cal - calendario
- $ cat teste.txt (Lista dados do Arquivo)
- $ date - data e hora
- $ nano - para abrir arquivo file
- $ htop - sistema e os processos
- $ kill - matar processos em execução
- $ ps - mostrar processos em execução
- $ who - informa quais os usuários que estão conectados.
- $ xman - aplicativo gráfico de exibição da documentação do Linux.
- $ chmod - permissões de um arquivo ou diretório [chmod 755 arquivo.txt {vira root}]
- $ grep - grep "texto" arquivo.txt procurará a palavra "texto" no arquivo "arquivo.txt".
- $ df: Mostra informações sobre o espaço em disco disponível nas partições.
- $ df: Mostra informações sobre o espaço em disco disponível nas partições.
- $ man - manual linux
- $ help - use help para encontrar algum comando não listado
- $ hostname - exibe nome da máquina
- $ history - exibe os comando digitados pelo usuário.
- $ last - exibe todas as informações referentes a entrada (login) e saída (logout) de usuários do sistema.
  
 --------------REDE LINUX------------------- 
- $ ping www.google.com
- $ ping -a
- $ ipconfig
- $ ipconfig -a
- $ nbtscan 192.168.1.1 - Descobrir o hostname do IP.
  
--------------TOR-------------------
- $ service tor start
- $ service tor status
- $ service tor stop
- $ proxychains firefox
  
--------------SHUTDOWN------------------- 
- $ shutdown -h now
- $ shutdown -h 21:55
- $ shutdown -h +45
- $ shutdown -c
- $ shutdown now

--------------/etc----------------------------------
- cd /etc/  - nano hosts [127.0.0.1       localhost]

--------------/CAL---------------------------------- 
- $ expr 2 + 8 #comEspaçosEntreAsSomas
- echo"(9 + 3) * 5" | bc - resultado (25)
- passwd @seuUsuario (Nova senha)
  
--------------USER------------------- 
Adicionar e Remover Usuários
-sudo adduser [newuser]
-sudo userdel -r [user]
