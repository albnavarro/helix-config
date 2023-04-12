# helix-config

## helix config with some vim/neovim fallback.

### compile tresseter-pug:

```
hx --grammar fetch
hx --grammar build
```

create runtime/queries/pug/highlights.scm<br/>
( copy from runtime/grammars/sources/pug/queries/highlights.scm )

docs: https://docs.helix-editor.com/guides/adding_languages.html

## At this time Helix supporto only one LSP

### JS/CSS/HTML LSP
```
npm i -g vscode-langservers-extracted
npm install -g typescript-language-server typescript
npm install -g prettier
```

#### Additional dependencies untile helix support multiple LSP: 

```
npm install -g eslint
npm install -g stylelint
```

#### Run additional dependencies on cli:

```
npm/npx eslint "**/*.js" --fix
npm/npx stylelint "**/*.js" --fix
npm/npx prettier --write "**/*.pug" 
npm/npx prettier --write "**/*.twig" 
```