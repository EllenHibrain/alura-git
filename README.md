## <center>Comandos Git</center>

|COMANDOS | VARIAÇÃO | FUNÇÃO |
|---|---|---|
|**version** |**--version**|Mostra a versão instalada; |
|**init**|**init** <br> **init --bare** *(usado para tornar o repositório remoto)* |Inicia o repositório ; <br> Repositório puro, conterá as alterações feitas, e não a cópia de cada arquivo; |
|**status**|**status**|Verifica e documenta o estado do repositório atual;
|**config**|**config --local user.nome** <br> **config --local user.email** <br> **config --global user.nome** <br> **config --global user.email**|Declara o **nome** do usuário no **repositório local**; <br> Declara o **email** do usuário no **repositório local**; <br> Declara o **nome** do usuário no **repositório global**; <br> Declara o **email** do usuário no **repositório global**;|
|**add**|**add .** <br> **add *identificação***|Adiciona todas as últimas configurações, sem nomeá-las; <br> Abre o arquivo para adicionar commit's;|
|**commit**|**commit –m " "**|Usado para adicionar mensagem ao *commit* que será salvo;|
|**config**|**config --global** *ou* **local**|Modifica as configurações. <br> **global:** Máquina como um todo; <br> **local:** Cada projeto;|
|**log**|**log** <br> **log --oneline** <br> **log -p**|Mostra as commits <br> Mostra as commits resumidas em uma **única linha**; <br> Mostra as informações de commit com **as alterações detalhadas**;|
|**remote**|**remote** <br> **remote add *nomedesejado*** + ***endereçodorepositório*** <br> **remote rename *nomeatual*** + ***novonome*** <br> **remote -v**|Mostra os repositórios reconhecidos; <br> Adiciona o repositório citado; <br> Renomeia repositório; <br> Mostra o caminho do repositório; 
|**clone**|**clone *endereçodorepositório***|Clona o repositório em questão;|
|**push**|**push *identificação*** + ***linhadetrabalho*** *(ex:master)*|Envia dados de alterações para o repositório desejado, como *commits* e **tags**;|
|**pull**|**pull *identificação*** + ***linhadetrabalho*** *(ex:master)*|Copia os dados de alterações do repositório desejado;|
|**branch**|**branch** <br> **branch *identificação***|Consultar *branches* criadas; <br> Adiciona uma nova *branche*;|
|**checkout**|**checkout *identificação*** <br> **checkout --*identificação***|Muda para a *branche* ou *commit* citada; <br> Descarta última alteração que não foi *commitada*;|
|**merge**|**merge *branch1* *branch2***|Cria uma *commit* em comum para unir as *branches*;|
|**rebase**|**rebase *branch1* *branch2*** <br><br> ![Imagem demonstrando diferença entre merge e rebase](GetImage.png)|Alinha *branches* e suas *commits* de forma ordenada;|
|**reset**|**reset HEAD *nomedoarquivo***|Desfaz alteração que estava em **aberto**, ou seja, que ainda não havia sido *commitado*;|
|**revert**|**revert *códigodocommit***|Reverte *commit* salvo;|
|**stash**|**stash** <br> **stash list** <br> **stash *númerodoitem*** <br> **stash drop** <br> **stash pop**|Guarda alterações para depois, **sem commitá-las**; <br> Lista *stashs* existentes; <br> Recupera alteração salva para depois; <br> Apaga alteração salva para depois; <br> Recupera alteração salva para depois, **e apaga** da lista;|
|**diff**|**diff** <br> **diff *númerocommit1* .. *númerocommit2***|Mostra alterações que ainda não foram commitadas; <br> Mostra alterações feitas de uma *commit* até outra *commit*;
|**tag**|**tag** <br> **tag –a *nomedesejado***|Mostra as tags existentes; <br> Gera uma nova tag;| 
<br>

**HEAD:** Estado atual do nosso código, ou seja, onde o Git nos colocou  
**Working tree:** Local onde os arquivos realmente estão sendo armazenados e editados  
**index:** Local onde o Git armazena o que será commitado, ou seja, o local entre a working tree e o repositório Git em si.

##### -Tecla Q para sair do git log -p  

**-Para voltar no tempo nos commits:**  
**git log --oneline**
Anote o número de identificação do *commit* que deseja ir
**git checkout *númerodeIDE***
*Caso queira salvar as alterações feitas nesse *commit*, crie uma nova *branch* para realizar as alterações, e depois **sincronize** com merge ou rebase à *branch* principal.
