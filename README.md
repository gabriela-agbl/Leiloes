<div align="center">
   <h1>🏷️ Sistema de Leilão Online</h1>

   Este é um sistema básico de leilões, desenvolvido em Java com integração a um banco de dados MySQL. Ele permite o cadastro, listagem e gerenciamento de produtos em leilão. O projeto foi criado com o objetivo de consolidar conceitos de programação orientada a objetos e manipulação de banco de dados.
</div>

<div align="center">
   <h2>📌 Funcionalidades</h2>
</div>

- **Cadastro de Produtos**: Permite inserir novos produtos para leilão, especificando nome e valor inicial.
- **Listagem de Produtos**: Exibe todos os produtos cadastrados com detalhes como ID, nome, valor e status.
- **Gerenciamento de Leilões**: Altera o status dos produtos para "vendido" após realizar uma venda.
- **Persistência de Dados**: Utiliza o banco de dados MySQL para armazenar informações.

<div aling="center">
   <h2>🛠️ Tecnologias Utilizadas</h2>
</div>

- **Java**: Linguagem principal do projeto.
- **Swing**: Para a interface gráfica.
- **MySQL**: Banco de dados relacional para armazenar os produtos.
- **JDBC**: Para conexão e manipulação do banco de dados.

<div align="center">
   <h2>🚀 Como Executar o Projeto</h2>
</div>

<div align="center"> 
   <h3>Pré-requisitos<h3>
</div>

- [Java JDK](https://www.oracle.com/java/technologies/javase-jdk-downloads.html) instalado.
- [MySQL](https://dev.mysql.com/downloads/mysql/) instalado.
- Um IDE com suporte a Java Swing, como **NetBeans**.

<div align="center">
   <h3>Passos</h3>
</div>

1. **Clone este repositório**:
   ```bash
   git clone https://github.com/Agbl09/Leiloes.git

2. **Configure o banco de dados**:
   - Crie um banco de dados chamado uc11:
     ```sql
     CREATE DATABASE uc11;
     
   - Crie a tabela de produtos com o seguinte script SQL:
     ```sql
     CREATE TABLE produtos (id INT AUTO_INCREMENT PRIMARY KEY, nome VARCHAR(100) NOT NULL, valor INT NOT NULL, status VARCHAR(20) DEFAULT 'A Venda');
     
3. **Configure a conexão com o bando de dados**:
   - Edite o arquivo `conectaDAO.java` para ajustar as credenciais do bando de dados:
     ```java
     conn = DriverManager.getConnection("jdbc:mysql://localhost/uc11?user=root&password=");
     
4. **Implemente o projeto na sua IDE**:
   - Importe o projeto em sua IDE(por exemplo, NetBeans).
   - Compile e execute a classe principal para iniciar o sistema.

<div aling="center">
   <h2>📂 Estrutura do Projeto</h2>
</div>

   ```plaintext
Leiloes/
├── cadastroVIEW.java       # Interface para cadastro de produtos
├── listagemVIEW.java       # Interface para listagem e gerenciamento de produtos
├── conectaDAO.java         # Classe para conexão com o banco de dados
├── ProdutosDAO.java        # Lógica de acesso e manipulação dos dados
└── README.md               # Documentação do projeto
   ```

<div align="center">
   <h2>📋 Como Contribuir</h2>
</div>

   1. Faça um fork deste repositório.
      
   2. Crie uma branch para sua feature:
      ```bash
      git checkout -b minha-feature
      
   3. Faça suas alterações e realize um commit:
      ```bash
      git commit -m "Adicionada nova feature"
      
   4. Envie para o repositório remoto:
      ```bash
      git push origin minha-feature
   5. Abra um Pull Request neste repositório.

<div align="center">
   <h2>📝 Licença</h2>

   Este projeto foi desenvolvido para fins educacionais e está disponível para uso e modificação conforme necessário.

   Feito por [Gabriela Rodrigues](https://github.com/Agbl09)
   
![](https://private-user-images.githubusercontent.com/74038190/240885497-49abd3ca-b048-4f27-b7e0-ea6a7b172ac3.gif?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM4NDU5ODIsIm5iZiI6MTczMzg0NTY4MiwicGF0aCI6Ii83NDAzODE5MC8yNDA4ODU0OTctNDlhYmQzY2EtYjA0OC00ZjI3LWI3ZTAtZWE2YTdiMTcyYWMzLmdpZj9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjEwVDE1NDgwMlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTdmZDJhOGYzNTc1ODEyODkxODIyNzFkNmU3YmM0MjExYTFkODk1NzVkZWNjOGEwMWEwNWU4MjQwMWY5YThlYTEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.dv2KEqB-SIvKq2rtlRGr-BhMmV1z88s_yorB61xAkso)

</div>