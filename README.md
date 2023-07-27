# clone-tabnews

Minhas anotações do curso.dev usando o tabnews como referência.

## Dia 3

### A fundação

- Arquivo `.nvmrc`. O `rc` significa `run command`. Aqui nós colocamos especificações recomendadas para rodar nosso projeto.

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

- `Diff`: o Git não salva apenas o `diff` das alterações, pois em arquivos com muitas alterações isso teria um custo de processamento muito alto.

### Git Diff e Amend (e a Viagem no Tempo)

- `git diff`
- `git commit --amend`

## Dia 6

### Git Push

- `Your branch is ahead of 'origin/main' by 1 commit.` Minha branch local está 1 commit na frente da branch original.
- `git push`
- `package.json` metadados como autor, descrição, scripts e dependências.
- `package-lock.json` exclusivo das dependências principais e as dependências dessas dependências.
- `commit -m` = mensagem

## Dia 7

### Client / Server

- `Client` e `Server` podem trocar de posição, dependendo do que estão fazendo no momento. Ou seja, um certo momento, um `client` pode virar um `server` e vice-versa. Um servidor pode ter vários clientes conectados nele e também pode se conectar a vários outros servidores.

### Hospedagem e Deploy

- Vercel ❤️
- Continuous Deployment

## Dia 9

### Qual o “segredo” para organização de tarefas?

- Fazer muito com pouco e não pouco com muito.
- Níveis de planejamento
  - Nível 1: Ser lembrado individualmente.
    - Menor custo de produção e menor tempo de aquecimento possível. Exemplo: lista de tarefas numa folha de papel.
  - Nível 2: Ser lembrado em grupo.
    - Exemplo: Kanban.
    - Nesse tipo de organizador nós fazemos as marcações de progresso que está sendo feito.
    - Não é tão bom para detalhar o que precisa ser feito.
  - Nível 3: Expandir conhecimento.
    - Nesse nível de planejamento podemos detalhar melhor cada tarefa. Mas, é mais caro para produzir e aquecer.
    - Exemplos: Trello.
  - Nível 4: Gerar métricas

### Como peitar projetos de qualquer tamanho?

- Nosso cérebro tenta negociar com o "tudo ou nada". "Ou faz o projeto inteiro de uma vez ou não faz nada!" Ele quer que a gente não faça nada, porque o saldo para não fazer nada é sempre muito positivo e deixa a gente livre pra fazer qualquer coisa, como se divertir.
- `Issues` e `Milestones`
- 3 estágios da dopamina
  1. Início. Quando identificamos que algo positivo pode acontecer. Cérebro libera um pouco de dopamina que nos motiva a fazer alguma coisa para receber a recompensa.
  2. Progresso. Quando percebemos progresso, o cérebro libera mais dopamina para nos incentivar a continuar com vontade de continuar fazendo a tarefa.
  3. Conclusão. Quando finalizamos a tarefa recebemos a dopamina final.

## Dia 10

### Sincronização das configurações do Editor

- Dividir `Issues` em `Tarefas`.
- 💡Sugestão de outro aluno: criar perfis de configuração para o editor. Isso ajuda a ter um gerenciamento melhor das ferramentas usadas em cada projeto.

### Configurar o `EditorConfig`

- A extensão `EditorConfig` é um configurador de editor. No arquivo `.editorconfig`, definimos como o editor deve ser comportar.
  - Largura da indentação, espaçamento e etc.
- Ele atua nos arquivos **_antes_** do salvamento.

### Configurar o `Prettier`

- `Prettier` é um formatador de código opinado.
- Ele atua nos arquivos **_depois_** do salvamento.
- Comando para instalação: `npm install prettier -D`
  - `-D` indica que ele será instalado como uma ferramenta de desenvolvimento.
- Script para o `Prettier` **_verificar_** todos os arquivos:
  - `package.json` > `scripts` > `"lint:check": "prettier --check ."`
- Script para o `Prettier` **_corrigir_** todos os arquivos:
  - `package.json` > `scripts` > `"lint:fix": "prettier --write ."`
- `npm run lint:check` ou `lint:fix`
- A extensão do `Prettier` atua **_ao salvar_** os arquivos. Nas configurações do editor, definimos em `Editor: Default Formatter` a opção `Prettier`. Assim, o vscode vai deixar que o `Prettier` formate os arquivos ao salvarmos. Habilitamos a opção `Editor: Format On Save`.

### Configurar o Prettier Ignore

- `.prettierignore` funciona igual o `.gitignore`.

## Dia 11

### Resolução de `DNS`

- Domínios são **_apelidos_** dos IPs.
- `DNS` Domain Name System.
- De maneira simples, como o computador acessa um site?
  1. O computador se conecta com o servidor DNS usando o **_domínio_** do site.
  2. O servidor DNS fornece o **_IP_** do domínio.
  3. O computador acessa o servidor do site usando o IP que ele recebeu.