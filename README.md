#wpp-auto

PT-BR
Script simples pra alternar wallpapers no KDE Plasma com base no horario do dia. Compativel com diversas telas.

## Requisitos
- KDE Plasma
- qdbus6 ou qdbus
- Bash

#Estrutura das pastas

-Por padrão, o script espera que os wallpapers estejam dentro de:

~/Imagens/wpp

A organização basica usa duas pastas:

~/Imagens/wpp/
|- d/ #Wallpaper para o periodo do dia
|- n/ #Wallpaper para o periodo da noite

Exemplo:

~/Imagens/wpp/
|- d/
|  |- wallpaper-dia-1.png
|  |- wallpaper-dia-2.jpg
|
|
|- n/
|  |- wallpaper-noite-1.png
   |- wallpaper-noite-2.jpg


Também é possivel usar wallpapers diferentes para cada tela.

A estrutura de pastas então seria:
~/Imagens/wpp/
|---t1/ # Primeira tela
|   |-d/
|   |-n/
|
|---t2/ # Segunda tela
|   |-d/
|   |-n/


## Uso

Dê permissão de execução do script:

 " chmod +x wpp-auto "

e então execute
 " ./wpp-auto "


#Inicialização Automática
 Adicione o script á inicialização automática do KDE PLasma ou crie um serviço de usuário com o comando "systemd"

OBS: O script não inclui wallpapers. Ele apenas procura na pasta configurada e escolhe qual aplicar dependendo da hora.


