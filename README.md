# 📍 Aula - Tópicos Avançados em Sistemas de Informação II 


<h1>  1️⃣ Configuração Inicial </h1>

Abra o CMD e configure seu nome e e-mail (apenas 1 vez no computador):

git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"


Verifique se foi configurado corretamente: git config --list

<h1>  2️⃣ Criar ou Acessar um Projeto </h1>

Criar uma nova pasta e acessar:

mkdir meu-projeto
cd meu-projeto


Se já tiver uma pasta existente:

cd caminho/da/sua/pasta

<h1>  3️⃣ Iniciar o Git no Projeto </h1>

Transforma a pasta em um repositório Git: git init


<h1>  4️⃣ Verificar o Status </h1>

Mostra o que mudou desde o último commit: git status


<h1>  5️⃣ Adicionar Arquivos para Commit </h1>

Adicionar todos os arquivos modificados: git add .


Adicionar um arquivo específico:

git add nome_do_arquivo.ext


<h1>  6️⃣ Criar um Commit </h1>

Salvar as alterações com uma mensagem explicativa:

git commit -m "Sua Mensagem"


<h1>  7️⃣ Conectar ao Repositório Remoto (GitHub) </h1>

Se você criou o repositório no GitHub, conecte-o ao seu projeto local:

git remote add origin https://github.com/seuusuario/seurepositorio.git


Verifique se conectou certo: git remote -v

<h1>  8️⃣ Enviar o Código para o GitHub </h1>

Enviar para a branch principal (geralmente main ou master):

git branch -M main
git push -u origin main


Depois, quando quiser mandar novas alterações: git push


<h1> 9️⃣ Baixar Alterações do Repositório Remoto </h1>

Caso alguém altere o projeto no GitHub, use: git pull


<h1>  🔄 Fluxo Completo de Trabalho </h1>

Depois da configuração inicial, o fluxo do dia a dia é:

git status
git add .
git commit -m "mensagem"
git push


🔧 Comandos Úteis Extras
Comando	Para que serve
git log	Mostra histórico de commits
git checkout -b nome-da-branch	Cria e muda para uma nova branch
git checkout nome-da-branch	Troca para outra branch
git merge nome-da-branch	Junta branch selecionada na branch atual
git clone URL	Baixa um repositório já existente do GitHub
git reset --hard HEAD~1	Desfaz o último commit (⚠️ cuidado)

<h1>  🧰 Comandos Git Importantes </h1>

🔍 Exploração e Status
Comando	O que faz
git status	Mostra o que mudou, arquivos prontos para commit, etc.
git log	Mostra o histórico de commits (pressione q para sair).
git log --oneline --graph --decorate	Histórico resumido, ótimo para visualizar branches.
git diff	Mostra diferenças entre seu código e o último commit.
git show <commit_id>	Mostra o que foi alterado em um commit específico.

🌱 Branches (Ramificações)
Comando	O que faz
git branch	Lista todas as branches locais.
git branch nome-da-branch	Cria uma nova branch.
git checkout nome-da-branch	Troca para outra branch.
git checkout -b nome-da-branch	Cria e já troca para a nova branch.
git merge nome-da-branch	Junta outra branch na branch atual.
git branch -d nome-da-branch	Apaga uma branch local.

📦 Trabalhando com Commits
Comando	O que faz
git commit --amend	Edita o último commit (mensagem ou arquivos).
git reset --soft HEAD~1	Desfaz o último commit, mas mantém as mudanças no stage.
git reset --hard HEAD~1	Apaga o último commit e as mudanças (⚠️ cuidado).
git revert <commit_id>	Cria um novo commit que desfaz outro commit.

🔄 Sincronização e Colaboração
Comando	O que faz
git fetch	Baixa alterações do remoto sem misturar no seu código.
git pull	Baixa e mescla alterações do remoto na sua branch.
git push origin nome-da-branch	Envia sua branch para o repositório remoto.
git remote -v	Lista repositórios remotos conectados.

🧹 Limpeza e Segurança
Comando	O que faz
git stash	Guarda temporariamente mudanças sem fazer commit.
git stash pop	Recupera mudanças guardadas pelo stash.
git clean -f	Remove arquivos não rastreados (⚠️ cuidado).

🆘 Ajuda
Comando	O que faz
git help <comando>	Mostra a documentação do comando.
git --version	Mostra a versão do Git instalada.

📌 Dica de ouro:
Sempre faça git pull antes de começar a mexer no projeto para evitar conflitos e manter tudo atualizado.
