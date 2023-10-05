## COMANDOS BÁSICOS LINUX

pwd: Mostra o caminho completo do diretório atual.
```
LinuxMint@LinuxMint-D3200:~$ pwd
/home/LinuxMint
```
ls: Lista os arquivos e pastas no diretório atual.
```
LinuxMint@LinuxMint-D3200:~$ ls
'Área de Trabalho'   Imagens     Música   
 Documentos          Público     Vídeos
 Downloads           Modelos     
LinuxMint@LinuxMint-D3200:~$
```
cd: Altera o diretório atual. Por exemplo, cd /pasta o levará para a pasta chamada "pasta".
```
LinuxMint@LinuxMint-D3200:~$ cd
LinuxMint@LinuxMint-D3200:~/home$
```
mkdir: Cria um novo diretório. Por exemplo, mkdir novo_diretorio criará uma pasta chamada "novo_diretorio".

touch: Cria um novo arquivo vazio. Por exemplo, touch arquivo.txt criará um arquivo chamado "arquivo.txt".

cp: Copia arquivos ou diretórios. Por exemplo, cp arquivo.txt destino/ copiará o arquivo "arquivo.txt" para o diretório "destino".

mv: Move ou renomeia arquivos e diretórios. Por exemplo, mv arquivo.txt novo_nome.txt renomeará o arquivo "arquivo.txt" para "novo_nome.txt".

rm: Remove arquivos ou diretórios. Tenha cuidado com este comando, pois é irreversível e pode apagar arquivos importantes. Por exemplo, rm arquivo.txt apagará o arquivo "arquivo.txt".

grep: Procura padrões de texto em arquivos. Por exemplo, grep "texto" arquivo.txt procurará a palavra "texto" no arquivo "arquivo.txt".

chmod: Altera as permissões de um arquivo ou diretório. Por exemplo, chmod 755 arquivo.txt dará permissões de leitura, escrita e execução ao proprietário, e permissões de leitura aos outros usuários.

ps: Mostra os processos em execução no sistema.

kill: Interrompe ou envia sinais para processos em execução. Por exemplo, kill PID interromperá o processo com o ID do processo especificado.

top: Mostra informações em tempo real sobre o uso do sistema e os processos.

df: Mostra informações sobre o espaço em disco disponível nas partições.

free: Mostra informações sobre a memória RAM e o uso de swap.
## COLOCANDO O LINUX COMO PRIORIDADE NO BOOT
 
Para definir o Linux como prioridade no boot usando o Grub Customizer, você pode seguir os seguintes passos:
```
Abra um terminal - ctrl + alt + T
```
 
Edite o arquivo **/etc/default/grub** usando um editor de texto, como o Nano ou o Gedit. Você pode usar o comando abaixo para abrir o arquivo no Nano:
```
sudo nano /etc/default/grub
``` 
Dentro do arquivo **/etc/default/grub,** verifique as linhas **GRUB_DEFAULT e GRUB_SAVEDEFAULT.** Certifique-se de que elas estejam configuradas da seguinte maneira:
```
GRUB_DEFAULT=saved
GRUB_SAVEDEFAULT=true
``` 

Se alguma dessas linhas estiver diferente ou estiver desabilitada com # ou 0, faça as alterações necessárias.

Se as linhas **GRUB_DEFAULT e GRUB_SAVEDEFAULT** não existirem, adicione ao arquivo. 

Após fazer as alterações, salve o arquivo e saia do editor de texto. No Nano, você pode pressionar **Ctrl + O** para salvar e **Ctrl + X** para sair.

Depois, atualize o Grub:
```
sudo update-grub
``` 
 
- Isso atualizará a configuração do Grub e garantirá que o Linux seja definido como a opção padrão no próximo boot.
