# Comando: Git status

Para saber se há atualizações dentro do repositório, utilizar o comando:
`git status`

# Comando: Git add

Para adicionar arquivos que foram modificado recentemente, utilize o comando:

```
git add <nome_do_arquivo>
```

# Comando Git commit

Para efetuar o "salvamento" do arquivo, ou seja gravar a última versão que foi modificada no repositório, você deve utilizar o comando `git commit -m 'comentário'`.

_Atenção:_ O comando deve ser utilizado com o parametro _-m_ seguido de uma breve mensagem do que foi modificado entre apas..

## GIT

**Para realizar o dowonload e instalação do GIT, utilize o site oficial:** 
  https://git-scm.com/ 


Utilizando o Prompt de comando do GIT, chamado **Gitbash**

Para fazer com que o Git veja os arquivo que estão dentro daquela pasta/repositório faça:

* Navegue até a pasta desejada, utilizando o comando `cd` e depois começe a digitar a pasta que você quer acessar, no exemplo abaixo irei acessar a pasta git-e-github que está dentro do meu desktop (ou área de trabalho)

`cd Desktop\git-e-github`

## **Comandos Git**

### **Verificando Versão do GIT**
`git --version`
Este comando te informa qual a versão do git instalado na sua máquina

### `git init`
Este Comando inicia um repositório na pasta que você está acessando e defini ela para o GIT que essa pasta agora é um 'Repositório', onde ele deverá ficar monitorando e verificando se existem atualizações ou não.

`git status`
Este comando informa os arquivos que o GIT está monitorando ou não naquele repositório

`git add`
Utilizando o comando `git add` Você pode utilzar o `.` após o comando que o git irá adicionar todos os arquivos da pasta atual para monitoramento ou você pode definir um arquivo específico colocando o nome dele após o comando `git add`, como exemplo: `git add index.html`


`git commit -m`
Este comando serve para enviarmos as modificações realizadas no código para o servidor, **sempre deve ser utiulizado após o comando** `git add`
O parâmetro `-m` identifica um comentário que deve ser colocado entre `""` e nele, como boas práticas, é indicado que haja uma breve descrição da modificação que foi realizada no código

### **Visualizando Logs das alterações realizadas**
`git log`

Comando mostra várias informações dos **commits enviados para o** GIT
1. Commit HASH, HASH do commmit (identificador único de cada commit executado)
2. é o Branch (Ramo) (HEAD -> local onde estamos, MASTER -> ramo)
3. Author = Quem realizou o commmit
4. Date = Data do commit


`git log --online`

Esse comando mostra todas as alterações realizadas pelos commits de forma resumida em uma única linha

`git log -p`

Este comando mostra as alterações realizadas linha a linha no código, onde as linhas marcadas com `- foram removidas` e `+ foram adicionadas`


**Para saber mais informações sobre configurações e customizações de logs:**

Você pode acessar o link a seguir: https://devhints.io/git-log 
Neste link, você encontrará varios comandos que podem ser utilizados com o comando log.

# Criando Repositórios Remotos

Para criar um repositório remoto, onde ele irá armazenar as cópias dos arquivos em que fizemos modificações, você precisa utilizar o comando:

`git remote add <nome_do_repositorio> <caminho_do_repositorio>`

O caminho pode ser qualquer local de rede (pasta) ou até mesmo um endereço web





### Para verificar informações do repositório

Utilize o comando abaixo:

`git remote -v`

onde: 

*fecht* é o lugar onde irá buscar dados 

*push* é o lugar onde ele irá enviar dados


# **Clonando informações de um repositório remoto**

O comando abaixo é utilizado quando queremos realizar uma cópia 

`git clone <endereço_do_servidor_que_deseja_clonar> <nome_da_pasta>`

O comando abaixo é utilizado para enviar os dados para um servidor

`git push `

O comando abaixo é utilizado  para atualizar o nosso repositório com os dados no repositório remoto

`git pull`

# **Revertendo alterações -> Control Z no GIT**
Com o `git checkout` nós desfazemos uma alteração que ainda não foi adicionada ao index ou stage, ou seja, antes do `git add`. Depois de adicionar com git add, para desfazer uma alteração, precisamos tirá-la deste estado, com `git reset`. Agora, se já realizamos o `commit`, o comando git revert pode nos salvar.
