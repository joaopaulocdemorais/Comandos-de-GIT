# Comandos de GIT

 ![Logo GIT](https://github.com/joaopaulocm23/Comandos-de-GIT/blob/b08e01ee6971a20c53d1a3dbc3617c8cbb629595/Git-Logo-2Colorp.png)
 ***
## Nesse repositório vou colocar os comandos de GIT que uso atualmente no meu dia a dia de estudante de desenvolvimento de softwares. Uso esses comandos no CMD Windows sem interface gráfica para o GIT.

O quadro a seguir conterá os comandos na  primeira coluna e a explicação das suas funções na segunda.

COMANDO|EXPLICAÇÃO
:---: | :---:
git config --global user.name "NomeUsuario"|Define o nome de usuário do seu GIT. Exemplo: `git config --global user.name "João"`
git config --global use.email "E-mail"|Define o e-mail do seu usuário do GIT. Exemplo: `git config --global use.email "joaopaulomorais2@gmail.com"`
git config --list|Exibe como estão as configurações de usuários do git.
mkdir nomepasta|Cria uma pasta no terminal (cmd) do Windows. Ex: `mkdir git`.
cd diretório/pasta|Navega até uma pasta de arquivos do Windows através do terminal. Ex: `cd documents`
dir|Mostra todos os arquivos do diretório no cmd.
git init|Inicializa o git na pasta que você deseja ter o controle de versão.
git status|Mostra o atual estado dos arquivos dentro do git.
git add nomeDoAquivo|Passa um arquivo de modificado (modified) para preparado (staged) o deixando pronto para realizar um commit.Ex: `git add Readme.md`
git add .|Passa todos os arquivos do repositório de modificado (modified) para preparado (staged) o deixando pronto para realizar um commit.
git diff|Mostra as mudanças feitas nos arquivos antes de ser feito um commit.
git commit -m "Mensagem"|Guardar o estado do seu repositório naquele momento. Ex: `git commit -m "add Readme.md"`
git log|Lista os estados (commits) do repositório.
git checkout -b nomeDoBranch|Cria um novo Branch. Ex: `git checkout -b developer`
git branch|Mostra os branchs do repositório e qual está setado no momento.
git log --graph|Mostra de forma gráfica como foi o andamento dos branches no repositório
git checkout nomeDoBranch|Seta o branch que foi passado no comando. Ex: `git checkout developer`
git branch -D nomeDoBranch|Apaga o branch que foi passado no comando. OBS: O "-D" do comando esta em letra maiúscula. Ex: `git branch -D developer`
git merge nomeDoBranch|Faz o marge para dentro do branch que você desejá. Ex: `git marge developer`. [Clique aqui para saber o que git-marge](https://git-scm.com/docs/git-merge)
git rebase nomeDoBranch|Faz o rebase para dentro do branch que voçê desejá. Ex: ``git rebase developer`.[Clique aqui para saber o que git-rebase](https://git-scm.com/docs/git-rebase)
git show hashDoCommit|Mostrar as alterações adicionadas em relação ao commit anterior.Ex: `git show c58453f50f1ad91ee8709911c1ed68656ae67d43`
git reset nomeDoArquivo|Retorna o arquivo de staged (pronto para realizar o commit) para modified (arquivo em modificação). Ex: `git reset Readme.md`
git checkout nomeDoArquivo|Retorna um arquivo em edição (modified) para o estado do último commit. Ex: `git checkout Readme.md`
git reset --hard CodigoDoCommitQueDesejaVoltar| Volta para o commit  que você apontou através do código (hash) e elimina todos commit acima dele, e retira todas as modificações feitas nos arquivos. Ex: `git reset --hard 901794c31e3a56e545d10b32d7bc919fd4227a7b`
git reset --mixed CodigoDoCommitQueDesejaVoltar|Volta para o commit  que você apontou através do código (hash) e elimina todos commit acima dele, porém deixa o arquivo em modo de modificação, e não tira as alterações feitas. Ex: `git mixed --hard 901794c31e3a56e545d10b32d7bc919fd4227a7b`
git reset --soft CodigoDoCommitQueDesesaVoltar|Volta para o commit que você apontou através do código porem deixa os arquivos anteriores, e o mesmos ficam em modo staged prontos para realizar um novo commit.
git remote add LinkDoRepositorioRemoto|Adiciona repositório remoto (GitHub) ao local.  
git remote|Mostra o repositório remoto que está adicionado.
git push RepositórioDeDestino RepositórioDeOrigem| Envia os arquivos para o repositório remoto.
git push -u  RepositórioDeDestino RepositórioDeOrigem|Comando para enviar arquivos para o GitHub na primeira vez.  O "-u" do comando grava o destino e a origem do repositório, assim nas próximas vezes basta usar o `git push`. Ex: `git push -u origin master`
git push|Caso a origem e o destinho do repositório sejam iguais, após usar o  "-u" da primeira vez basta fazer um `git push` para enviar as atualizações.
git clone LinkDoRepositórioRemoto RepositórioLocal|Clona um repositório remoto para seu computador. Ex: `git clone git@github.com:joaopaulocm23/Comandos-de-GIT.git CloneComandos`
git tag -a NumeroVersao -m "Mensagem"|Usado para definir uma versão (Ponto) do sistema. Ex: `git tag -a v1 -m "Primeira versão"`
git tag|Mostra todas as tags geradas.
git push RepositórioDeDestino RepositórioDeOrigem --tags|Envia as versões (tags) para o GitHub. `git push origin master --tags`

### Nesse link  >> [clique aqui](https://docs.github.com/en/authentication/connecting-to-github-with-ssh) << tem a documentação de como gerar uma chave ssh para autenticar a máquina local ao GitHub. Isso evita  erro de permissão ao subir arquivos para o GitHub, e preciso criar uma chave para cada máquina.

### Para escrever esse arquivo Readme usei a linguagem Markdown. Para usar essa linguagem sigo manual escrito pelo professor Gustavo Guanabara. Você pode baixar esse aquivo nesse link >> [Guia Markdown](https://github.com/joaopaulocdemorais/Comandos-de-GIT/blob/e0853f50d04e89c1150ebe1149fe24bae0e7993d/guia-markdown.pdf)
