 
## COLOCANDO O LINUX COMO PRIORIDADE NO BOOT
 
Para definir o Linux como prioridade no boot usando o Grub Customizer, você pode seguir os seguintes passos:

- **Abra um terminal.**

Edite o arquivo **/etc/default/grub** usando um editor de texto, como o Nano ou o Gedit. Você pode usar o comando abaixo para abrir o arquivo no Nano:

- **sudo nano /etc/default/grub**

Dentro do arquivo **/etc/default/grub,** verifique as linhas **GRUB_DEFAULT e GRUB_SAVEDEFAULT.** Certifique-se de que elas estejam configuradas da seguinte maneira:

- **GRUB_DEFAULT=saved**
- **GRUB_SAVEDEFAULT=true**

Se alguma dessas linhas estiver diferente ou estiver desabilitada com # ou 0, faça as alterações necessárias.

Se as linhas **GRUB_DEFAULT e GRUB_SAVEDEFAULT** não existirem, adicione ao arquivo. 

Após fazer as alterações, salve o arquivo e saia do editor de texto. No Nano, você pode pressionar **Ctrl + O** para salvar e **Ctrl + X** para sair.

Depois, atualize o Grub:
 
- **sudo update-grub**

- Isso atualizará a configuração do Grub e garantirá que o Linux seja definido como a opção padrão no próximo boot.
