# Guia de Comandos do Yarn

Este documento descreve os comandos mais comuns do Yarn, um gerenciador de pacotes para JavaScript que facilita o gerenciamento de dependências e automação de tarefas em projetos.


---

## Sumário
- [Gerenciamento de Pacotes](#gerenciamento-de-pacotes)
- [Gerenciamento de Dependências](#gerenciamento-de-dependências)
- [Scripts e Execução](#scripts-e-execução)
- [Cache](#cache)
- [Verificação e Diagnóstico](#verificação-e-diagnóstico)
- [Utilidades](#utilidades)
- [Build e Produção](#build-e-produção)
- [Trabalhando com Monorepos](#trabalhando-com-monorepos)

---

## Gerenciamento de Pacotes

- **`yarn init`**: Inicializa um novo projeto e cria um arquivo `package.json`.
- **`yarn add [pacote]`**: Instala uma dependência no projeto (na versão mais recente).
  - **`yarn add [pacote]@[versão]`**: Instala uma dependência de uma versão específica.
  - **`yarn add [pacote] --dev`**: Instala uma dependência como dependência de desenvolvimento.
- **`yarn remove [pacote]`**: Remove uma dependência do projeto.
- **`yarn upgrade [pacote]`**: Atualiza uma dependência para a última versão disponível.
- **`yarn upgrade [pacote]@[versão]`**: Atualiza uma dependência para uma versão específica.

---

## Gerenciamento de Dependências

- **`yarn install`**: Instala todas as dependências listadas no arquivo `package.json`.
- **`yarn install --frozen-lockfile`**: Garante que nenhuma alteração seja feita no arquivo `yarn.lock` ao instalar dependências.
- **`yarn install --force`**: Reinstala todas as dependências, ignorando o cache.

---

## Scripts e Execução

- **`yarn run [script]`**: Executa um script definido no `package.json`.
- **`yarn start`**: Atalho para o script `start` no `package.json`.
- **`yarn test`**: Atalho para o script `test` no `package.json`.

---

## Cache

- **`yarn cache list`**: Lista os pacotes armazenados no cache do Yarn.
- **`yarn cache clean`**: Limpa o cache do Yarn.

---

## Verificação e Diagnóstico

- **`yarn why [pacote]`**: Explica por que um pacote está instalado, mostrando suas dependências e versões.
- **`yarn outdated`**: Lista as dependências que têm versões mais recentes disponíveis.

---

## Utilidades

- **`yarn global add [pacote]`**: Instala um pacote globalmente.
- **`yarn global remove [pacote]`**: Remove um pacote instalado globalmente.
- **`yarn global list`**: Lista os pacotes instalados globalmente.

---

## Build e Produção

- **`yarn build`**: Executa o script de build definido no `package.json`.
- **`yarn clean`**: Limpa os arquivos gerados durante o build (se definido como script no `package.json`).

---

## Trabalhando com Monorepos

- **`yarn workspace [nome] [comando]`**: Executa comandos em um workspace específico dentro de um monorepo.
- **`yarn workspaces list`**: Lista os workspaces do projeto.

---

## Contribuições

Contribuições são bem-vindas! Caso queira adicionar mais informações ou sugerir melhorias, fique à vontade para enviar um pull request ou abrir uma issue.

---

## Licença

Este guia é fornecido sob a licença MIT. Sinta-se livre para utilizá-lo e adaptá-lo conforme necessário.

---
