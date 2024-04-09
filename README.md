<h1 align='center' > Monitoria em Ferramentas de Desenvolvimento de Software e Versionamento </h1>
<h2 align='center' > VsCode - PyCharm - Git - GitHub </h2>

O objetivo deste projeto foi desenvolver um minicurso introdutório sobre as ferramentas de desenvolvimento de software, focando especialmente no Visual Studio Code (VsCode) e PyCharm, ambas amplamente utilizadas no campus. Além disso, o curso apresentou os conceitos fundamentais do Git e a utilização da plataforma Github para versionamento de código, colaboração e controle de projetos. O intuito foi capacitar os participantes a utilizar eficientemente essas ferramentas essenciais para o desenvolvimento e colaboração em projetos de software.

### Visual Studio Code (VsCode)
O Visual Studio Code, ou VsCode, é um editor de código fonte desenvolvido pela Microsoft. Ele é amplamente utilizado devido à sua <strong>interface intuitiva</strong>, <strong>extensibilidade</strong> e <strong>suporte robusto</strong> para uma <strong>variedade de linguagens de programação</strong>.

Algumas características notáveis do VsCode para desenvolvimento Python incluem:

- `Interface Amigável`: O VsCode oferece uma interface limpa e amigável que facilita a escrita, edição e navegação no código.

- `Extensões`: Possui uma vasta gama de extensões disponíveis que podem ser instaladas para adicionar funcionalidades específicas, como depuração, formatação de código, suporte a ambientes virtuais, entre outros.

- `Configuração Personalizada`: Permite personalizar facilmente as preferências do editor, atalhos de teclado e temas visuais para se adequar às preferências individuais do desenvolvedor.

### Como baixar e instalar o VsCode?

1. Baixe o VsCode em: https://code.visualstudio.com/
2. Execute o arquivo e siga as orientações, até concluir a instalação.

#

### PyCharm
O PyCharm é um ambiente de desenvolvimento integrado (IDE) projetado especificamente para Python pela JetBrains. É amplamente reconhecido pela sua poderosa funcionalidade e conjunto de recursos voltados para desenvolvimento eficiente em Python. 

Alguns destaques do PyCharm incluem:

- `Integração Completa`: Oferece suporte completo para Python, incluindo assistência inteligente ao código, depuração avançada, e testes integrados.

- `Funcionalidades Avançadas`: Inclui ferramentas avançadas como análise de código, refatoração inteligente, gerenciamento de pacotes e integração com frameworks populares como Django, por exemplo.

- `Otimização do Fluxo de Trabalho`: Fornece dicas e truques úteis para aumentar a produtividade, como geração automática de código, integração com controle de versão e suporte a virtual environments.

### Como baixar e instalar o PyCharm?

1. Baixe o Pycharm em: https://www.jetbrains.com/pt-br/pycharm/download/
2. Execute o arquivo e siga as orientações, até concluir a instalação.

#

### Git
Imagine que você precise gerenciar um projeto de desenvolvimento de software que envolve uma equipe com vários desenvolvedores, cada um contribuindo com uma parte específica do código..

Como podemos assegurar que todas as peças vão se encaixar perfeitamente?

É aí que entram as ferramentas Git e GitHub. Ambas são ferramentas distintas, mas colaboram de maneira integrada para tornar o desenvolvimento de software mais eficiente.

Git é um sistema de controle de versão de arquivos. Em outras palavras, é responsável por guardar o histórico de alterações sempre que alguém modificar algum arquivo que está sendo monitorado por ele.

Características do Git:
- `Controle de Versão Eficiente`: Permite registrar e acompanhar todas as alterações feitas em um projeto, facilitando a reversão a versões anteriores se necessário.

- `Workflow Flexível`: Suporta diferentes fluxos de trabalho de desenvolvimento, como ramificações (branches) para desenvolvimento paralelo e mesclagem (merge) de código.

- `Funcionalidades Cruciais`: Oferece comandos essenciais como 'commit' para salvar alterações, 'branch' para criar e gerenciar ramificações, e 'merge' para combinar alterações de diferentes ramificações.

### Como baixar e instalar o Git?

1. Acesse o site oficial do Git em https://git-scm.com/downloads.
2. Execute o arquivo e siga as orientações, até concluir a instalação.

### Iniciando no Git

- Inicialize um repositório Git local(sua máquina):

    Para começar a rastrear seu código/monitorar o estado dos arquivos, crie um repositório Git em seu projeto. Navegue até a pasta do seu projeto e execute:
    ```bash
    git init
    ```

- Configure seu nome de usuário e e-mail, cadastrados no github:

    No Git, os comandos `git config user.name` e `git config user.email` são utilizados para configurar as informações de identidade do usuário nos commits. Essas configurações são importantes para identificar quem fez determinadas alterações no código-fonte ao longo do histórico do repositório. 
    
    Use os comandos, no terminal:
    ```bash
    git config --global user.name "Seu Nome"
    git config --global user.email "seu@email.com"
    ```
    `--global`: Indica que esta configuração será aplicada globalmente para todos os repositórios Git no seu sistema. Se você omitir --global, a configuração será específica para o repositório atual.

- Verificar o Status da Staging Area:
    
    Staging area, é um espaço temporário onde você prepara os arquivos alterados para só depois serem “commitados” ou salvos.
    
    Você pode verificar o estado dos arquivos, usando o comando:
    ```bash
    git status
    ```
    Isso mostra quais arquivos foram modificados e quais estão na staging area prontos para fazer o commit.
    
- Adicione Arquivos ao Controle de Versão:

    Use o comando `git add` para adicionar arquivos ao "staging area":
    ```bash
    git add nome-do-arquivo
    ```
    
    Ou

    ```
    git add .
    ```
    (Caso tenha certeza de que quer subir todos os arquivos modificados)

- Conceitos de Branch:

    As “ramificações” ou branches permitem que você crie linhas separadas de desenvolvimento para trabalhar em recursos ou correções sem afetar a linha principal do projeto.

    Cada branch é uma ramificação independente do código-fonte, possibilitando que você isole e desenvolva novas funcionalidades, refatore o código ou faça correções e testes em paralelo, sem interferir no código existente na branch principal, que geralmente é nomeada como "main".

    Em um projeto com branches diferentes, a fusão, ou merge, permite combinar as alterações dessas branches de volta à linha principal, quando as alterações estão prontas.

    Vamos aos comandos:

    Para vermos as branch existentes:
    ```bash
    git branch
    ```

    Para criarmos uma branch nova:
    ```bash
    git branch nome-da-branch
    ```

    Para navegar entre as versões do projeto:
    ```bash
    git checkout nome-da-branch
    ```

    Para criar uma branch e imediatamente mudar para ela:
    ```bash
    git checkout -b nome-da-branch
    ```

- Faça um Commit:

    Um commit seria o “compromisso”, uma ação em que você faz uma alteração no projeto, se compromete e salva suas alterações no histórico do projeto.

    Cada commit registra o nome do autor (nome de usuário) e endereço de e-mail do autor, juntamente com a data e hora em que o commit foi realizado.
    
    Crie um commit com uma mensagem descritiva do que foi alterado no projeto, executando:
    ```bash
    git commit -m "Sua mensagem de commit aqui"
    ```
- Visualize o Histórico de Commits:

    ```bash
    git log
    ```
    ara ver o histórico de alterações do projeto, onde aparecerão todos os commits feitos, com suas respectivas mensagens e códigos identificadores.

    Um comando útil quando precisamos rastrear o andamento de um projeto e verificar em qual ponto cada funcionalidade foi implementada.

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

### Criando Repositórios
1. Na página inicial, clique no botão verde "Create repository" (Criar repositório) / "New" (Novo).

2. Defina um nome para o seu repositório;
 - Caso seja seu primeiro repositório, é comum na comunidade dev criar um repositório "especial"(o github te mostra na interface), no caso, com o mesmo nome do seu user, onde estaria um README* mais geral, com suas informações principais, como habilidades, linguagens que mais usa, etc.
 
 - Caso seja para algum projeto, é interessante que o nome seja bem direto e específico, por exemplo, "ProjetoFinal_CadeiraTal".
 
    Após isso, crie uma breve descrição, se preferir e depois escolha se deseja que o repositório seja público (visível para todos) ou privado (acessível apenas por convite).

3. Você pode optar por inicializar o repositório com um arquivo README, (* - Voltando ao ponto 2 - ) que é um arquivo em linguagem de markdown(.md), semelhante ao html, a boa prática para fornecer informações sobre o projeto. Além disso, você pode escolher uma licença para o seu código, se desejar.

.gitignore: Você pode especificar tipos de arquivos que o Git deve ignorar ao rastrear alterações. Por exemplo, você pode selecionar uma linguagem de programação específica para gerar um arquivo .gitignore correspondente.

Escolha um Template (Opcional): Se o seu projeto se encaixa em um dos modelos de projeto disponíveis, você pode escolher um para iniciar com estrutura pré-definida.

Create Repository: Após preencher todas as informações necessárias, clique no botão "Create repository" (Criar repositório) para criar o seu repositório.


#

## Referências

Artigo da Formação DevOps da Alura
- [O que é Git e Github: os primeiros passos nessas ferramentas](https://www.alura.com.br/artigos/o-que-e-git-github)

<br>

Canal da Rafaella Ballerini
- [O QUE É GIT E GITHUB? - definição e conceitos importantes 1/2](https://youtu.be/DqTITcMq68k?feature=shared)
- [COMO USAR GIT E GITHUB NA PRÁTICA! - desde o primeiro commit até o pull request! 2/2](https://youtu.be/UBAX-13g8OM?feature=shared)

