# REST-API_Tabela-FIP


API REST desenvolvida utilizando Spring Boot e Maven, com Java 17, para facilitar o acesso a informações de veículos da Tabela Fipe. Esta API foi criada para simplificar a busca por marcas, modelos, anos e valores de veículos (carros, motos, caminhões), oferecendo um ponto de integração eficiente para o consumo desses dados.

## Funcionalidades
A API oferece quatro endpoints principais, que permitem acessar as informações da Tabela Fipe:

/marcas: Retorna a lista de marcas de veículos disponíveis na Tabela Fipe.

/modelos/{marca}: Dado o ID de uma marca, retorna a lista de modelos de veículos associados a essa marca.

/anos/{marca}/{modelo}: Dado o ID de uma marca e de um modelo, retorna os anos de fabricação disponíveis para aquele modelo.

/valor/{marca}/{modelo}/{ano}: Retorna o valor de mercado de um modelo específico de veículo para um determinado ano de fabricação, conforme a Tabela Fipe.

## Tecnologias Utilizadas
Spring Boot: Utilizado para estruturar a aplicação, facilitar o gerenciamento de dependências, e fornecer uma abordagem rápida para construir APIs RESTful.

Maven: Gerenciamento de dependências e automação do build, simplificando a configuração do projeto e garantindo consistência entre ambientes.

Java 17: A versão mais recente de suporte de longo prazo (LTS) do Java, que oferece melhorias de performance e novos recursos que ajudam a construir uma API robusta.

RestTemplate / WebClient: Para fazer as requisições HTTP à API da Tabela Fipe, o Spring oferece duas opções que permitem a fácil integração com APIs externas.

## Como a API Funciona
Consulta à API da Tabela Fipe: Cada endpoint da API realiza uma requisição para os respectivos endpoints da API pública da Tabela Fipe. Dependendo do endpoint solicitado, a API faz chamadas GET para buscar as marcas, modelos, anos ou valores de veículos.

Resposta ao Cliente: A resposta da API é um JSON contendo as informações solicitadas pelo cliente, facilitando a integração dos dados em aplicações diversas.

## Exemplo de Uso

![image](https://github.com/user-attachments/assets/20faeae6-4886-48ef-b709-06c5e5373945)


![image](https://github.com/user-attachments/assets/6e4f1117-21cb-425b-8053-34aaddadfe9b)
