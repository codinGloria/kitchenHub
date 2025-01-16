<h1 align="center"> Projeto: Kitchen Hub 🍕 </h1>
<br>

O Kitchen Hub é um projeto criado para facilitar o gerenciamento de restaurantes e pedidos, trazendo organização para as operações do dia a dia. Além de ser uma ótima oportunidade para praticar Java, Spring Boot e PostgreSQL, o projeto também é um jeito de explorar conceitos de microsserviços, Docker e integração entre sistemas.

## 📂 Estrutura do Projeto

Será dividido em duas aplicações principais, e em ambas devemos:
- Criar tabelas no banco de dados automaticamente ao rodar a aplicação (caso não existam).
- Conectar ao banco de dados PostgreSQL em um container Docker.

### 1) *restaurant-management-service*
Responsável pelo gerenciamento de restaurantes e seus recursos associados.

#### Entidades e Funcionalidades:
- **Empresa**: CRUD para empresas associadas a restaurantes.
- **Restaurante**: CRUD para informações de restaurantes.
- **Cardápio**: CRUD para os cardápios disponíveis em cada restaurante.
- **Prato**: CRUD para os pratos do cardápio.

---

### 2) *order-management-service*
Responsável pelo gerenciamento de pedidos realizados pelos clientes.

#### Entidades e Funcionalidades:
- Cliente: CRUD para cadastro de clientes.
- Pedido: CRUD para pedidos realizados.
- Item: CRUD para itens do pedido.

#### Requisitos:
- Comunicar-se com o serviço **restaurant-management-service** através de uma API REST:
  - Requisição `GET` para buscar o objeto `Cardápio`, contendo os pratos relacionados.

## 📊 Modelo de Entidades
![image](https://github.com/user-attachments/assets/1a74698c-2ef8-4383-8529-d25f36ecb170)


## ⚙️ Como Executar o Projeto
[adicionar após criar o projeto]
  
## 📬 Comunicação entre Serviços
No order-management-service, um cliente HTTP acessará o endpoint do restaurant-management-service para obter informações de cardápios e pratos.

- Endpoints:
    - `GET ...`: Retorna o cardápio com seus pratos relacionados.

## 🛠️ Tecnologias Utilizadas
- Backend: 
  - Spring Boot,
  - Java (21 LTS)
- Dados:
  - Banco: PostgreSQL,
  - JPA e Hibernate
- Containerização:
  - Docker
- Integração:
  - REST APIs (Comunicação entre microsserviços)

## 🚀 Funcionalidades a serem adicionadas
- Testar a persistência de dados no Docker após reinicialização.
- Implementar autenticação entre os serviços.
- Criar testes unitários e de integração para ambos os serviços.
- Documentar as APIs com Swagger.

## 🧑‍💻 Contato
Para mais informações ou dúvidas sobre o projeto, entre em contato:
<div align="center">
<h2> Glória Braz
<br> codingloria@gmail.com
<br><br>
<a href="https://www.linkedin.com/in/codingloria/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
</div>
