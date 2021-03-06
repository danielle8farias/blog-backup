# Instalando, configurando e inicializando o Git no Linux


Para instalar o Git no Linux, digite no terminal:

```
$ sudo apt install git
```

- o símbolo **$** indica que você deve usar o **usuário comum** para fazer essa operação.

- o **sudo** é o comando que dá permissões de super usuário temporariamente; assim é possível fazer a instalação de programas.

- o **apt** do inglês, *Advanced Package Tool*, em português, Ferramenta de Empacotamento Avançada; é a ferramenta que nos ajuda na instalação, atualização e desinstalação de programas, entre outras funções.

- o **install** é o comando de instalar, indicando ao apt o que fazer.

Verifique se a instalação foi feita corretamente digitando:

```
$ git --version
```

Você receberá o retorno da versão instalada.

Antes de começar a usá-lo é preciso fazer as configurações iniciais. Assim,

```
$ git config --global user.name seu_nome_aqui
```

Insira seu nome no local marcado; *seu_nome_aqui*.

Em seguida:

```
$ git config --global user.email seu@email.com
```

Insira seu email no local marcado; *seu@email.com*.

Configurando o editor padrão:

```
$ git config --global core.editor nano
```

No meu caso, estou usando o **nano**.

Para verificar as suas configurações:

```
$ git config --list
```

Caso queira que as configurações sejam feitas apenas no diretório (não global) indicado, basta retirar dos comandos a flag **--global**. Assim:

```
$ git config user.name seu_nome_aqui
$ git config user.email seu@email.com
$ git config core.editor nano
```

Para inicializar o git no diretório desejado (caso ainda não o tenha feito), vá até o local onde você deseja fazer o controle de versionamento.

```
$ cd /home/seu_usuário/seu_repositório
```

- o comando **cd** serve para mudar de diretório/pasta; em seguida digite o caminho até a pasta.

e digite

```
$ git init
```

A partir de agora, os arquivos serão rastreados pelo **Git**.

tags: git, linux, configuracao, instalacao
