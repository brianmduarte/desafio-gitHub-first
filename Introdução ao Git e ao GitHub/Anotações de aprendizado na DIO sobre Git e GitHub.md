## Anotações de aprendizado na DIO sobre Git e GitHub :man_technologist:

Link para download do Git: https://git-scm.com/downloads

Entendendo o que é Git e sua importância

Um [repositório do Git](https://bitbucket.org/product/br/code-repository) é um armazenamento virtual para projetos. Ele permite que você salve versões do código, que você pode acessar quando precisar.

Possibilidades do GIT:

•	Controle de Versão
•	Armazenamento em nuvem
•	Trabalho em equipe
•	Melhorar o seu código
•	Reconhecimento.

**Tópicos fundamentais para entender o funcionamento do Git**

- SHA1: a sigla significa *Secure Hash Algorithm*, é um conjunto de funções hash criptográficas projetadas pela NSA. A encriptação gera um conjunto de caracteres identificador de **40 dígitos**.
* É uma forma curta de representar um arquivo.

Blobs, Trees e Commits: códigos relacionados ao versionamento.

**Blob**: contém o tamanho, \0 e a string de fato.
**Tree**: armazenam blocos <tamanho>

**Chave SSH**: forma de estabelecer uma conexão segura e confiável com o GIT Hub.
**Local para gerar a chave SSH no Git Hub: para gerar a chave, inserir o código indicado pelo próprio site da Git hub.

**mkdir** – cria uma pasta em sequência você pode atribuir o nome a ela.

**Git init** – cria-se um repositório/pasta git.
**Git add e Git commit** – Depois de adicionar o arquivo e fazer as inserções pelo Markdown, voltamos ao GIT para utilizar o git add * (já com o documento na pasta), e depois o git commit –m “a mensagem que eu quiser”.

**Git commit:** O comando `git commit` captura um instantâneo das mudanças preparadas do projeto no momento. Os instantâneos com commit podem ser considerados versões "seguras" de um projeto, o Git nunca os altera, a menos que você peça a ele. Antes da execução de `git commit`, o comando `git add` é usado para promover ou "preparar" mudanças no projeto que são armazenadas em um commit. Estes dois comandos - `git commit` e `git add` - estão entre os mais usados.



**Untracked**: arquivo que acaba de ser criado no repositório (ainda era inexistente).
Quando criado, vai direto para o Staged.

**Unmodified**: ocorre quando um arquivo é modificado.
Se removido, retorna para Untracked.

**Staged**: momento em que o arquivo se tornará um Commit (o ciclo será reiniciado em Untracked).



**Alguns comandos:**

* cd "+nome da pasta para entrar"

* git config --global user.email "inserir o e-mail aqui" --> Tal comando é utilizado para realizar o cadastro do e-mail do usuário.
* git config --global user.name "inserir o nome de usuário" --> cadastrar o nome (por preferência o mesmo do GitHub)
* git config --list --> traz um rol de informações importantes, dentre elas o nome de usuário e e-mail. 
* git config --global unset user.name/user.email --> comando utilizado para alterar um nome de usuário ou e-mail.

**Inserindo o repositório ao GitHub:**

* 1º passo: criar um repositório no GitHub;
* 2º copiar o "git remote add origin"
* 3º ir no git bash e realizar o seguinte comando: "git remote add origin "inserir o link entre as aspas"
* 4º git remote -v --> observar se o link de fato foi registrado;
* 5º git push origin master --> "empurra" o projeto para o site, no mesmo momento irá pedir autorização no GitHub para cadastrá-lo.
* 6º o repositório estará disponível no GitHub.
* Também é possível "puxar" o projeto caso este esteja conflitado pela alteração de algum outro usuário.  Neste caso, utiliza-se o comando: "git pull origin master", e assim faz a organização pelo terminal das alterações que foram sugeridas e/ou feitas.

