### Como Executar o Projeto local

#### Pré-requisitos para Executar
1. **.NET Core**
2. **SQL Server**
3. **RabbitMQ**

#### Configuração Inicial

1. **Configurar o banco de dados**

 A configuração, foi feita seguindo abaixo. 
 Ou seja, crie um banco de dados chamado Ambev em sua instancia e ajuste a stringa abaixo conforme necessário para o seu ambiente
  "Server=localhost\\SQLEXPRESS;Database=Ambev;Trusted_Connection=True;TrustServerCertificate=True"
   

2. **Rodar as Migrations**
Uma migration inicial está criada, basta executar Update-Database.

3. **Configuração RabbitMQ**
 As configurações do rabbit encontra-se em também em launchsettings.json, assim como a connectionstring.
basta alterar de acordo com sua instancia local do rabbitmq:
        "RABBITMQHOSTNAME": "localhost",
        "RABBITMQUSERNAME": "guest",
        "RABBITMQPASSWORD": "guest",
        "RABBITMQVIRTUALHOST": "localhost"


