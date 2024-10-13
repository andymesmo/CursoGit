## **Comandos mais usados no Git**:
![Logo do git](https://sujeitoprogramador.com/wp-content/uploads/2021/04/gitimage.png)

### **_Credencial_** : 	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

| Comando                    | Descrição                                  |
|----------------------------|---------------------------------------------|
| git remote -v             | Verifica os repositórios remotos conectados |
| git remote remove origin | Remove o repositório remoto "origin"       |


### **Parear com o github**:
``` ps
git branch -M main
git remote add  origin https://github.com/andymesmo/amazon.git
git push -u origin main
```

### **Configurar usuario e email no git**:
```ps
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@exemplo.com"
```

---

## Pirmeiro repositorio
```ps
cd Projetos/Python
git init
git add .
git commit -m "Inicializando projeto Python"
git remote add origin https://github.com/seu_usuario/projeto_python.git
git push -u origin main
```
---

### **Verificar as configurações no git**:
```ps
git config --global user.name
git config --global user.email
```

---

### **Observações**:
Configuração Local vs Global:

Se você usar o comando com a flag --global, as configurações serão aplicadas para todos os repositórios Git no seu sistema.

Se você quiser configurar o e-mail e nome de usuário apenas para um repositório específico (local), omita a flag --global:

* git config user.name "Seu Nome"
* git config user.email "seu-email@exemplo.com"


### **Verificar as configurações do git**:
git config --list


---

### **Comandos Git mais usados**:
|Descrição   |Comando   |
|---|---|
|1. Verificar o nome de usuário = 								|`git config --global user.name`
|2. Verificar o e-mail = 										|`git config --global user.email`
|3. Iniciar um repositório = 									|`git init`
|4. Clonar um repositório existente = 							|`git clone <url-do-repositorio>`
|5. Verificar o status dos arquivos no repositório = 			|`git status`
|6. Adicionar um arquivo ao índice (staging area) = 			|`git add <nome-do-arquivo>`
|7. Adicionar todos os arquivos ao índice = 					|`git add .`
|8. Criar um commit com mensagem = 								|`git commit -m "Mensagem do commit"`
|9. Verificar o histórico de commits = 							|`git log`
|10. Criar e mudar para um novo branch = 						|`git checkout -b <nome-do-branch>`
|11. Unir (merge) outro branch ao branch atual = 				|`git merge <nome-do-branch>`
|12. Enviar commits para o repositório remoto = 				|`git push origin <nome-do-branch>`
|13. Atualizar o repositório local com as mudanças remotas = 	|`git pull origin <nome-do-branch>`
|14. Excluir um branch local = 									|`git branch -d <nome-do-branch>`
|15. Verificar branches disponíveis = 							|`git branch`
|


### **Opções (ou "Atributos") mais comuns no Git**:

1. Adicionar uma mensagem ao commit = 								`-m`
2. Criar um novo branch e alternar para ele = 						`-b`
3. Excluir um branch local = 										`-d`
4. Listar todas as branches (locais e remotas) = 					`-a`
5. Forçar uma ação, como sobrescrever alterações = 					`-f`
6. Definir uma configuração global = 								`--global`
7. Alterar o último commit = 										`--amend`
8. Restauração forçada de um estado anterior = 						`--hard`
9. Remover arquivos da área de stage sem excluí-los do diretório = 	`--cached`
10. Associar o branch local ao branch remoto no primeiro push = 	`-u`

---

### **Para renomear uma branch no Git**:
* renomear branch atual: git branch -m <novo-nome-da-branch>
* renomear branch sem precisar estar nela: git branch -m <nome-antigo-da-branch> <novo-nome-da-branch>

---

### **Para atualizar a branch no repositório remoto**:
| Descrição                                | Comando                                                |
|----|----|
| Excluir a branch antiga no remoto:       | git push origin --delete `nome-antigo-da-branch`       |
| Enviar a branch renomeada para o remoto: | git push origin `novo-nome-da-branch`                  |
| Configurar o upstream (rastrear o novo branch remoto): | git push -u origin `novo-nome-da-branch` |




### **Para desfazer o uso do git init em um diretório**:
|   |   |
|---|---|
| rm -rf .git   |
| powersheel: 	| Remove-Item -Recurse -Force .git
| cmd: 			| rmdir /S /Q .git
| 




### **Atualizar o VSCode**:
* 1. Usar o comando Reload Window no VSCode:
* 2. Pressione Ctrl+Shift+P para abrir a paleta de comandos do VSCode.
* 3. Digite Reload Window e selecione essa opção.
* 4. Agurade recarregar a janela do VSCode, forçando a atualização do estado dos arquivos.


### RESOLVENDO ALGUNS ERROS 
---
#### NO PUSH
```ps
git pull origin main
git push origin main
git pull --rebase origin main
```

#### NA BRANCH
```ps
git branch
git checkout main
git checkout -b main
```

#### RENOMEANDO A BRANCH
```ps
git branch -m master main
git push origin --delete master
git push -u origin main
```

#### REMOVER BRANCH LOCAL
```ps
git branch -d master
```
