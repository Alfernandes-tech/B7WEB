[⬅️ Voltar para o Índice Principal](../learningLog.md)


### 📌 Módulo 04: Git + GitHub

#### 💡 Curiosidades & Descobertas
- Ainda no básico, mas interessante começar a entender as branchs... Sendo:
  - `git branch` - para listar as atuais no diretório.
  - `git branch <nome_branch>` - para criação de nova branch.
  - `git switch <nome_branch>` - para poder alterar a branch em uso ou exibição.
  - `git merge <nome_branch>` - para poder fundir (merge) a branch escolhida para a atual.


- Outro ponto que achei importante foi que quando tentei utilizar o `git log` para verificar tudo, pude aprender que a apresentação vai ser feita através de um pager que apresenta algumas informações das quais para apresentar as demais é preciso dar "enter" ou "espaço" e que para sair o "control-c" não funciona mas que é preciso enviar "q" de quit para poder finalizar o pager

  - `git revert <hash>` - Cria um **novo commit** desfazendo o que aquele commit antigo fez. É o mais seguro porque não apaga o histórico de commits (ótimo quando o código já foi pro GitHub).
  
  - `git reset <hash>` - Volta a linha do tempo para o commit indicado. Se usado com `--hard`, apaga as alterações posteriores; se usado sem `--hard`, desfaz os commits mas deixa o código intacto na tela para você refazer.

  - `git stash` - É a "gaveta temporária". Salva alterações inacabadas que ainda não quero commitar para limpar a branch. Depois, uso `git stash pop` para recuperar tudo de onde parei.

  - `Ao usar branch -d` - Podemos estar excluindo uma branch (Mas comumente usada após finalizar as funções daquela branch e realizar o merge para a 'master')

  - `git merge --abort` - Para abortar um merge que travou ou esta em conflito

[⬅️ Voltar para o Índice Principal](../learningLog.md)
