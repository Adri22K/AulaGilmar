# AulaGilmar
Aula 3 de Tópicos Avançados em Sistemas de Informação II - 12/09, necessário subir um projeto para o GIT HUB



1️⃣ Configuração Inicial 

Abra o CMD e configure seu nome e e-mail (apenas 1 vez no computador):

git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"


Verifique se foi configurado corretamente:

git config --list

2️⃣ Criar ou Acessar um Projeto

Criar uma nova pasta e acessar:

mkdir meu-projeto
cd meu-projeto


Se já tiver uma pasta existente:

cd caminho/da/sua/pasta

3️⃣ Iniciar o Git no Projeto

Transforma a pasta em um repositório Git:

git init

4️⃣ Verificar o Status

Mostra o que mudou desde o último commit:

git status

5️⃣ Adicionar Arquivos para Commit

Adicionar todos os arquivos modificados:

git add .


Adicionar um arquivo específico:

git add nome_do_arquivo.ext

6️⃣ Criar um Commit

Salvar as alterações com uma mensagem explicativa:

git commit -m "Descrição breve do que foi alterado"

7️⃣ Conectar ao Repositório Remoto (GitHub)

Se você criou o repositório no GitHub, conecte-o ao seu projeto local:

git remote add origin https://github.com/seuusuario/seurepositorio.git


Verifique se conectou certo:

git remote -v

8️⃣ Enviar o Código para o GitHub

Enviar para a branch principal (geralmente main):

git branch -M main
git push -u origin main


Depois, quando quiser mandar novas alterações:

git push

9️⃣ Baixar Alterações do Repositório Remoto

Caso alguém altere o projeto no GitHub, use:

git pull

🔄 Fluxo Completo de Trabalho

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
