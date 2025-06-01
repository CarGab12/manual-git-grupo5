## 1. O Que São Branches?
Branches (ramificações) são linhas independentes de desenvolvimento. A branch principal geralmente é chamada de main ou master, e outras branches são usadas para criar novas funcionalidades ou corrigir bugs sem afetar o código principal.

## 2. Criar e Usar Branches
Criar uma nova branch: git branch nome-da-branch
Exemplo: git branch nova-funcionalidade

Mudar para uma branch existente: git checkout nome-da-branch
Exemplo: git checkout nova-funcionalidade

Criar e já mudar para a nova branch: git checkout -b nome-da-branch
Exemplo: git checkout -b ajuste-layout

## 3. Trabalhar na Nova Branch
Depois de mudar para a nova branch, você pode:

Editar arquivos

Adicionar mudanças com git add

Comitar com git commit

As alterações ficarão isoladas da branch principal até que você faça o merge.

##  4. Juntar (Merge) as Branches
Voltar para a branch principal (geralmente main): git checkout main

Fazer o merge da outra branch: git merge nome-da-branch
Exemplo: git merge nova-funcionalidade
Se não houver conflitos, o Git fará o merge automaticamente.

## 5. Lidando com Conflitos de Merge
Se dois arquivos foram modificados nas duas branches, o Git mostrará um conflito.

Você verá algo assim no arquivo:
<<<<<<< HEAD
código da branch atual
==========
código da branch que está sendo mesclada
>>>>>>> nova-funcionalidade

Como Resolver:
Edite o arquivo e escolha qual código manter (ou combine os dois).

Salve o arquivo.

Adicione o arquivo resolvido: git add nome_arquivo

Finalize o merge com: git commit

## 6. Apagar uma Branch
Depois que a branch for mesclada e não for mais necessária, você pode apagá-la:

Apagar branch local: git branch -d nome-da-branch
Apagar branch remota: git push origin --delete nome-da-branch

## 7. Boas Práticas com Branches
Dê nomes descritivos: ajuste-footer, bug-login, feature-api.

Faça git pull antes do merge para evitar conflitos desnecessários.

Trabalhe em pequenas tarefas por branch (evita bagunça e facilita revisão).

## 8. Visualizar as Branches
Listar todas as branches: git branch
Ver branches locais e remotas: git branch -a

