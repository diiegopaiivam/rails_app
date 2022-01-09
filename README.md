<h2 align=center>
<img src="https://miro.medium.com/max/1400/1*_uQ2O1kMA6DBI3_nNOBVOA.png" />
</h2>

<div align="center">

![Rails_Badge][rails] ![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)

</div>

<h3 align="center">

Projeto **Open Source** desenvolvido para servir de modelo Padrão para desenvolvimento de aplicações **Rails** com **Postgres** utilizando a tecnologia ***Docker***.

</h3>

## **Tutorial para utilização do projeto**


#### **INSTALAÇÃO** 

#####  - **Clone o repositório git na sua máquina:**
    - git clone https://github.com/diiegopaiivam/rails_app.git
#####  - **Remova o remote origin do repositório através do seguinte comando:**
    - git remove remote origin
#####  - **Abra o arquivo docker-compose.yml e altere o parâmetro POSTGRESS_PASSWORD para uma senha da sua escolha**
#####  - **Dentro do seu terminal execute o comando:**
    - docker-compose run --no-deps web rails new . --force --database=postgresql 
  OBS.: Esse comando fará com que você crie uma aplicação rails dentro do container já preparada com as configurações do posrgres
##### - **Caso esteja em um ambiente linux será necessário alterar as permissões de usuário dos diretórios da aplicação. Você deverá executar o seguinte comando:**
    - sudo chown -R $USER:$USER .
##### - **Execute o comando para a aplicação realizar a instalação das gems que foram inseridas automaticamente no Gemfile**
    - docker-compose build
##### - **Próximo passo será inserir nossas credenciais de conexão com o banco dentro do arquivo config/database.yml**
    - o password do database.yml deverá ser o mesmo que foi inserido no docker-compose.yml
    - o host utilizado é o mesmo nome da imagem, ou seja "DB" 
    - o username é postgres
#### - **Próximo passo será subir os containers**
    - Execute o comando: docker-compose up
#### - **Execute o comando para criação dos bancos no postgres**
    - docker-compose run web rake db:create


## **Após seguir esses passos a aplicação estará pronta e exibida no localhost dentro da porta 3000**

## **LICENÇA**

Esse repositório está licenciado pela **MIT LICENSE**. Para mais informações detalhadas, leia o arquivo [LICENSE](./LICENSE) contido nesse repositório. 



<!-- Website Links -->

[rocketseat_site]: https://rocketseat.com.br/

<!-- Badges -->

[github_issues_badge]: https://img.shields.io/github/issues/x0n4d0/ecoleta?color=green

[repository_license_badge]: https://img.shields.io/github/license/x0n4d0/ecoleta

[rails]: https://img.shields.io/badge/rails-%23CC0000.svg?style=for-the-badge&logo=ruby-on-rails&logoColor=white

[npm_version_badge]: https://img.shields.io/badge/npm-6.14.4-red

[web_react_badge]: https://img.shields.io/badge/web-react-blue

[mobile_react-native_badge]: https://img.shields.io/badge/mobile-react%20native-blueviolet

[server_nodejs_badge]: https://img.shields.io/badge/server-nodejs-important

<!-- Techs -->

[react]: https://reactjs.org/

[typescript]: https://www.typescriptlang.org/

[node]: https://nodejs.org/en/

[leaflet]: https://react-leaflet.js.org/en/

[ibge_api]: https://servicodados.ibge.gov.br/api/docs/localidades?versao=1

[ibge_api_ufs]: https://servicodados.ibge.gov.br/api/docs/localidades?versao=1#api-UFs-estadosGet

[ibge_api_municipios]: https://servicodados.ibge.gov.br/api/docs/localidades?versao=1#api-Municipios-estadosUFMunicipiosGet

[vscode]: https://code.visualstudio.com/

[react_native]: http://www.reactnative.com/

[stackedit]: https://stackedit.io

[vscode_sqlite_extension]: https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite

[markdown_emoji]: https://gist.github.com/rxaviers/7360908

[commitlint]: https://github.com/conventional-changelog/commitlint

[express]: https://expressjs.com/

[cors]: https://expressjs.com/en/resources/middleware/cors.html

[knex]: http://knexjs.org/

[sqlite3]: https://github.com/mapbox/node-sqlite3

[tsnode]: https://github.com/TypeStrong/ts-node

[feather_icons]: https://feathericons.com/

[insomnia]: https://insomnia.rest/

[react_leaflet]: https://react-leaflet.js.org/

[react_router_dom]: https://github.com/ReactTraining/react-router/tree/master/packages/react-router-dom

[react_icons]: https://react-icons.github.io/react-icons/

[axios]: https://github.com/axios/axios
