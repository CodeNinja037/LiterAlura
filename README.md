# LiterAlura
Catálogo de livros LiterAlura
Literalura - Projeto de Busca e Cadastro de Livros via API Gutendex
Descrição
Literalura é um projeto desenvolvido em Java com Spring Boot que permite buscar livros na API pública Gutendex pelo título e salvar automaticamente os dados desses livros e seus autores em um banco de dados PostgreSQL. A aplicação possui uma interface simples via terminal para realizar buscas, listar livros, autores, filtrar autores por ano de nascimento e listar livros por idioma. O projeto é ideal para praticar consumo de APIs REST, manipulação de JSON, persistência de dados relacionais e construção de interfaces simples em Java.

Funcionalidades
Buscar livros pelo título na API Gutendex.

Salvar livros e autores no banco PostgreSQL automaticamente após a busca.

Listar todos os livros registrados no banco.

Listar todos os autores registrados.

Listar autores por ano de nascimento.

Listar livros por idioma.

Tecnologias Utilizadas
Java 21

Spring Boot 3.1.4

PostgreSQL

Spring Data JPA

RestTemplate para consumo de API REST

JSON (org.json) para manipulação dos dados da API

Maven para gerenciamento de dependências

Estrutura do Projeto
com.alura.literalura.dto: Classes DTO para mapeamento das respostas da API.

com.alura.literalura.service: Lógica de negócio e integração com API e banco.

com.alura.literalura.model: Entidades JPA para livros e autores.

com.alura.literalura.repository: Repositórios JPA para acesso ao banco.

com.alura.literalura.client: Cliente HTTP para requisições à API Gutendex.

com.alura.literalura: Classe principal e configuração da aplicação.

Como Rodar o Projeto
Clone este repositório:


git clone https://github.com/seuusuario/literalura.git
cd literalura
Configure o banco PostgreSQL e crie um banco de dados para o projeto.

Ajuste as configurações de conexão no application.properties:

properties

spring.datasource.url=jdbc:postgresql://localhost:5432/seubanco
spring.datasource.username=seuusuario
spring.datasource.password=suasenha
spring.jpa.hibernate.ddl-auto=update
Compile e execute a aplicação com Maven:


mvn clean install
mvn spring-boot:run
Utilize o menu no terminal para buscar livros e interagir com a base de dados.

Exemplo de Uso
Ao escolher a opção de busca, digite o título do livro desejado (ex: "Dom Casmurro").

Caso o livro seja encontrado na API, ele será salvo no banco automaticamente.

Use as outras opções para listar livros, autores, ou filtrar por ano e idioma.

Desafios Encontrados
Tratamento correto do encoding do título para buscas na API evitando erros de URL.

Mapeamento correto da estrutura JSON complexa da API para objetos Java com DTOs.

Evitar duplicidade de autores no banco, garantindo que relacionamentos fossem consistentes.

Criação de uma interface simples e intuitiva via terminal para facilitar a interação do usuário.

Configuração e ajuste do ambiente Spring Boot e conexão com PostgreSQL para persistência eficaz.

Próximos Passos
Implementar testes automatizados para garantir a robustez das buscas e persistência.

Adicionar paginação e filtros avançados para a listagem de livros e autores.

Criar interface web para facilitar o uso do sistema.

Contato
Projeto desenvolvido por Luiz Fernando Ribeiro.

<img width="1908" height="1079" alt="image" src="https://github.com/user-attachments/assets/9b4263c4-17be-4615-8b63-8285c780a7f0" />

<img width="1919" height="1074" alt="image" src="https://github.com/user-attachments/assets/ff3fa2a5-7272-430c-a87e-744bcb816c10" />

