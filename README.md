# COMEÇANDO DE NOVO
Um repositorio com instrução passo a passo do que devo instalar quando trocar de distro

#Terminal

Vamos instalar o ZSH

```
sudo apt install zsh
```
Vamos definir o zsh como nosso terminal padrão, para isso precisamos editar o arquivo `/etc/passwd`, uma posssivel maneira é com o comando.

```
sudo gedit /etc/passwd
```

Procure pela linha do seu usuário, ela deve estar ao final do arquivo, no meu caso na linha 45, mas o seu pode estar em outra, então olhe com calma.

Reparece que existe uma informação logo ao final da linha **”:/bin/bash"**, tudo o que temos a fazer aqui é trocar a palavra **“bash”** por **“zsh“**. Quando reiniciar as configurações farão efeito.

# Programas

Antes de instalar qualquer programa é bom dar uma atualizada no sistema.

```
sudo apt update; sudo apt upgrade -y
```

## Zoom
https://zoom.us/download

## Slack
https://slack.com/intl/pt-br/downloads/linux

## Chrome
https://www.google.com/intl/pt-BR/chrome/

## VsCode
https://code.visualstudio.com/download

Após concluir o download, vá até ao local do arquivo, clique com o botão direito do mouse e escolha a opção `abrir no terminal`, no terminal digite:
```
sudo dpkg -i <nome-do-arquivo>
```
exemplo
 ```
 sudo dpkg -i code_1.63.2-1639562499_amd64.deb
 ```
 
