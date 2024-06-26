﻿<h1 align='center' > Monitoria em Ferramentas de Desenvolvimento de Software e Versionamento</h1>

<h3 align="center"> VsCode - PyCharm - Git & GitHub </h3>

<br>

Este é um projeto do PROGRAMA DE ACOLHIMENTO E INCENTIVO À PERMANÊNCIA (PAIP), da UFC - Campus de Itapajé, que tem como objetivo desenvolver uma monitoria/minicurso introdutório sobre as ferramentas de desenvolvimento de software, focando especialmente no Visual Studio Code (VsCode) e PyCharm, ambas amplamente utilizadas no campus, além de apresentar os conceitos fundamentais do Git e a plataforma GitHub para versionamento de código, colaboração e controle de projetos. O intuito foi capacitar os participantes a utilizar eficientemente essas ferramentas essenciais para o desenvolvimento e colaboração em projetos de software.

## Visual Studio Code (VsCode)
O Visual Studio Code, ou VsCode, é um editor de código fonte desenvolvido pela Microsoft. Ele é amplamente utilizado devido à sua _interface intuitiva_, _extensibilidade_ e _suporte robusto_ para uma variedade de linguagens de programação.

Algumas características notáveis do VsCode para desenvolvimento Python incluem:

- `Interface Amigável`: O VsCode oferece uma interface limpa e amigável que facilita a escrita, edição e navegação no código.

- `Extensões`: Possui uma vasta gama de extensões disponíveis que podem ser instaladas para adicionar funcionalidades específicas, como depuração, formatação de código, suporte a ambientes virtuais, entre outros.

- `Configuração Personalizada`: Permite personalizar facilmente as preferências do editor, atalhos de teclado e temas visuais para se adequar às preferências individuais do desenvolvedor.

### Como baixar e instalar o VsCode?

1. Baixe o VsCode em: https://code.visualstudio.com/
2. Execute o arquivo e siga as orientações, até concluir a instalação.

<br>

## PyCharm
O PyCharm é um ambiente de desenvolvimento integrado (IDE) projetado especificamente para Python pela JetBrains. É amplamente reconhecido pela sua poderosa funcionalidade e conjunto de recursos voltados para desenvolvimento eficiente em Python. 

Alguns destaques do PyCharm incluem:

- `Integração Completa`: Oferece suporte completo para Python, incluindo assistência inteligente ao código, depuração avançada, e testes integrados.

- `Funcionalidades Avançadas`: Inclui ferramentas avançadas como análise de código, refatoração inteligente, gerenciamento de pacotes e integração com frameworks populares como Django, por exemplo.

- `Otimização do Fluxo de Trabalho`: Fornece dicas e truques úteis para aumentar a produtividade, como geração automática de código, integração com controle de versão e suporte a virtual environments.

### Como baixar e instalar o PyCharm?

1. Baixe o Pycharm em: https://www.jetbrains.com/pt-br/pycharm/download/
2. Execute o arquivo e siga as orientações, até concluir a instalação.

<br>

## Git
Git é um `Sistema de Controle de Versão` de arquivos. Em outras palavras, é responsável por guardar o histórico de alterações sempre que alguém modificar algum arquivo que está sendo monitorado por ele.

Características do Git:
- `Colaboração Eficiente`:Permite que várias pessoas trabalhem simultaneamente no mesmo projeto sem interferir no trabalho umas das outras.

- `Controle de Versão Eficiente`: Permite registrar e acompanhar todas as alterações feitas em um projeto, facilitando a reversão a versões anteriores se necessário.

- `Workflow Flexível`: Suporta diferentes fluxos de trabalho de desenvolvimento, como ramificações (branches) para desenvolvimento paralelo e mesclagem (merge) de código.

- `Funcionalidades Cruciais`: Oferece comandos essenciais como 'commit' para salvar alterações, 'branch' para criar e gerenciar ramificações, e 'merge' para combinar alterações de diferentes ramificações.

### Como baixar e instalar o Git?

1. Acesse o site oficial do Git em https://git-scm.com/downloads.
2. Execute o arquivo e siga as orientações, até concluir a instalação.

<br>

## Comandos Principais do Git

### Inicialize um repositório Git local(sua máquina):

Para começar a rastrear seu código/monitorar o estado dos arquivos, crie um repositório Git em um diretório local. Navegue até a pasta do seu projeto e execute:
```bash
    git init
```
#

### Configure seu nome de usuário e e-mail, cadastrados no GitHub:

No Git, os comandos `git config user.name` e `git config user.email` são utilizados para configurar a identidade que será associada aos commits, ao usar o GitHub ou qualquer outro serviço Git remoto.

No caso, as credenciais feitas no momento da criação da conta no GitHub. Essas configurações são importantes para identificar quem fez determinadas alterações no código-fonte ao longo do histórico do repositório. 

Existem algumas maneiras principais de configurar o nome de usuário e o e-mail no Git. Duas principais delas são:

`Configuração Local`

```bash
    git config user.name "Seu Nome"
    git config user.email "seu@email.com"
```
Quando você configura o usuário localmente, as informações de nome de usuário e e-mail são específicas para o diretório/repositório Git atual em que você está trabalhando.

É útil configurar localmente se você trabalha em vários projetos com identidades de usuário diferentes(contas diferentes, por exemplo) ou se compartilha o ambiente de trabalho com outras pessoas. Permitindo que cada projeto tenha sua própria identidade de usuário.

Essas configurações são armazenadas no arquivo `.git/config` dentro do diretório do seu projeto Git. O Git usará essas informações ao fazer commits apenas nesse repositório específico.

`Configuração Global (com --global)`

```bash
    git config user.name "Seu Nome"
    git config user.email "seu@email.com"
```

Usar a opção `--global` indica que esta configuração será aplicada globalmente para todos os repositórios Git no seu sistema. Isso é útil quando você deseja usar as mesmas informações de identidade em todos os seus projetos `pessoais`, geralmente.

É conveniente definir globalmente suas informações de usuário se você usar Git em diferentes projetos ou em várias máquinas. Isso garante consistência em todos os commits que você faz. Recomendado para uso pessoal ou quando você não precisa alternar frequentemente entre identidades de usuário.

`Dicazinha*`<br>
Se você precisar sobrescrever ou verificar as configurações atuais do Git, você pode usar:

```bash
git config --list  # Lista todas as configurações do Git
git config user.name  # Exibe o nome de usuário configurado
git config user.email  # Exibe o e-mail configurado
```
#

### Adicione Arquivos ao Controle de Versão:

Use o comando `git add` para adicionar um arquivo específico ao staging area, preparando-o para o commit:
```bash
    git add nome-do-arquivo
```
    
Ou

```bash
    git add .
```
Caso tenha certeza de que quer subir todos os arquivos modificados.

`Staging area`, é um espaço temporário onde você adiciona e prepara os arquivos alterados para só depois serem “commitados” ou salvos no seu repositório local, ou no remoto se já estiver trabalhando com o GitHub.

#

### Verificar o Status do repositório:

Você pode verificar o estado atual dos repositório e seus arquivos, usando o comando:
```bash
    git status
```
Isso mostra quais arquivos foram modificados e quais estão na staging area, prontos para fazer o commit.
    
#

### Faça um Commit:

```bash
    git commit -m "mensagem-do-commit"
```

Fazer commit seria registrar as alterações no seu repositório, seja ele local ou remoto(GitHub, GitLab, etc). Eles representam um `compromisso` com a integridade e a `evolução do projeto`.

Por isso, é importante escrever mensagens de commit claras e significativas, para que outras pessoas (ou você mesmo, no futuro) possam entender o que foi feito em cada alteração:

```bash
    Ex.:
    git commit -m "Corrigir bug na validação do formulário de cadastro"
```

Cada commit registra o nome do autor (nome de usuário) e endereço de e-mail do autor, juntamente com a data e hora em que o commit foi realizado. Isso é mostrado também quando usamos o comando `git status`.

#

### Desfazendo Alterações

Há duas formas de desfazer alguma alterações indesejada, que talvez tenha sido "commitada" sem querer, etc..:

1º `git reset`
 - Desfaz commits existentes. Use quando precisar reescrever o histórico de commits local e não se importa em perder os commits desfeitos. Tenha cuidado ao usar git reset --hard, pois isso pode resultar na perda irreversível de alterações no diretório de trabalho.

2º `git revert`
 - Desfaz um commit existente, mas dessa fez criando um commit novo que reverte as alterações introduzidas pelo commit especificado. É úitl quando você deseja manter o histórico de commits intacto e apenas desfazer as alterações de um commit específico.
#

### Visualize o Histórico de Commits:

 ```bash
    git log
```
    
Para ver o histórico de alterações do projeto, onde aparecerão todos os commits feitos, com suas respectivas mensagens e códigos identificadores.

Um comando útil quando precisamos rastrear o andamento de um projeto e verificar em qual ponto cada funcionalidade foi implementada.

#

### Configurando Repositório Remoto

Para isso, antes é necessário que tenha uma [conta no GitHub](#como-criar-uma-conta), um [repositório remoto](#criando-repositórios) criado, mesmo que vazio. Pois, este é a versão do seu projeto que está hospedada no servidor remoto, no GitHb, por exemplo.

Finalmente! Chega de falar só do local, chegamos na parte de compartilhar as alterções de um repositório local para um remoto.

Mas, antes precisamos configurar nosso repositório hospedado (no nosso ambiente de trabalho, no VSCode ou PyCharm) antes de gerenciar a conexão entre local e remoto.

Para verificar se já possui um repositório remoto configurado e listar suas configurações existentes usando o comando:
```bash
    git remote -v
```

Para configurar um repositório remoto novo:
```bash
    git remote add 'apelido-repositorio-remoto' 'url-repositorio-remoto'
```
- Substitua `apelido-repositorio-remoto` pelo nome que você deseja atribuir ao repositório remoto _(O termo origin é frequentemente utilizado como um nome convencional para se referir ao repositório remoto principal de onde um repositório local foi clonado ou `para o qual foi configurado para enviar alterações`)_.

- Substitua `url-repositorio-remoto` pela URL do repositório remoto _(por exemplo, um [link HTTPS ou SSH](#criar-cópias-de-repositórios-remotos), geradas no GitHub)_.

Ex.:
```bash
    git remote add origin https://github.com/seu_usuario/seu_repositorio.git
```

#

### "Empurrando/Jogando" alterações do `local para o remoto`

Agora, que já configuramos nosso repositório remoto, podemos jogar nossas alterações para ele e assim guardar nosso projeto na núvem, podendo colaborar com outros devs, disponibilizar projetos próprios para que empresas vejam, etc:

```bash
    git push -u 'apelido-repositório-remoto' 'branch-local'
```

`push` vem de "empurrar", no caso, jogar aquelas alterações do local para o remoto.

`-u` (ou --set-upstream) é um parâmetro utilizado para configurar o branch local para rastrear o branch remoto durante o git push. Ao fazer isso, o Git associa automaticamente o branch local ao branch remoto correspondente.

`apelidorepositório_remoto`: É o apelido que referencia o repositório remoto para o qual você deseja enviar suas alterações.

`branch_local`: É o nome da [branch](#conceitos-de-branch) local que contém os commits que você deseja enviar para o repositório remoto.


#

### Conceitos de Branch

As “ramificações” ou branches permitem criar linhas separadas de desenvolvimento para trabalhar em recursos ou correções sem afetar a linha principal (branch `main`, geralmente) do projeto.

Cada branch é uma ramificação independente, possibilitando que você isole e desenvolva novas funcionalidades, refatore o código ou faça correções e testes em paralelo, `sem interferir no código` existente na `branch principal`.

O conceito prático de Branches, é ideal para projetos com vários desenvolvedores, cada qual executando uma atividade a parte, na sua própria branch, para só lá na frente examinarem a possibilidade de juntar todas essas informações, na branch principal, por exemplo.

Vamos aos comandos:

Para vermos as branch locais existentes:
```bash
    git branch
```

#

Para criarmos uma branch nova:
```bash
    git branch nome-da-branch
```

#

Para trocar para uma outra branch local (ou remota, caso já esteja trabalhando com repositórios remotos e outras branches):
```bash
    git checkout nome-da-branch
```

#

Para criar uma branch e imediatamente trocar para ela:
```bash
    git checkout -b nome-da-branch
```
#

Para renomear uma branch local:
```bash
    git branch -m 'nome-atual-branch' 'novo-nome-branch'
```

#

Para deletar uma branch:
```bash
    git branch -d nome-da-branch
```
#
Ou, se a branch não estiver totalmente mesclada e você deseja forçar a deleção, você pode usar -D em vez de -d:
```bash
    git branch -D nome-da-branch
```

#

### "Puxando" atualizações do `remoto para o local`

Outro mecanismo do Git é o fato de poder buscar e atualizar/integrar o repositório local com as alterações de um repositório remoto, sincronizando seu ambiente de trabalho com as últimas atualizações, `puxando` alterações de alguma branch, como a principal `main` ou outra qualquer:

```bash
    git pull 'apelido-repositorio' 'nome-branch'
```

Ele combina duas operações do Git em um único comando:
- `git fetch` para buscar as alterações do repositório remoto; e
- `git merge` para integrar essas alterações no seu branch local _(Falaremos dele mais adiante)_.

#

### Criar cópias de repositórios remotos:

Até o momento, trabalhamos muito com nossa própria parea de trabalho, criando um repositório local, etc.. Mas, que tal trabalharmos com um repositório que já existesse?

Imagine que seu professor solicitou que clonasse um repositório remoto dele, do GitHub, onde teria algumas atividades para cada aluno fazer sua parte..

No Git, há duas visões um tanto distintas de como fazer essa etapa de clonagem/criar uma cópia de algum repositório remoto:

1º Clone (Clona um repositório remoto, para o seu ambiente local de trabalho)
```bash
    git clone 'url-do-repositorio'
```
Subistitua `url-do-repositorio` pela url do repositório que deseja clonar, basta ir na página do repositório remoto, no GitHub, clicar no butão verde `code`, lá mostrará tanto a opção de `url HTTP` quanto `url SSH` _(Chave para autenticação. A autenticação por chave SSH é baseada em criptografia assimétrica, sendo mais segura e conveniente para ambiente de desenvolvimento mais sensíveis.)_.

- Poderia também, clonar pela própria IDE (VSCode), na opção `Clonar um repositório`, assim que você abre a IDE e entra no ícone do git, na janela à esquerda, e então inserir a url deste repositório.

- Ou pelo PyCharm, clicando no butão `Get From VCS` e colocar a url do repositório.

<br>

2º Fork _(Cria uma cópia independente de um repositório existente, isso dentro do seu GitHub)_

Ele é, geralmente, usado em projetos de código aberto e é uma maneira poderosa de contribuir para projetos mantidos por outras pessoas ou organizações sem modificar diretamente o repositório original.

 - No repositório desejado, clique no botão "Fork" no canto superior direito da página do repositório. Isso criará uma cópia do repositório na sua conta;

 - Clone o fork para o seu ambiente local usando git clone;

 - Faça as modificações desejadas no seu fork. Você pode criar novos branches, fazer commits, e push para o seu fork como faria com qualquer repositório Git, contribuindo com suas alterações.

<br>

#### Diferenças Chave

`Propriedade e Localização`: Um fork é uma cópia do repositório que fica armazenada no servidor (por exemplo, no GitHub), sob sua própria conta. Já um clone é uma cópia local do repositório, seja ele um original ou um fork.

`Permissões`: Ao fazer um fork, você obtém seu próprio repositório no GitHub que você controla completamente. Por outro lado, com um clone, você pode trabalhar localmente, mas para contribuir de volta ao repositório original (ou ao fork no servidor), você precisará de permissões adequadas para fazer push.

`Uso`: Forks são frequentemente usados em contextos onde você quer contribuir para um projeto do qual não é um colaborador direto, ou quando quer iniciar um projeto paralelo independente. Clones são usados para desenvolvimento local e colaboração direta (quando você tem acesso para push).

#

### GitHub
GitHub é uma plataforma de hospedagem de código baseada na web que utiliza o Git para controle de versão. É como se fosse uma “rede social dev” em que é possível armazenar e compartilhar projetos de desenvolvimento de software.

Além dos recursos do Git, o GitHub oferece funcionalidades adicionais:
- `Hospedagem Remota`: Permite armazenar repositórios Git na nuvem, facilitando o compartilhamento e colaboração entre desenvolvedores.

- `Colaboração em Equipe`: Facilita o trabalho em equipe através de recursos como pull requests, que permitem revisar e discutir alterações antes de mesclá-las no código principal.

- `Gestão de Projetos`: Oferece ferramentas para rastreamento de problemas (issues), gerenciamento de projetos e integração contínua.


### Como criar uma conta?

1. Acesse o site em "https://github.com".

2. Na página inicial do GitHub, você encontrará no canto superior direito um botão "Sign up" (Inscrever-se). Clique nele para iniciar o processo de criação da conta e preencha as informações, incluindo seu email, nome de usuário desejado e senha.
 - O GitHub pode enviar um email de verificação para o endereço fornecido. Verifique sua caixa de entrada e siga as instruções para confirmar seu email.

3. Verificação de e-mail cadastrado.

4. Escolha os membros (geralmente, só você) e se é estudante, professor ou nenhum.

<br>

### Criando Repositórios

Na página inicial, clique no botão verde "Create repository" (Criar repositório) / "New" (Novo).

Defina um nome para o seu repositório;
 - Caso seja seu primeiro repositório, é comum na comunidade dev criar um repositório "especial"(o GitHub te mostra na interface), no caso, com o mesmo nome do seu user, e optar por criar ou não um README _(Um arquivo em linguagem de markdown(.md))_, semelhante ao html, com suas informações principais, como habilidades, linguagens que mais usa, etc.
 
 - Caso seja um repositório para algum projeto, é interessante que o nome seja bem direto e específico, por exemplo, "ProjetoFinal_CadeiraTal", e nele haja um README com algumas explicações de como executar aquele projeto, ou só informações gerais.

Após isso, crie uma breve descrição, se preferir, e depois escolha se deseja que o repositório seja público (visível para todos) ou privado (acessível apenas por convite).

.gitignore: Você pode especificar tipos de arquivos que o Git deve ignorar ao rastrear alterações.

Escolha um Template (Opcional): Se o seu projeto se encaixa em um dos modelos de projeto disponíveis, você pode escolher um para iniciar com estrutura pré-definida.

Após preencher todas as informações necessárias, clique no botão "Create repository" (Criar repositório) para criar o seu repositório.

#

Com isso, chegamos ao final dessa jornada da monitoria. Foi um prazer imenso compartilhar esse conhecimentos com cada um dos alunos que participaram do projeto. Quero agradecer a todos pela cooperação e atenção. Espero ter sido coeso nas minhas falas e que este repositório sirva para pesquisas futuras, mas também estarei à disposição, se necessário.

Abaixo, deixarei alguns links que me auxiliaram na construção desta monitoria.

## Referências

Artigo da Formação DevOps da Alura
- [O que é Git e GitHub: os primeiros passos nessas ferramentas](https://www.alura.com.br/artigos/o-que-e-git-github)

<br>

Canal da Rafaella Ballerini
- [O QUE É GIT E GITHUB? - definição e conceitos importantes 1/2](https://youtu.be/DqTITcMq68k?feature=shared)
- [COMO USAR GIT E GITHUB NA PRÁTICA! - desde o primeiro commit até o pull request! 2/2](https://youtu.be/UBAX-13g8OM?feature=shared)

<br>
