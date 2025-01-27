# Blog-Pessoal

O **Blog-Pessoal** é um projeto desenvolvido como parte do programa **Generation Brasil**, com o objetivo de criar uma aplicação para gerenciar postagens de blogs de maneira prática e intuitiva. Através de uma API REST, o sistema permite a criação, visualização, edição e exclusão de postagens, além de funcionalidades como autenticação de usuários e gerenciamento de temas.

## Estrutura do Projeto

| Camada       | Elementos                                          |
|--------------|----------------------------------------------------|
| Model        | UsuarioModel, PostagemModel, TemaModel             |
| Repository   | UsuarioRepository, PostagemRepository, TemaRepository |
| Service      | UsuarioService, PostagemService, TemaService       |
| Controller   | UsuarioController, PostagemController, TemaController |

## Funcionalidades da API

A API foi desenvolvida para gerenciar as postagens e os temas de forma eficiente, com suporte a operações como:

- **GET**: Visualizar todas as postagens, buscar por ID ou filtrar por título.
- **POST**: Criar novas postagens e temas.
- **PUT**: Atualizar postagens e temas existentes.
- **DELETE**: Excluir postagens e temas por ID.

### Respostas de Status

| Código | Descrição                |
|--------|--------------------------|
| 200    | Sucesso!                 |
| 201    | Objeto persistido!       |
| 204    | Objeto excluído!         |
| 400    | Erro na requisição!      |
| 401    | Acesso não autorizado!   |
| 403    | Acesso proibido!         |
| 404    | Objeto não encontrado!   |
| 500    | Erro na aplicação!       |

## Testes Realizados

### 1. Gerenciamento de Postagens
| Teste               | Descrição                                                             | Resultado Esperado                                 |
|---------------------|-----------------------------------------------------------------------|--------------------------------------------------|
| ID Válido           | Verificar se a postagem é retornada corretamente por um ID válido.   | Status HTTP 200 e dados da postagem retornados. |
| ID Inválido         | Verificar se retorna erro ao buscar postagem inexistente.            | Status HTTP 404 e mensagem de erro.             |
| Criação de Postagem | Verificar se uma postagem válida é criada com sucesso.               | Status HTTP 201 e detalhes da postagem criada.  |

### 2. Gerenciamento de Temas
| Teste               | Descrição                                                             | Resultado Esperado                                 |
|---------------------|-----------------------------------------------------------------------|--------------------------------------------------|
| Tema Válido         | Verificar se o tema é retornado corretamente por um ID válido.       | Status HTTP 200 e dados do tema retornados.     |
| Tema Inválido       | Verificar se retorna erro ao buscar tema inexistente.                | Status HTTP 404 e mensagem de erro.             |
| Criação de Tema     | Verificar se um tema válido é criado com sucesso.                    | Status HTTP 201 e detalhes do tema criado.      |

## Stack Utilizada

- **Java 17**  
- **Spring Boot**  
- **Spring Web**  
- **Spring Data JPA**  
- **Spring Security**  
- **Validation**  
- **MySQL Driver**

## Colaboradora

| [![DandaraaAfroo](https://github.com/DandaraaAfroo.png?size=100)](https://github.com/DandaraaAfroo) |
| :-------------------------------------------------------------------------------------------------: |
| [DandaraaAfroo](https://github.com/DandaraaAfroo)                                                  |
