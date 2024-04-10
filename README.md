
<h1 align="center">Dicas e Auxiliares</h1>

<br/>
<p align="center">
<img src="https://img.shields.io/badge/-GERAL-informational"/>
</p>

 - Dicas de [PHP Conceitual](https://github.com/maniero/SOpt/blob/master/PHP/Conceptual.md)
 - Usar PHP Intephesense na versão 1.8.0
 - Visualize perfeitamente seus dados JSON instantaneamente em gráficos [JSON Crack](https://jsoncrack.com/)
 - [Como configurar o Xampp para trabalhar com HTTPS - SSL](https://www.youtube.com/watch?v=0kvOQJj7gVk)
 - Compilando o Bootstrap com SASS e NPM [Tutorial Youtube](https://www.youtube.com/watch?v=VAet5wEoOWU&t) e [Auxiliar DOC](https://diegomariano.com/compilando-o-bootstrap-com-sass-e-npm/)

## 💻📊✔️Software de Gerenciamento de Projetos

- [Microsoft Project](https://project.microsoft.com/)
- [Trello](https://trello.com/)
- [Slack](https://slack.com/intl/pt-br)
- [Wekan(Kaban) - Open Source](https://github.com/wekan/wekan)


## 🪑📊Sistemas de gerenciamento de banco de dados(SGBD)

- [DBeaver Community](https://dbeaver.io/download/)
- [HeidiSQL](https://www.heidisql.com/download.php)
- [SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16)


## 💻➡️✔️Ferramentas de Logica De Programação

- Interface para criar diagramas como fluxogramas, wireframes, diagramas UML [Diagrams.net(draw.io)](https://app.diagrams.net/)
- Ferramenta gráfica para escrever e executar fluxogramas  [Flowgorithm](http://www.flowgorithm.org/download/index.html)

## 🪑💹 Banco de dados
 
 - [Tipos de campos e exemplos de valores](http://www.fititnt.org/off/tipos-de-campos-e-exemplos-de-valores-empresas-em-sistemas-cnpj-cep.html)
 - [SQL Convertion](https://www.sqlines.com/online)
 
 
 ## 📄README :

- [Um modelo para fazer bom README](https://gist.github.com/lohhans/f8da0b147550df3f96914d3797e9fb89)
- [Como escrever um README incrível no seu Github](https://www.alura.com.br/artigos/escrever-bom-readme)
- [Exemplo de README Ecoleta](https://github.com/tgmarinho/README-ecoleta/blob/master/README.md)

 ## 👨‍💻	:octocat: Github :

- [Git, desfazendo commits](https://brorlandi.github.io/git-desfazendo-commits)
- [Como modificar o repositorio remoto no Git](https://wallacemaxters.com.br/blog/50/como-modificar-o-repositorio-remoto-no-git)
- [Diferença entre "git add --all", "git add ." e "git add -u"](https://pt.stackoverflow.com/questions/326160/diferen%C3%A7a-entre-git-add-all-git-add-e-git-add-u)
- Geekhunter [13 comandos Git mais usados](https://blog.geekhunter.com.br/comandos-git-mais-utilizados/#Git_add)
- Desfazer o último commit e remover as alterações do stage area `git reset HEAD~1` | `(git reset HEAD~2 volta 2 Commits)`
- Desfazer o último commit e manter as alterações no stage area  `git reset --soft HEAD~1`
- Fusão sem verificar os 2 Historicos de commits  `git pull origin master --allow-unrelated-histories` ->
- [Resolvendo o erro “fatal: refusing to merge unrelated histories” no Git](https://community.umbler.com/br/t/resolvendo-o-erro-fatal-refusing-to-merge-unrelated-histories-no-git/657)

<details>
  <summary>Como mudar o username e email dos commits já feitos</summary>
 <br>
<pre>
  <code class="language-git">
git filter-branch --env-filter '
EMAIL_ANTIGO="seu-email-antigo@example.com"
NOME_CORRETO="Nome correto"
EMAIL_CORRETO="seu-email-correto@example.com"
if [ "$GIT_COMMITTER_EMAIL" = "$EMAIL_ANTIGO" ]
then
    export GIT_COMMITTER_NAME="$NOME_CORRETO"
    export GIT_COMMITTER_EMAIL="$EMAIL_CORRETO"
fi
if [ "$GIT_AUTHOR_EMAIL" = "$EMAIL_ANTIGO" ]
then
    export GIT_AUTHOR_NAME="$NOME_CORRETO"
    export GIT_AUTHOR_EMAIL="$EMAIL_CORRETO"
fi
' --tag-name-filter cat -- --branches --tags
  </code>
</pre>

</details>



## ✔️Emoji

- Enciclopédia de Emoji [Emojipedia](https://emojipedia.org/)
- Emojis Padrao WhatsApp [GetEmoji](https://getemoji.com/)
- Emoji Geral [Git Markdown emoji](https://itinerant.tistory.com/60)
- Emojis do Github [Github Emoji](https://github.com/StylishThemes/GitHub-Dark/wiki/Emoji)
- [Emoji-Cheat-Sheet](https://github.com/ikatyang/emoji-cheat-sheet)
- Emojis Padrao Markdown [Gist Emoji Markdown](https://gist.github.com/rxaviers/7360908)
 
## 📍Icons

- Font Awesome [Icons](https://fontawesome.com/icons)
- Logotipos de linguagens e ferramentas de desenvolvimento [DevIcon](https://github.com/devicons/devicon/tree/master/icons)
- Icones Simples [Simple Icons](https://simpleicons.org/)
- Favicons [Icons8](https://icons8.com.br/icons/set/popular)

## 🔖Badges

- 150+ Badges for GitHub [DEV Community](https://dev.to/envoy_/150-badges-for-github-pnk)
- Badges Readme [Badges 4 README.md](https://github.com/alexandresanlim/Badges4-README.md-Profile)
- Criador de Badges e Exemplos[Shields.io](https://shields.io/)


## 💻🧾 Editores

<details>
  <summary>📌Mardown</summary>
 <br>

- Editor e Auxiliador Online de Markdown [Readme.SO](https://readme.so/pt/editor)
- Editor de Markdown no navegador [StackEdit](https://stackedit.io/)
- Editor Online [Dillinger](https://dillinger.io/)
- Editor de Markdown Software [Typora](https://typora.io/)
 
</details>


<details>
  <summary>👨🏻‍💻Editor de código e IDE</summary>
 <br>

- IDE abrangente para desenvolvedores .NET e C++ [Visual Studio 2022](https://visualstudio.microsoft.com/pt-br/vs/)
- Editor de Código-Fonte excelente para Web [Visual Studio Code](https://code.visualstudio.com/)
- Editor de texto [Notepad++](https://notepad-plus-plus.org/downloads/)
- Editor de Código-Fonte Multi-Plataforma [Sublime Text](https://www.sublimetext.com/)
- IDE Python [PyCharm](https://www.jetbrains.com/pt-br/pycharm/)
 
</details>

<details>
  <summary>📚Auxiliares de Next.JS</summary>
 <br>

- Authentication for Next.js [NextAuth.js ](https://next-auth.js.org/)
- Ferramenta de banco de dados ORM [Prisma.IO](https://www.prisma.io/) 
- Criar sua biblioteca de componentes [shadcn/ui](https://ui.shadcn.com/)
- Biblioteca de componentes para React [Chakra UI](https://chakra-ui.com/)
- Biblioteca de componentes para o framework CSS Tailwind CSS [daisyUI](https://daisyui.com/)
- Framework de CSS [Tailwind CSS](https://tailwindcss.com/)
- Coleção de componentes para criar e-mails [React Email](https://react.email/) 
 
</details>



<details>
  <summary>📍Leitores de JSON</summary>
 <br>

- JSON Crack [JSONCrack](https://jsoncrack.com)

</details>
