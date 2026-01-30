### ScreenSound - Gestão de Músicas e Artistas 🎵

<p align="center">
<img width="461" height="95" alt="image" src="https://github.com/user-attachments/assets/aa70ea6f-5792-4860-a34d-5d365efc6d2f" />
</p>

O ScreenSound é uma aplicação Java robusta desenvolvida com Spring Boot para gerenciar um catálogo personalizado de artistas e suas músicas. O foco principal deste desafio é a implementação de um sistema de persistência de dados relacional e a criação de consultas inteligentes utilizando o Spring Data JPA.

## 🚀 Funcionalidades
- Cadastrar Artistas: Registro de artistas com definição de tipo (Solo, Dupla ou Banda).
- Cadastrar Músicas: Vinculação de músicas a artistas já existentes no banco de dados.
- Listar Músicas: Exibição de todo o acervo musical cadastrado.
- Buscar Músicas por Artista: Filtro dinâmico para encontrar todas as obras de um cantor ou banda específica.
- Pesquisar Dados do Artista: Integração (opcional) com APIs externas ou busca por inteligência artificial para obter informações biográficas do artista selecionado.

## 🛠️ Tecnologias Utilizadas
- Java 17: Linguagem base para a lógica de negócio.
- Spring Boot 3: Framework para gerenciamento da aplicação.
- Spring Data JPA: Para facilitar a comunicação com o banco de dados e criação de queries automáticas.
- PostgreSQL: Banco de dados relacional para armazenamento seguro dos dados.

## ⚙️ Configuração e Execução
### 1. Requisitos
- JDK 17+
- PostgreSQL instalado.
### 2. Configuração do Banco de Dados
- Configurar as variaveis de ambiente.
- No arquivo src/main/resources/application.properties, configure o acesso ao seu banco:
```
spring.datasource.url=jdbc:postgresql://localhost:5432/screensound
spring.datasource.username=${seu_usuario}
spring.datasource.password=${sua_senha}
spring.jpa.hibernate.ddl-auto=update
```
### 3. Rodando o Projeto
```
# Clone o repositório
git clone https://github.com/Medeiros20/screensound.git

# Acesse a pasta
cd screensound

# Execute via Maven
./mvnw spring-boot:run
```
