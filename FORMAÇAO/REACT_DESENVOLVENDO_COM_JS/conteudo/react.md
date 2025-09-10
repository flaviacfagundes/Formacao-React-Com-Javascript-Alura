
# Criando uma aplicação front-end com pacotes do Node.js

Para trabalhar com o **React**, por exemplo, existem diferentes ferramentas que nos auxiliam a criar um projeto. Uma dessas ferramentas é o **Vite**, que é capaz de criar automaticamente um projeto base para trabalharmos com um framework front-end, além de disponibilizar um servidor que realiza operações automatizadas.

Para utilizar o **Vite**, devemos executar o seguinte comando:

~~~~
npm create vite@latest
~~~~

O `npm create` é um dos comandos disponibilizados pelo **NPM** (*Node Package Manager*, ou *Gerenciador de pacotes do Node*, do inglês). O NPM é um programa que vem instalado junto com o **Node** e que é capaz de instalar ou executar um pacote via linha de comando.

---

# O arquivo package.json

É muito comum que haja um ou mais pacotes “principais” do projeto e que eles tenham o auxílio de vários outros pacotes, que trazem soluções prontas para diversos tipos de problemas.

Todos esses pacotes também precisam ser instalados no seu computador para serem aproveitados. É aí que entra o arquivo `package.json` ele documenta todos os pacotes necessários para o funcionamento do projeto.

Vamos entender os atributos desse **JSON**:

- `name` *(nome)*: o nome do projeto Node.js.
- `private` *(privado)*: define se o seu projeto será privado ou se ele estará disponível para que outras pessoas da comunidade possam utilizá-lo.
- `version` *(versão)*: a versão atual do projeto. O **NPM** utiliza o chamado versionamento semântico (*SemVer*). Você pode ler mais sobre isso nesse artigo.
- `type` *(tipo)*: o tipo de modularização que será utilizada no projeto. O tipo padrão é commonjs, mas hoje em dia é recomendado utilizarmos o module, para seguir as versões mais recentes do **ECMAScript**.
- `scripts`: essa sessão tem alguns scripts pré-definidos, mas você também pode definir os seus personalizados.
- `dependencies` *(dependências)*: define a lista de pacotes necessários para executar seu projeto num ambiente de produção.
- `devDependencies` *(dependências de desenvolvimento)*: define a lista de pacotes necessários para executar o projeto em um ambiente de desenvolvimento e de testes.

---
