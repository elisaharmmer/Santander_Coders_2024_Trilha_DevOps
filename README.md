# Módulo 1: Git e Versionamento
* Este é o 1° módulo da Trilha DevOps ofertado pelo Santander em parceria com a Ada Tech! Nesse módulo, estamos aprendendo sobre Git e Versionamento.
# O que aprendemos até o momento?
* Comandos Básicos de Shell:
```powershell
$ cd
$ ls
```
* O que é Git;

* Repositórios do Git (local e remoto);

* Git branch;

* GitHub;

* Estados do Git:
```powershell
> Tracked;

> Unmodified;

> Modified;

> Staged;

> Untracked;

> Commited.
```
* Comandos do Git:
```powershell
> Git init: Inicializa um novo repositório Git em um diretório. Cria um repositório vazio;

> Git clone: Faz uma cópia de um repositório existente em um novo diretório. É usado para baixar um repositório existente de um servidor remoto;

> Git status: Mostra o estado atual do repositório, incluindo quais arquivos foram modificados, adicionados ou removidos, mas ainda não foram confirmados (committed);

> Git add .: Adiciona todas as mudanças no diretório atual ao próximo commit. Inclui novos arquivos, modificações e exclusões;

> Git diff: Exibe as diferenças entre os arquivos modificados e a última versão confirmada (committed). Ajuda a ver o que foi alterado antes de confirmar;

> Git commit: Salva as mudanças adicionadas ao repositório. É como tirar um "instantâneo" do estado atual do código. Geralmente é acompanhado de uma mensagem de commit para descrever as mudanças;

> Git log: Mostra o histórico de commits do repositório, incluindo mensagens de commit, autor, data e ID dos commits;

> Git restore --staged <arquivo>: Remove o arquivo especificado da área de stage (preparação para commit), mas mantém as mudanças no diretório de trabalho. Útil para desfazer a adição de um arquivo antes do commit;

> Git checkout: Muda para uma outra branch ou restaura arquivos do repositório. Pode ser usado para alternar entre diferentes versões do código;
```