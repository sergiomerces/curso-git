![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fmedia.licdn.com%2Fdms%2Fimage%2Fv2%2FD4D12AQG6sk7vqlhmdA%2Farticle-cover_image-shrink_720_1280%2FB4DZfRAC4DHkAQ-%2F0%2F1751558140561%3Fe%3D2147483647%26v%3Dbeta%26t%3Dz51POqNqRAMnxQ7_fPZ7N52LpdHqPGIJvaQFfmYl860&f=1&nofb=1&ipt=baf7352512c787a05b10aff55a99305b58d418e0916e8c47206160368a9c2966)

# Curso de Git



**Git** é um sistema de controle de versão distribuída, criado por _Linus Torvals_ em 2005. Ele permite rastrear alterações no código-fonte ao longo do tempo, facilitando a colaboração entre desenvolvedores e o gerenciamento do histórico de um projeto.

Por que usar git:

1. Cada alteração feita é registrada, permitindo voltar a qualquer ponto do tempo;
2. Vários desenvolvedores podem trabalhar simultaneamente no mesmo projeto sem conflitos;
3. Permite criar linhas de desenvolvimento independentes para features, correções, documetação, etc e
4. Cada desenvolvedor possui uma cópia completa do repositório, não dependendo de um servidor central.

### Repositório

É uma pasta do projeto que está sendo rastreada pelo git.

### Estados

1. modificado
2. preparado
3. commitado

### Commit

É um _snapshot_ do estado dos arquivos do projeto em um determinado momento.

### Branch

Ramificação independente do desenvolvimento, a _branch_ padrão é chamada **main** ou **master**.



## Configuração Default Terminal

**git config --global user.name <nome-usuario>**

- seta o nome de usuário da conta git

**git config --global user.email <conta-email>**

- seta a conta de e-mail da conta git

**git config --global init.defaulBranch <main>**



## Meu Projeto

**git init**

- iniciar novo repositório local com git

**git add <nome-arquivo>/.**

- adiciona o arquivo modificado ao _stage_ para ser commitado

**git add .**

- adiciona todos arquivos modificados ao _stage_ para serem commitados

**git diff**

- mostra o que foi alterado
- mostra quais foram as alterações na ramificação

**git restore <arquivo>**

- descarta alterações do stage

**git commit -m <mensagem commit>**

- commita os arquivos no histórico

  - feat: nova funcionalidade

    fix: correção de bug

    docs: alteração na documentação

    style: formatação e sintaxe

    refactot: refatoração de código

    test: adição ou correção de teste

**git commit --amend -m <nova mensagem>**

- altera o comentário do último commit

**git status**

- mostra como está o estado da nossa modifcação

**git merge <branch>**

- mescla a ramificação indicada com a atual

**git branch**

- mostra a ramificação atual

**git branch <branch>**

- cria uma branch com o nome indicado

**git branch -m <branch>**

- renomeia uma branch

**git checkout -b <branch>**

- cria uma nova ramificação com o nome indicado a partir da atual e muda para ela

**git branch -D <branch>**

- deleta a branch indicada

**git checkout <branch>**

- muda para a ramificação indicada

**git remote add origin <url>**

- adiciona um repositório remoto

**git push -u origin main**

- configura upstream e empurra alterações locais para o repositório remoto (primeira vez)

**git push origin <branch>**

- empurra alterações locais para o repositório remoto

**git push origin <nova branch>**

- empurra nova branch local para o repositório remoto

**git pull origin <branch>**

- puxa alterações remotas para o repositório local

**git fetch**

- atualiza o histórico do repositório local com o histórico do repositório remoto
- sincroniza o repositório local com o repositório remoto

**git clone <url>**

- clona o repositório remoto para a máquina local

**git log**

- mostra o histórico de commits

**git shortlog**

- mostra o histórico de commits de forma simplificada



## Fluxo de Trabalho

1. Começar uma nova feature
2. Editar código para desenvolvimento da feature
3.  Salvar alterações (commitar)
4.  Empurrar alterações para o remoto (push)
5. Aprovação
6. Acessar a main
7. Dar pull na main
8. Mesclar 
9. Push na main

## 