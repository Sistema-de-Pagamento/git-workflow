# Git Workflow

A cada nova submissão no github, deve-se criar uma branch para seu desenvolvimento seguindo as seguintes instruções:

* O nome da branch deve começar com 'feat-', caso seja a implementação de uma nova funcionalidade, ou 'hotfix-', caso seja a correção de uma funcionalidade.
* Cada commit deve ser feito na sua branch e depois feito o merge request na branch Master.

## Iniciando o desenvolvimento

Antes de iniciar a codificação, deve-se clonar o repositório do projeto, para atualizar com todas as novas implementações.

```
git clone url-do-repositorio
```
Digitando o comando acima no terminal, o Git baixará o projeto no diretório selecionado.
Após isso, deve-se criar a sua branch. No caso de nova funcionalidade:

OBS: A nova branch sempre deve ser criada a partir da master, logo, deve-se estar na branch master para executar o comando de criação de branch

```
git checkout -b feat-especificacao-da-nova-funcionalidade
```
Para verificar em qual branch voce está:

```
git branch
```
Para trocar de branch:

```
git checkout nome-da-branch-de-destino
```
Uma vez criada a sua branch, e o projeto estar na branch criada, pode-se realizar o desenvolvimento.

## Terminando o desenvolvimento

Ao terminar o desenvolvimento, deve-se enviar sua implementação para o repositório.
Para isso, primeiro deve-se adicionar o projeto com as modificações, que faz a branch local reconhecer as alterações. Em seguida, realizar o commit para lançar para a branch local, e, por fom fazer o push para mandar da sua branch local para a remota. Na pasta do seu projeto, faça isso
OBS: certifique-se que você está na sua branch e não na master.

```
git add .
git commit -m "caso você queira escrever uma mensagem, escreva aqui"
git push origin nome-da-sua-branch
```
Por fim, para mandar sua branch para a branch master, deve-se realizar o merge
