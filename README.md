**Comandos Essenciais do Git**

### Uma Introdução ao GIT - *Staging Area*

Quando se deseja começar uma nova versão, não se edita um arquivo e imediatamente ele é registrado. É possível, inclusive, registrar somente certos arquivos na nova versão, deixando de lado outros arquivos modificados. A *staging area* é o conjunto de arquivos cujas mudanças serão incluídas na nova versão.

Na janela de tempo entre uma versão e outra, os arquivos podem estar em quatro estados. Estes são:

- Não-modificado (*unmodified*) → Arquivos neste estado estão na versão atual (*HEAD*) e não foram alterados.
- Modificado (*modified*) → Arquivos neste estado estão na versão atual (*HEAD*), foram alterados, mas não constarão na próxima versão.
- Não-rastreado (*untracked*) → Arquivos neste estado não estão presentes na versão atual (*HEAD*) e não constarão na próxima versão
- *Staged →* Arquivos neste estado trazem alguma mudança e constarão na nova versão.

## ⚙️ Configurações

`git config --global user.name "[nome]"` → Configura o nome relacionado aos commits

`git config --global user.email "[endereco-de-email]"` → Configura o email relacionado aos commits

`git config --list` → Lista as configurações atuais

---

## ⚙️ Comandos Básicos

`mkdir nomedapasta` → cria pastas na sua máquina

`echo"# nomedapasta" >> nomedoarquivo` → cria arquivos dentro de uma pasta

`cd nomedapasta` → acessar a pasta

`ls` → lista o que tem dentro da pasta

`git status` →  verifica status e modificações realizadas

`cd ..` → para mudar diretórios (voltar uma pasta anterior)

`git init` → Inicializa um repositório git

`git add nomedapasta ou nomedoarquivo` → adiciona o arquivo ou pasta específicos modificados na staged area

`git add .` →  adiciona todos os arquivos modificados na staged area

`git commit-m "comentário"` → Armazena os arquivos que estão na staged area para um novo commit, gravando-os no histórico de versão

Criando o repositório no GitHub, sem criar o README.md, teremos alguns comandos para fazer

![criando repositório](https://github.com/selenitye/git/blob/main/criando-repositorio.png?raw=true)

Já fizemos alguns ( init, add Readme, commit) e iremos fazer os outros que faltaram:

`git branch [nomedabranch]` → Cria uma nova branch

`git branch` → Apresenta as branches existentes e destaca a branch atual

`git remote add [nome-remote] [url-remote]` → Vincula o repositório remoto ao repositório local

`git push -u [nome-remote] [nome-branch-local]` → Envia os arquivos da branch do repositório local para o repositório remoto (utilizado no primeiro push)

**Repositório “subido” com sucesso!**

## 🧬 Clonando um repositório para nossa máquina

![clonando repositório](https://github.com/selenitye/git/blob/main/clonando-repositorio.png?raw=true)

em CODE, copiar a URL do repositório

na nossa máquina, na pasta que queremos colocar o repositório, abrimos o git e digitamos o comando:

`git clone [url que foi copiada]`  → Clona um repositório remoto para o repositório local

Entre no repósitório dentro da sua máquina com `cd nomedapasta` e digite 

`code .` → abre o repositório no VSCODE e voce pode codar por lá

![vscode](https://github.com/selenitye/git/blob/main/vscode.png?raw=true)

## 🆙 Subindo um repositório para o GitHub

Para subir subir uma alteração de um repositório já existente, siga os passos:

Na ordem, voce fará no GIT Bash
                                                                               
`cd [nomedapasta]`  → entre na pasta

`git status`  → veja o status e o que tem dentro da pasta

`git add .`  → `git commit -m "comentário"`  → `git push`  → Repositório add com sucesso ✌️

***fim xx***
