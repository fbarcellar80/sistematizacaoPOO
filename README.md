# Sistematizacao POO

# Sistema de Controle de Pacotes
Esta aplicação segue práticas de Programação Orientadaa Objetos, usa Spring Boot para facilitar o desenvolvimento, e utiliza o Maven para gerenciamento de dependências. O Postman foi empregado para testar e validar as operações da API REST.
Foi utilizado ainda o banco de dados MySQL par armazenar os dados depacotes.

# Funcionalidades:

Cadastro de Pacotes: A API permite o cadastro de novos pacotes, incluindo informações como código de rastreamento, data de recebimento, status, mensageiro e data de entrega.
Listagem de Pacotes: Oferece um endpoint para listar todos os pacotes armazenados no sistema.
Detalhes de um Pacote: Possui um endpoint que fornece detalhes de um pacote específico com base no seu identificador.
Atualização de Pacotes: Permite a atualização das informações de um pacote existente, utilizando seu identificador.
Exclusão de Pacotes: Possui um endpoint para remover um pacote com base no seu identificador.

# Implementação:

Entidade PackageEntity: Representa a estrutura de dados para os pacotes e é persistida no banco de dados.
Repositório PackageRepository: Fornece métodos para operações no banco de dados relacionadas aos pacotes.
Controlador PackageController: Gerencia as requisições HTTP relacionadas aos pacotes, implementando os endpoints mencionados acima.
Inicializador de Dados DataInitializer: Popula o banco de dados com dados iniciais durante o início da aplicação.

#Como Utilizar:

Clone este repositório.
Configure um banco de dados MySQL e ajuste as credenciais no arquivo de configuração application.properties, que fica dentro de src/main/resources.
Execute a aplicação usando o Maven: mvn spring-boot:run.
Acesse a API através dos endpoints mencionados na descrição.
