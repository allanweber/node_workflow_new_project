# Workflow de projetos

> Arquivos e configurações para inicio de projeto Java Script

# Author
> Allan Weber

**Passos para criação de um projeto Java script**

> ## .gitattributes
Configurações de final de linha para arquivos, normalizando para LF

> ## .editorconfig
Confguração dos comportamentos de formatação dos arquivos, para habilitar a formatação automática, configurar 'formatOnSave' (abaixo)

> ## formatOnSave
Formatar aquivos conforme EditorConfig e Prettier
* pressinar Crtl + , para abrir as preferências.
* ``` "[javascript]": {
        "editor.formatOnSave": true
        },
        "[json]": {
            "editor.formatOnSave": true
        },
        "[jsonc]": {
            "editor.formatOnSave": true
        }

> ## npm init -y
Inicializa o package.json, com -y para confirmar as questões que serão exibidas

> ## package.json
Informar dados do projeto, contatos, keywords e etc, e :
```
"scripts": {
    "start": "node src/index.js"
  },
```

> ## .npmrc
Configurações para NPM:
* "package-lock = false" - desativa o arquivo package-lock
* "progress = false" - desativa a barra de progresso
* "save-exact = true" - usa apenas versões exatas dos pacotes

> ## Instalar o eslint nas dependências de desenvolvimento
O EsLint valida o código de acordo com regras de boas práticas.

Rodar o comando:```npm i -D eslint```

> ## Instalar Prettier com configuração e plugin para eslint
O Prettier formata o código de acordo com regras de boas práticas.

Rodar o comando: ```npm i -D prettier eslint-config-prettier eslint-plugin-prettier```

> ## .prettierrc
Configurações para salvar os aquivos com a formatação correta de código.

> ## README.MD
Arquivo de descrição do projeto

> ## CHANGELOG.MD
Arquivo com as mudanças do projeto

> ## .gitignore
Estratégia de commit para o git

> ## Incializar o GIT
Rodar o comando: ```git init```

> ## .eslintignore
Configurações para ignorar arquivos que não deve rodar lint

> ## .eslintrc.json
Configurações para o eslint

> ## npm command prettier
Configurar comando que roda lint no projeto

Adicionar dentro de script no package.json a linha:

```"lint": "eslint src/**/*.js --fix",```

Fazendo o comando ```npm run lint``` no terminal, esse executará p lint e todos os aquivos da pasta src. O parâmetro **--fix** indica ao lint que ele deve tentar corrigir qualquer problema que venha a ocorrer.

