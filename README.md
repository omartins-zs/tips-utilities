# Dicas e Auxiliares

<p align="center">
  <img src="https://img.shields.io/badge/-GERAL-informational" />
</p>

- Visualize perfeitamente seus dados JSON instantaneamente em gráficos: [JSON Crack](https://jsoncrack.com/editor)  
- Compilando o Bootstrap com SASS e NPM: [Tutorial Youtube](https://www.youtube.com/watch?v=VAet5wEoOWU&tk) | [Auxiliar DOC](https://diegomariano.com/compilando-o-bootstrap-com-sass-e-npm/)  
- Avatar Aleatório: [Avatar Liara](https://avatar.iran.liara.run/public)

---

## 💻📊✔️ Software de Gerenciamento de Projetos

- [Microsoft Project](https://project.microsoft.com/)  
- [Trello](https://trello.com/)  
- [Slack](https://slack.com/intl/pt-br)  
- [Wekan (Kanban) – Open Source](https://github.com/wekan/wekan)

---

## 🪑📊 SGBD

- [SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16)  
- [DBeaver Community](https://dbeaver.io/download/)  
- [HeidiSQL](https://www.heidisql.com/download.php)

---

## 💻➡️✔️ Ferramentas de Lógica de Programação

- Diagrams.net (draw.io) — [Criar diagramas (fluxogramas, wireframes, UML)](https://app.diagrams.net/)  
- Flowgorithm — [Escrever e executar fluxogramas](http://www.flowgorithm.org/download/index.html)

---

## 🪑💹 Banco de Dados

- [Tipos de campos e exemplos de valores (CNPJ, CEP, etc.)](http://www.fititnt.org/off/tipos-de-campos-e-exemplos-de-valores-empresas-em-sistemas-cnpj-cep.html)  
- [SQL Convertion (sqlines)](https://www.sqlines.com/online)

---

## 📄 README

- [Modelo para um bom README (Gist)](https://gist.github.com/lohhans/f8da0b147550df3f96914d3797e9fb89)  
- [Como escrever um README incrível (Alura)](https://www.alura.com.br/artigos/escrever-bom-readme)  
- [Exemplo de README Ecoleta](https://github.com/tgmarinho/README-ecoleta/blob/master/README.md)

---

## 👨‍💻 :octocat: GitHub

- [Git: desfazendo commits](https://brorlandi.github.io/git-desfazendo-commits)  
- [Modificar repositório remoto no Git](https://wallacemaxters.com.br/blog/50/como-modificar-o-repositorio-remoto-no-git)  
- [Diferença entre `git add --all`, `git add .` e `git add -u`](https://pt.stackoverflow.com/questions/326160/diferen%c3%a7a-entre-git-add-all-git-add-e-git-add-u)  
- [13 comandos Git mais usados (Geekhunter)](https://blog.geekhunter.com.br/comandos-git-mais-utilizados/#Git_add)  
- Desfazer o último commit e remover do stage area:  
  ```bash
  git reset HEAD~1        # volta 1 commit
  git reset HEAD~2        # volta 2 commits
  ```  
- Desfazer o último commit e manter no stage area:  
  ```bash
  git reset --soft HEAD~1
  ```  
- Fusão sem verificar históricos:  
  ```bash
  git pull origin master --allow-unrelated-histories
  ```  
- [Resolver “fatal: refusing to merge unrelated histories”](https://community.umbler.com/br/t/resolvendo-o-erro-fatal-refusing-to-merge-unrelated-histories-no-git/657)

<details>
  <summary>Como mudar username &amp; email dos commits já feitos</summary>

  ```bash
  git filter-branch --env-filter '
    EMAIL_ANTIGO="seu-email-antigo@example.com"
    NOME_CORRETO="Nome correto"
    EMAIL_CORRETO="seu-email-correto@example.com"
    if [ "$GIT_COMMITTER_EMAIL" = "$EMAIL_ANTIGO" ]; then
      export GIT_COMMITTER_NAME="$NOME_CORRETO"
      export GIT_COMMITTER_EMAIL="$EMAIL_CORRETO"
    fi
    if [ "$GIT_AUTHOR_EMAIL" = "$EMAIL_ANTIGO" ]; then
      export GIT_AUTHOR_NAME="$NOME_CORRETO"
      export GIT_AUTHOR_EMAIL="$EMAIL_CORRETO"
    fi
  ' --tag-name-filter cat -- --branches --tags
  ```
</details>

<details>
  <summary>Alterando a mensagem de commits específicos</summary>

  1. `git rebase -i HEAD~n` (substitua `n` pelo número de commits)  
  2. No editor, troque `pick` por `reword` no commit desejado  
  3. Edite a mensagem quando o Git abrir o editor novamente  
  4. Resolva conflitos (se houver) e execute:
     ```bash
     git rebase --continue
     ```  
  5. Force o push:
     ```bash
     git push --force
     ```
</details>

<details>
  <summary>Alterando commits após detached HEAD</summary>

  Se você criou novos commits em detached HEAD e quer reaplicar na sua branch:

  ```bash
  # forçar a branch principal para o HEAD atual
  git branch -f nome-da-branch HEAD
  # voltar para a branch principal
  git checkout nome-da-branch
  # push forçado para o remoto
  git push origin HEAD:nome-da-branch --force
  ```
</details>

---

## ✔️ Emoji

- [Emojipedia](https://emojipedia.org/)  
- [GetEmoji (padrão WhatsApp)](https://getemoji.com/)  
- [Git Markdown Emoji](https://itinerant.tistory.com/60)  
- [GitHub Emoji](https://github.com/StylishThemes/GitHub-Dark/wiki/Emoji)  
- [Emoji Cheat Sheet](https://github.com/ikatyang/emoji-cheat-sheet)  
- [Gist Emoji Markdown](https://gist.github.com/rxaviers/7360908)

---

## 📚 Auxiliares de Next.js

- [NextAuth.js (autenticação)](https://next-auth.js.org/)  
- [Prisma ORM](https://www.prisma.io/)  
- [shadcn/ui (biblioteca de componentes)](https://ui.shadcn.com/)  
- [Chakra UI](https://chakra-ui.com/)  
- [daisyUI (Tailwind CSS)](https://daisyui.com/)  
- [Tailwind CSS](https://tailwindcss.com/)  
- [React Email (componentes para e-mail)](https://react.email/)

---

## 📍 Ícones

- [Font Awesome Icons](https://fontawesome.com/icons)  
- [DevIcon (linguagens e ferramentas)](https://github.com/devicons/devicon/tree/master/icons)  
- [Simple Icons](https://simpleicons.org/)  
- [Icons8 (favicons)](https://icons8.com.br/icons/set/popular)
- [Heroicons](https://heroicons.com/)

---

## 🔖 Badges

- [150+ Badges for GitHub (DEV Community)](https://dev.to/envoy_/150-badges-for-github-pnk)  
- [Badges4-README.md](https://github.com/alexandresanlim/Badges4-README.md-Profile)  
- [Shields.io (criador de badges)](https://shields.io/)

---

## 💻🧾 Editores

<details>
  <summary>📌 Markdown</summary>

  - [Readme.so (editor online)](https://readme.so/pt/editor)  
  - [StackEdit](https://stackedit.io/)  
  - [Dillinger](https://dillinger.io/)  
  - [Typora](https://typora.io/)
</details>

<details>
  <summary>👨🏻‍💻 Código &amp; IDE</summary>

  - [Visual Studio 2022](https://visualstudio.microsoft.com/pt-br/vs/)  
  - [Visual Studio Code](https://code.visualstudio.com/)  
  - [Notepad++](https://notepad-plus-plus.org/downloads/)  
  - [Sublime Text](https://www.sublimetext.com/)  
  - [PyCharm](https://www.jetbrains.com/pt-br/pycharm/)
</details>

---

## 🔔 Alerts

- [Sweet Alert](https://sweetalert.js.org/)  
- [SweetAlert2](https://sweetalert2.github.io/)  
- [Notyf](https://carlosroso.com/notyf/)  
- [Alertify JS](https://alertifyjs.com/)  
- [Toastr](http://www.toastrjs.com/)  
- [Laravel Noty](https://github.com/rsmalc/laravel-noty)
- [Notify.js](https://notifyjs.jpillora.com/)

---

## 🖼️ Placeholders

Sim! O site [placehold.co](https://placehold.co/) é um gerador de imagens placeholder para usar em desenvolvimento (tamanho, texto, cor de fundo e da fonte).  
Alternativas:

- [via.placeholder.com](https://via.placeholder.com)  
  - Exemplo: `https://via.placeholder.com/300x200`
- [dummyimage.com](https://dummyimage.com)  
  - Exemplo: `https://dummyimage.com/300x200/000/fff&text=Texto`
- [placeimg.com](https://placeimg.com)  
  - Exemplo: `https://placeimg.com/300/200/tech`
- [picsum.photos](https://picsum.photos)  
  - Exemplo: `https://picsum.photos/300/200`

---

- [Logos de Times](https://logodetimes.com/)
