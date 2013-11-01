Existem alguns comandos que não são muito usados pelos usuários do NPM, porém podem fazer toda a diferença quando se trata de agilidade ou resolução de problemas.

### Mais comandos e menos JSON...

Criar um `package.json` é algo prático e inteligente se você não quiser quebrar as dependências do seu projeto, mas até mesmo essas tarefas triviais podem ficar massantes se for necessário executá-las diversas vezes ao dia, para isso foi criado o `npm init`. Como o próprio nome já sugere, ele serve para inicializar um `package.json` apenas respondendo perguntas, nada mais de JSON :)

<script type="text/javascript" src="http://asciinema.org/a/6172.js" id="asciicast-6172" async></script>

Para adicionar e remover pacotes também não é mais necessário abrir o seu `package.json`, podemos usar o `npm install pacote` e o `npm remove pacote` juntamente com o argumento `--save`, isso fará com que o npm adicione e remova pacotes automaticamente das dependências do seu projeto. Precisa adicionar ou remover um pacote das dependências de desenvolvimento? Sem problemas, utilize o argumento `--save-dev`.

<script type="text/javascript" src="http://asciinema.org/a/6173.js" id="asciicast-6173" async></script>

Note que o script é inteligente o suficiente para adicionar o `~` na frente de cada versão do pacote, restringindo assim os próximos updates para as versões menores de cada pacote, evitando quebra de compatibilidade.

### Dicas rápidas

* Pesquise por pacotes usando o próprio npm
    * `npm find command line kitties`
* Pesquise por um determinado dado de um pacote
    * `npm view schemator repository.url`
* Liste recursivamente todas as dependências do seu projeto no estilo árvore
    * `npm list`
* Faça o update das suas dependências
    * `npm update`
* Faça o update dos seus pacotes globais (`supervisor`, `forever`...)
    * `sudo npm update -g`
* Troque a versão do seu projeto
    * `npm version 0.0.2`
* Use abreviaturas dos comandos
    * `ls` para `list`, `s` para `search`, `i` para `install`, `r` para `remove`...
* Veja a ajuda para qualquer comando no npm
    * `npm help search`
* Limpe o cache do npm (útil para os momentos "wtf is happening")
    * `npm cache clean`

### Ajude a expandir e manter atualizado este documento

Encontrou algum erro? Deseja acrescentar ou remover informações? Acesse o link abaixo e envie um pull request imediatamente.
