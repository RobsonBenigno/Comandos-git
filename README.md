# Comandos-git
🧭 1. Configuração inicial

Esses comandos definem as informações básicas do usuário:

Comando	Função	Exemplo
git config --global user.name "Seu Nome"	Define seu nome de usuário (aparece nos commits)	git config --global user.name "Robson Santhana"
git config --global user.email "seuemail@exemplo.com"	Define seu e-mail de identificação	git config --global user.email "robson@email.com"
git config --list	Mostra todas as configurações atuais do Git	—

📁 2. Criação e inicialização

Cria ou prepara um repositório Git.

Comando	Função	Exemplo
git init	Inicia um novo repositório Git na pasta atual	git init
git clone [URL]	Clona (baixa) um repositório remoto do GitHub para o seu computador	git clone https://github.com/robson/meu-projeto.git

🧱 3. Controle de arquivos

Adiciona, verifica e remove arquivos do controle do Git.

Comando	Função	Exemplo
git status	Mostra o estado atual do repositório (arquivos modificados, não rastreados, etc.)	git status
git add [arquivo]	Adiciona um arquivo à área de stage (prepara para commit)	git add index.html
git add .	Adiciona todos os arquivos modificados	git add .
git rm [arquivo]	Remove um arquivo e registra a remoção no Git	git rm style.css

💾 4. Commits (salvar alterações)

Usado para registrar uma nova versão do seu projeto.

Comando	Função	Exemplo
git commit -m "mensagem"	Cria um commit com uma mensagem descritiva	git commit -m "Adicionando página inicial"
git log	Mostra o histórico de commits (com autor, data e mensagem)	git log
git show [id_do_commit]	Mostra o que foi alterado em um commit específico	git show 3e1f7ab

🌿 5. Branches (ramificações)

Branches são versões paralelas do projeto (muito usadas em equipe).

Comando	Função	Exemplo
git branch	Lista todas as branches	git branch
git branch [nome]	Cria uma nova branch	git branch nova-funcionalidade
git checkout [nome]	Muda para outra branch	git checkout nova-funcionalidade
git branch -M main	Renomeia a branch atual para “main”	git branch -M main
git merge [nome]	Une uma branch com a atual	git merge nova-funcionalidade

☁️ 6. Repositório remoto (GitHub)

Permite sincronizar seu projeto local com o GitHub.

Comando	Função	Exemplo
git remote add origin [URL]	Conecta seu repositório local ao remoto	git remote add origin https://github.com/robson/meu-projeto.git
git remote -v	Lista os repositórios remotos conectados	git remote -v
git push -u origin main	Envia suas alterações locais para o GitHub	git push -u origin main
git pull	Atualiza o projeto local com as mudanças do GitHub	git pull
git fetch	Baixa as alterações do repositório remoto, mas não as aplica ainda	git fetch

🔄 7. Desfazer alterações

Corrige erros sem quebrar o histórico.

Comando	Função	Exemplo
git restore [arquivo]	Desfaz modificações feitas em um arquivo antes do commit	git restore index.html
git reset [arquivo]	Remove o arquivo da área de stage (sem apagar alterações)	git reset index.html
git reset --hard [commit]	Volta o projeto inteiro para um commit anterior (⚠️ perigoso)	git reset --hard 3e1f7ab

🔍 8. Visualização e comparação

Ajuda a inspecionar o que foi modificado.

Comando	Função	Exemplo
git diff	Mostra as diferenças entre a versão atual e a última commitada	git diff
git diff --staged	Mostra as diferenças entre o stage e o último commit	git diff --staged

🧹 9. Limpeza e manutenção

Mantém o repositório organizado.

Comando	Função	Exemplo
git clean -f	Remove arquivos não rastreados	git clean -f
git gc	Faz uma limpeza geral no repositório (otimiza espaço)	git gc

📋 10. Ajuda

Se esquecer de algo:

git help [comando]


Exemplo:

git help commit



➡️ Isso abre a documentação oficial do comando.

