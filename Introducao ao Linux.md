# Introdução ao Linux
* _O que é Linux?_

Linux é um sistema operacional de código aberto (Open Source) baseado em Unix, criado por Linus Torvalds em 1991. Ele é amplamente utilizado em servidores, supercomputadores, dispositivos móveis e outros dispositivos, sendo muito conhecido por sua estabilidade, segurança, flexibilidade e capacidade de customização. Além disso, o Linux possui uma grande variedade de distribuições/variações disponíveis para diferentes propósitos e necessidades!

Existem muitas distribuições (distros) de Linux criadas a partir do núcleo do seu código, normalmente chamado de Kernel. Cada distribuição possui seus próprios recursos.

# GUI vs CLI

A grande maioria das distribuições Linux incluem uma GUI (Graphic User Interface) como opção de interface de navegação no sistema operacional, permitindo que os usuários possam utilizá-lo de forma mais amigável e intuitiva.
Alternativamente, as mesmas funcionalidades disponíveis na GUI também estão disponíveis através da execução de comandos utilizando sua CLI (Command Line Interface), a famosa "tela preta".

# Terminal/Bash

* Principais comandos:

```sh
> cat: Mostra conteúdos presentes em arquivos de determinada pasta no Linux.
Exemplo de uso: "cat /etc/issue".
```
```sh
> pwd: Mostra em qual diretório você se encontra.
```
```sh
> whoami: Comando utilizado para mostrar qual é o usuário ativo no momento.
```
```sh
> cd  <nome do diretório>: Ir de um diretório para outro diretório.
```
```sh
> cd ~: Ir para a minha home.
```
```sh
> cd -: Retorna para o diretório anterior, mesmo que você não saiba o nome dele.
```
```sh
> cd ..: Retorna para o diretório anterior (chamado de "Caminho Relativo").
```
```sh
> ls: Listar o nome de pastas e diretórios no diretório atual.
```
```sh
> ls -l: Listar pastas e diretórios com informações detalhadas, tais como permissões, tamanho, grupo, etc.
```
```sh
> ls --help: Trazer o manual de como utilizar parâmetros no Linux.
```
```sh
> rmdir: Remover (excluir) diretórios vazios no Linux.
```
```sh
> .: Diretório que você está no momento atual.
```

# Identificando e criando arquivos e diretórios
``` 
> Quando o primeiro caractere for um "-" (hífen), significa que é um arquivo qualquer.
> Quando a primeira letra é "d", significa que é um diretório.
```
* O comando 'touch <nome do arquivo>' cria qualquer tipo de arquivo.

* O comando 'mkdir  <nome do diretório>' cria um diretório. Para criar uma árvore de diretórios, existe o parâmetro 'mkdir "-p"'. Utiliza-se o comando 'tree' para mostrar de forma ordenada e organizada os diretórios que foram criados.

# Movendo e apagando arquivos e diretórios

* _Como mover um arquivo para um diretório?_
```sh
'mv (de "move", em Inglês) <nome do arquivo> <nome do diretório>'
```

* _Como copiar um arquivo?_
```sh
'cp <nome do diretório>/<nome do arquivo>' . 
```

* _Como renomear um arquivo?_
```sh
'mv <nome do arquivo> <novo nome do arquivo>
```
* _Como remover um arquivo?_
```sh
'rm <nome do arquivo>'

OBSERVAÇÃO: Ao remover arquivos no Linux utilizando o terminal, não é possível restaurá-lo! Tome muito cuidado com este comando e utilize-o com cautela.
```
* _Como remover um diretório?_
```sh
Para remover um diretório, é necessário utilizar os seguintes parâmetros:

'rm -d <nome do diretório>': Remove um diretório que encontra-se vazio.

'rm -r <nome do diretório>': Remove um diretório que contém outros diretórios e todo o seu conteúdo.
```

# Instalando Programas
```sh
> 'sudo apt-get update': Atualiza a lista de pacotes disponíveis.

> 'sudo apt-get install < nome do programa >': Instala o programa especificado.
```
# Edição e Editores de Textos
* _Quais são os principais editores?_
```sh
> vi
```
```sh
> vim
```
```sh
> nano
```
* Comandos Básicos no vim:
```
:w = salvar o progresso
:quit = sair do editor de texto
```