# commerce-backend
Projeto Inicial BackEnd

# Implementação dos endpoints

## Users
-**GET all users**

-**POST user**
    - é comum existir um query params para mudar o comportamento da busca
    - dados de entrada são obrigatórios
    - validação > funcionalidade
-**DELETE user by id**
    - é importante tipar a tabela do banco de dados
    - path params é sempre string
    - validamos se a id já existe
    - *correção acerca do vídeo:
    - [**refatorando para garantir a constraint Foreign Key**]
        - para validar se a id recebida começa com a letra “f” precisamos olhar para a posição [0] e não a [1]

## Tasks
-**GET all tasks**

-**POST task**
    - é comum existir um query params para mudar o comportamento da busca
    - dados de entrada são obrigatórios
        - porém algumas colunas no banco de dados são preenchidas automaticamente
    - validação > funcionalidade
-**PUT task by id**
    - é importante tipar a tabela do banco de dados
    - **[refatorando para garantir a constraint Foreign Key]
    - dados de entrada são opcionais
-**DELETE task by id**
    - path params é sempre string
    - **[refatorando para garantir a constraint Foreign Key]
    - validamos se a id já existe

## Users + Tasks
- **[POST user to task by ids]

- **[DELETE user from task by ids]
    - recebendo as ids via path params
-**GET all users with tasks**
    - recebendo as ids via path params
    - não se preocupe caso o fluxo não faça sentido na sua cabeça, com o tempo tudo fica mais claro
    - vídeo sem cortes para deixar o processo de desenvolvimento o mais transparente possível (na vida real é realmente tentativa e erro!)