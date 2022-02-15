# COMEÇANDO DE NOVO
Um repositório com instrução passo a passo do que devo instalar quando trocar de distro.

> OBS: Considerando que meu `/home` está em uma partição separada e compartilhada entre as distros, apenas as configurações abaixo são necessárias.

# Terminal

### Vamos instalar o ZSH

```
sudo apt install zsh
```
Vamos definir o zsh como nosso terminal padrão, para isso precisamos editar o arquivo `/etc/passwd`, uma posssivel maneira é com o comando.

```
sudo gedit /etc/passwd
```

Procure pela linha do seu usuário, ela deve estar ao final do arquivo, no meu caso na linha 45, mas o seu pode estar em outra, então olhe com calma.

Reparece que existe uma informação logo ao final da linha **”:/bin/bash"**, tudo o que temos a fazer aqui é trocar a palavra **“bash”** por **“zsh“**. Quando reiniciar as configurações farão efeito.

### Instalando o LSD (LSDeluxe)

[Esse](https://github.com/Peltoche/lsd#configuration) é o repositório do **LSD**. E [nesse link](https://github.com/Peltoche/lsd/releases) estão as versões para download. Se estiver no Ubuntu ou em uma distro derivada dele procure por algo que se pareça com `lsd-musl_0.20.1_amd64.deb`.

Apos fazer o download executar o seguinte comando de terminal no local onde o arquivo foi baixado.\
`sudo dpkg -i <nome-do-arquivo>`.

Exemplo:
```
sudo dpkg -i lsd-musl_0.20.1_amd64.deb
```

Pronto, os comando do lsd já estarão funcionando.

# Git e GitHub

Siga esse repo https://github.com/duribeiro/Git-GitHub-config#gerando-uma-nova-chave-ssh

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

# Node com NVM

Baixando o repositório e instalando o nvm

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

> Feche o terminal e abra novamente antes de continuar.

Instalando o Node na ultima versão estável LTS

```
nvm install --lts
```
