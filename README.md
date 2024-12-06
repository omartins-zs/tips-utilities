<h1 align="center">Dicas e Auxiliares</h1>

<br />
<p align="center">
	<img src="https://img.shields.io/badge/-GERAL-informational" />
</p>

<ul>
 <li>Visualize perfeitamente seus dados JSON instantaneamente em gráficos <a href="https://jsoncrack.com/editor">JSON Crack</a>
	</li>
	<li>Compilando o Bootstrap com SASS e NPM <a href="https://www.youtube.com/watch?v=VAet5wEoOWU&tk">Tutorial
			Youtube</a> e <a href="https://diegomariano.com/compilando-o-bootstrap-com-sass-e-npm/">Auxiliar DOC</a>
	</li>
	<li>Avatar Aleatorio <a href="https://avatar.iran.liara.run/public">Avatar Liara</a>
	</li>
</ul>

<h2>💻📊✔️Software de Gerenciamento de Projetos</h2>

<ul>
	<li><a href="https://project.microsoft.com/">Microsoft Project</a></li>
	<li><a href="https://trello.com/">Trello</a></li>
	<li><a href="https://slack.com/intl/pt-br">Slack</a></li>
	<li><a href="https://github.com/wekan/wekan">Wekan(Kaban) - Open Source</a></li>
</ul>

<h2>🪑📊Sistemas de gerenciamento de banco de dados(SGBD)</h2>

<ul>
	<li><a
			href="https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16">SQL
			Server Management Studio (SSMS)</a></li>
	<li><a href="https://dbeaver.io/download/">DBeaver Community</a></li>
	<li><a href="https://www.heidisql.com/download.php">HeidiSQL</a></li>
</ul>

<h2>💻➡️✔️Ferramentas de Lógica de Programação</h2>
<ul>
	<li>Interface para criar diagramas como fluxogramas, wireframes, diagramas UML <a
			href="https://app.diagrams.net/">Diagrams.net(draw.io)</a></li>
	<li>Ferramenta gráfica para escrever e executar fluxogramas <a
			href="http://www.flowgorithm.org/download/index.html">Flowgorithm</a></li>
</ul>

<h2>🪑💹 Banco de Dados</h2>
<ul>
	<li><a href="http://www.fititnt.org/off/tipos-de-campos-e-exemplos-de-valores-empresas-em-sistemas-cnpj-cep.html">Tipos
			de campos e exemplos de valores</a></li>
	<li><a href="https://www.sqlines.com/online">SQL Convertion</a></li>
</ul>

<h2>📄README</h2>
<ul>
	<li><a href="https://gist.github.com/lohhans/f8da0b147550df3f96914d3797e9fb89">Um modelo para fazer bom README</a>
	</li>
	<li><a href="https://www.alura.com.br/artigos/escrever-bom-readme">Como escrever um README incrível no seu
			Github</a></li>
	<li><a href="https://github.com/tgmarinho/README-ecoleta/blob/master/README.md">Exemplo de README Ecoleta</a></li>
</ul>

<h2>👨‍💻 :octocat: Github</h2>
<ul>
	<li><a href="https://brorlandi.github.io/git-desfazendo-commits">Git, desfazendo commits</a></li>
	<li><a href="https://wallacemaxters.com.br/blog/50/como-modificar-o-repositorio-remoto-no-git">Como modificar o
			repositorio remoto no Git</a></li>
	<li><a href="https://pt.stackoverflow.com/questions/326160/diferen%C3%A7a-entre-git-add-all-git-add-e-git-add-u">Diferença
			entre "git add --all", "git add ." e "git add -u"</a></li>
	<li>Geekhunter <a href="https://blog.geekhunter.com.br/comandos-git-mais-utilizados/#Git_add">13 comandos Git mais
			usados</a></li>
	<li>Desfazer o último commit e remover as alterações do stage area <code>git reset HEAD~1</code> |
		(<code>git reset HEAD~2</code> volta 2 Commits)</li>
	<li>Desfazer o último commit e manter as alterações no stage area <code>git reset --soft HEAD~1</code></li>
	<li>Fusão sem verificar os 2 Historicos de commits <code>git pull origin master --allow-unrelated-histories</code>
	</li>
	<li><a
			href="https://community.umbler.com/br/t/resolvendo-o-erro-fatal-refusing-to-merge-unrelated-histories-no-git/657">Resolvendo
			o erro “fatal: refusing to merge unrelated histories” no Git</a></li>
<li>
  <details>
    <summary>Como mudar o username e email dos commits já feitos</summary>
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

 <pre>
      <code class="language-git">
       git filter-branch --env-filter '
    NOME_CORRETO="Seu Nome Correto"
    EMAIL_CORRETO="seu-email-correto@example.com"

    if [ "$GIT_COMMITTER_EMAIL" != "$EMAIL_CORRETO" ]
    then
        export GIT_COMMITTER_NAME="$NOME_CORRETO"
        export GIT_COMMITTER_EMAIL="$EMAIL_CORRETO"
    fi

    if [ "$GIT_AUTHOR_EMAIL" != "$EMAIL_CORRETO" ]
    then
        export GIT_AUTHOR_NAME="$NOME_CORRETO"
        export GIT_AUTHOR_EMAIL="$EMAIL_CORRETO"
    fi
' --tag-name-filter cat -- --branches --tags
      </code>
    </pre>
   
  </details>
</li>
	<li>
		<details>
			<summary>Alterando a Mensagem de Commits Específicos</summary>
			<ul>
				<li>
					<strong>1. Utilize o comando <code>git rebase -i HEAD~n</code></strong>
					<p>Onde <code>n</code> é o número de commits a partir do HEAD que você quer incluir no rebase.</p>
					<pre><code>git rebase -i HEAD~3</code></pre>
				</li>
				<li>
					<strong>2. Escolha o Commit para Editar</strong>
					<p>Encontre o commit cuja mensagem você deseja alterar e substitua <code>pick</code> por
						<code>reword</code> (ou <code>r</code>) e Salve e feche o editor, Exemplo:
					</p>
					<pre><code>reword abc1234 Mensagem antiga
pick def5678 Outro commit
pick ghi9012 Outro commit</code></pre>
				</li>
				<li>
					<strong>3. Edite a Mensagem do Commit</strong>
					<p>O Git abrirá o editor novamente, desta vez para você editar a mensagem do commit especificado.
						Edite a mensagem conforme necessário, salve e feche o editor</p>
				</li>
				<li>
					<strong>4. Continue o Rebase</strong>
					<p>Após editar a mensagem, o rebase interativo continuará automaticamente. Se houver conflitos, você
						precisará resolvê-los antes de continuar.</p>
					<pre><code>git rebase --continue</code></pre>
				</li>
				<li>
					<strong>5. Forçar o Push para o Repositório Remoto</strong>
					<p>Após completar o rebase, você precisará forçar o push para atualizar o repositório remoto com as
						mudanças.</p>
					<pre><code>git push --force</code></pre>
				</li>
			</ul>
		</details>
	</li>
<li>
		<details>
			<summary>Alterando Commits após fazer Checkout para Commit Anterior(Recuperando e Atualizando uma Branch a Partir de um Commit Anterior)</summary>
			<ul>
				<li>
					<p>
						Se você voltou apenas para um commit anterior (usando git checkout <hash>), e fez novos commits no estado de detached HEAD, mas agora quer que esses novos commits substituam o terceiro commit, aqui está o que fazer sem criar uma nova branch:
						
						
						# Force a branch principal para o estado atual
						git branch -f (nome-da-branch) HEAD
						
						# Volte para a branch principal
						git checkout (nome-da-branch)
						
						# Envie as alterações para o repositório remoto, sobrescrevendo o histórico
						git push --force
						
						
						git push origin HEAD:(nome-da-branch)--force
					</p>
				

				</li>
			</ul>
		</details>
	</li>
</ul>

<h2>✔️Emoji</h2>
<ul>
	<li>Enciclopédia de Emoji <a href="https://emojipedia.org/">Emojipedia</a></li>
	<li>Emojis Padrao WhatsApp <a href="https://getemoji.com/">GetEmoji</a></li>
	<li>Emoji Geral <a href="https://itinerant.tistory.com/60">Git Markdown emoji</a></li>
	<li>Emojis do Github <a href="https://github.com/StylishThemes/GitHub-Dark/wiki/Emoji">Github Emoji</a></li>
	<li><a href="https://github.com/ikatyang/emoji-cheat-sheet">Emoji-Cheat-Sheet</a></li>
	<li>Emojis Padrao Markdown <a href="https://gist.github.com/rxaviers/7360908">Gist Emoji Markdown</a></li>
</ul>

<h2>📚Auxiliares de Next.JS</h2>
<ul>
	<li>Authentication for Next.js <a href="https://next-auth.js.org/">NextAuth.js</a></li>
	<li>Ferramenta de banco de dados ORM <a href="https://www.prisma.io/">Prisma.IO</a></li>
	<li>Criar sua biblioteca de componentes <a href="https://ui.shadcn.com/">shadcn/ui</a></li>
	<li>Biblioteca de componentes para React <a href="https://chakra-ui.com/">Chakra UI</a></li>
	<li>Biblioteca de componentes para o framework CSS Tailwind CSS <a href="https://daisyui.com/">daisyUI</a></li>
	<li>Framework de CSS <a href="https://tailwindcss.com/">Tailwind CSS</a></li>
	<li>Coleção de componentes para criar e-mails <a href="https://react.email/">React Email</a></li>
</ul>

<h2>📍Icons</h2>
<ul>
	<li>Font Awesome <a href="https://fontawesome.com/icons">Icons</a></li>
	<li>Logotipos de linguagens e ferramentas de desenvolvimento <a
			href="https://github.com/devicons/devicon/tree/master/icons">DevIcon</a></li>
	<li>Icones Simples <a href="https://simpleicons.org/">Simple Icons</a></li>
	<li>Favicons <a href="https://icons8.com.br/icons/set/popular">Icons8</a></li>
</ul>

<h2>🔖Badges</h2>
<ul>
	<li>150+ Badges for GitHub <a href="https://dev.to/envoy_/150-badges-for-github-pnk">DEV Community</a></li>
	<li>Badges Readme <a href="https://github.com/alexandresanlim/Badges4-README.md-Profile">Badges 4 README.md</a></li>
	<li>Criador de Badges e Exemplos <a href="https://shields.io/">Shields.io</a></li>
</ul>

<h2>💻🧾 Editores</h2>
<ul>
	<li>
		<details>
			<summary>📌Markdown</summary>
			<ul>
				<li>Editor e Auxiliador Online de Markdown <a href="https://readme.so/pt/editor">Readme.SO</a></li>
				<li>Editor de Markdown no navegador <a href="https://stackedit.io/">StackEdit</a></li>
				<li>Editor Online <a href="https://dillinger.io/">Dillinger</a></li>
				<li>Editor de Markdown Software <a href="https://typora.io/">Typora</a></li>
			</ul>
		</details>
	</li>
	<li>
		<details>
			<summary>👨🏻‍💻Editor de código e IDE</summary>
			<ul>
				<li>IDE abrangente para desenvolvedores .NET e C++ <a
						href="https://visualstudio.microsoft.com/pt-br/vs/">Visual Studio 2022</a></li>
				<li>Editor de Código-Fonte excelente para Web <a href="https://code.visualstudio.com/">Visual Studio
						Code</a></li>
				<li>Editor de texto <a href="https://notepad-plus-plus.org/downloads/">Notepad++</a></li>
				<li>Editor de Código-Fonte Multi-Plataforma <a href="https://www.sublimetext.com/">Sublime Text</a></li>
				<li>IDE Python <a href="https://www.jetbrains.com/pt-br/pycharm/">PyCharm</a></li>
			</ul>
		</details>
	</li>
</ul>
