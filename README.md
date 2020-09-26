# Manual de uso do Git
Este tutorial mostra o fluxo básico para operar no Git. :alien:
## 1. Inicializar repositório:

~ git init

## 2. Adicionar arquivos na Stage Area

~ git add . (Adiciona todos os arquivos alterados e novos)  
~ git add *.txt (Adiciona todos os arquivos alterados de um tipo específico)  
~ git add arquivo.txt (Adiciona arquivo alterado específico)

## 3. Registar arquivos no repositório

~ git commit -m "Aqui vai o comentário da atualização"

## 4. Ver todos os Commits feitos

~ git log  
~ git log -p (Mostras os commits com detalhes das alterações)  
~ git log --pretty=oneline (Mostrar os commits em uma linha cada)

## 5. Criar tags para Commits

~ git tag -a v1.0 -m "Versão 1.0" (Cria uma tag para o commit atual)  
~ git tag -a v1.0 dd508f2fc6e08714e5a24bfddb5c48197e2e8ec6 -m "Versão 1.0" (Cria uma tag para um commit específico, sinalizado pela hash do commit)  
~ git tag (Lista as tags existentes)  
~ git tag -d v1.0 (Deleta uma tag)  
~ git checkout v1.0 (Muda o repositório para a tag escolhida)

## 6. Criar branchs no projeto

~ git branch novo_branch (Crian um branch no projeto)  
~ git branch (Lista todos os branchs exitentes no projeto)

## 7. Transitar entre Branchs ou Tags

~ git checkout [branch ou tag]

## 8. Mesclar conteudo de um branch a outro

~ git merge [branch]

## 9. Interações com repositório remoto

~ git clone https://github.com/yure-cs/{repositorio}.git (Clona repositório do github)  
~ git remote add origin https://github.com/yure-cs/{repositorio}.git (Envia aquivos para o repositório)
~ git remote (Exibir repositórios remotos)  
~ git push origin master (Enviar arquivos commitados para o repositório)   
~ git pull origin master (Baixar arquivos commitados do repositório)
