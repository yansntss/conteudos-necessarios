# Git e GitHub 🚀 
### Eu aprendo mais quando escrevo e finjo ensinar para alguem, então por que não compartilhar aqui ne?! vamo codaaaar 🚀 
<br>
Comandos básicos 
 
```jsx
//incializar a linha do tempo(repositorio)
git init

//adicionar tudo
git add .

//adicionar arquivo especifico
git add nome_do_arquivo

//criar o "ponto na historia"/enviar para o repositorio
git commit -m "nome_do_commit"

//mostrar o pontos na historia "commit"
git log

//mostrar o ultimo ponto na historia
git show
```

Vou começar uma nova funcionalidade mas não quero modificar o projeto, então eu crio uma nova branch para essa feature e modifico por la dessa forma:

```jsx
//criar uma nova branch(ramificação)
git branch nome_da_branch

//mudar a branch/entrar na branch
git checkout nome_da_branch 
 
// ver em qual branch está
git status
```

Entre na nova branch e adicione o quanto quiser sem ter o risco de bagunçar a branch master.

Tá, eu já criei uma nova branch, adicionei novas funcionalidades nela e quero colocar em produção na branch master, o que eu faço?

simpleeees :)

```jsx
//unir a linha do tempo/unir a branch nova com a master
git merge nome_da_branch_criada

//verificar se levou o arquivo pra branch master
git log
```

Hmmm, beleza, já que eu criei uma nova branch e ja coloquei em produção na branch master, agora eu quero deletar essa branch.

siiiimples 😂

  

```jsx
//deletar a branch criada
git branch -D nome_da_branch

// Liste as branch para verificar se foi deletada
git branch
```

## Resumo até agora

```jsx
git init //inicialiar linha do tempo/git
git add // adicionar a linha do tempo
git commit //criar  um ponto no repositorio
git log // vizualizar os commits

git branch nome_da_branch //criar uma nova branch(ramificação)
git checkout nome_da_branch //mudar a branch/entrar na branch
git merge nome_da_branch_criada //unir a linha do tempo/unir a branch nova com a master
git branch -D nome_da_branch //deletar a branch criada
```

E para enviar pro github ?

```jsx
//depois de ter criado o repositorio no github
//pegue o link do repositorio e faça dessa forma
git remote add origin link_do_repositorio

//como é o primeiro commit no github, você tem que criar a branch master la, dessa forma
git push -u origin master
```

No proximo commit para o github faça:

```jsx
git add . //para adicionar todas as alterações
git commit -m "nomde do commit" //criar o ponto no repositorio
git push //enviar para o repositorio do github

```

Tá, agora eu quero pegar o repositório do meu time e clonar, o que eu faço?

```jsx
//va ate o repoitorio que voce quer clonar
//pegue o link e execute esse comando:
git clone link_do_repositorio
```

Agora você precisa criar uma branch nova e mudar para essa branch

```jsx
//comando curto para cirar a branch e entrar
git checkout -b nome_aqui
```

Depois de  fazer a modificação

```jsx
//comando curto para atualizar e commitar
// o 'a' é de atualizar como se fosse o 'add .'
//o 'm' é a mensagem
git commit -am "nome do commit"
```

Para evitar conflitos, antes de enviar para o repositorio, você precisa atualizar o repositorio local.

```jsx
git pull

//depois pode dar o git push
git push
```

Para voltar um arquivo para um determinado momento da linha do tempo, primerio você tem que saber qual foi o momento

```jsx
//veja qual é o commit que você quer e copie o codigo
git log

//pode usar o checkout para amnipular a linha do tempo
git checkout codigo do comite -- nome_do_arquivo

//comando curto para atualizar e commitar
// o 'a' é de atualizar como se fosse o 'add .'
//o 'm' é a mensagem
git commit -am "nome do commit"

git push //para enviar para o repositorio

git config --global credential.helper store //para não ficar informando login e senha toda hora
```
### Referência 📖

 Aprendi a estilizar o readme com a 
Daniele Leao, vai la e deixa um carinho no youtube dela 💜 [Link do video](https://www.youtube.com/watch?v=2alg7MQ6_sI).

Tudo que eu escrevi aqui foi baseado [nesse video](https://www.youtube.com/watch?v=2alg7MQ6_sI) do mestre Maykao 💜 vai la e aprenda muito mais.

<br>

## Entre em Contato  💜

[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/yansntss/)](https://www.linkedin.com/in/yansntss/)
[![Twitter Badge](https://img.shields.io/badge/-Twitter-1ca0f1?style=flat-square&labelColor=1ca0f1&logo=twitter&logoColor=white&link=https://twitter.com/yanstnss)](https://twitter.com/NpmYan)
[![Whatsapp Badge](https://img.shields.io/badge/-Whatsapp-4CA143?style=flat-square&labelColor=4CA143&logo=whatsapp&logoColor=white&link=https://api.whatsapp.com/send?phone=55075988606100&text=Olá!)](https://api.whatsapp.com/send?phone=55075988606100&text=Olá!)
 