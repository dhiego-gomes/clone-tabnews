# clone-tabnews
Minhas anotações do curso.dev usando o tabnews como referência.

## Dia 3
### A fundação

- Arquivo ```.nvmrc```. O ```rc``` significa ```run command```. Aqui nós colocamos especificações recomendadas para rodar nosso projeto.

### A primeira parede
- 

## Dia 4
### Página inicial
-

## Dia 5
### Onde fica o "Git"? E como era feito antes disso?

- **Sistema de versionamento centralizado:** existe uma cópia principal do arquivo. Quem precisava editar o código, reservava o arquivo e ele não poderia ser editado por outras pessoas até que a pessoa que estava editando liberasse o arquivo.
- **Sistema de versionamento descentralizado:** todos podem editar o arquivo ao mesmo tempo. O algoritmo tenta aproveitar ao máximo as alterações feitas.

### Git Log (e o Jogo dos 7 Erros)

- ```Diff```: o Git não salva apenas o ```diff``` das alterações, pois em arquivos com muitas alterações isso teria um custo de processamento muito alto.

### Git Diff e Amend (e a Viagem no Tempo)

- ```git diff```
- ```git commit --amend```

## Dia 6
### Git Push
- ```Your branch is ahead of 'origin/main' by 1 commit.``` Minha branch local está 1 commit na frente da branch original.
- ```git push```
- ```package.json``` metadados como autor, descrição, scripts e dependências.
- ```package-lock.json``` exclusivo das dependências principais e as dependências dessas dependências.
- ```commit -m``` = mensagem

## Dia 7
### Client / Server
- ```Client``` e ```Server``` podem trocar de posição, dependendo do que estão fazendo no momento. Ou seja, um certo momento, um ```client``` pode virar um ```server``` e vice-versa. Um servidor pode ter vários clientes conectados nele e também pode se conectar a vários outros servidores.

### Hospedagem e Deploy
- Vercel ❤️
- Continuous Deployment