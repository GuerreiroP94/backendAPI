# PreSystem.StockControl

Sistema de controle de estoque desenvolvido em .NET 8, com arquitetura em camadas, autenticação JWT e API RESTful documentada via Swagger.

## Descrição

O PreSystem.StockControl é uma solução robusta para o gerenciamento de estoque, permitindo o cadastro, consulta, atualização e remoção de produtos, componentes e movimentações de estoque. O sistema também oferece controle de usuários com diferentes níveis de acesso, autenticação segura via JWT e integração facilitada com frontends modernos (ex: React/Vite).

## Funcionalidades Principais

- **Gestão de Produtos**: Cadastro, consulta, atualização e exclusão de produtos e seus componentes.
- **Gestão de Componentes**: Controle detalhado de componentes, incluindo grupo, quantidade em estoque e quantidade mínima.
- **Movimentação de Estoque**: Registro de entradas e saídas, com rastreio de usuário responsável.
- **Gestão de Usuários**: Cadastro de usuários com diferentes papéis (ex: operador, administrador).
- **Autenticação JWT**: Segurança nas rotas da API, permitindo acesso apenas a usuários autenticados.
- **Swagger**: Documentação interativa da API para facilitar testes e integração.
- **CORS Configurado**: Permite integração com frontends hospedados em outras origens (ex: localhost:5173).

## Tecnologias Utilizadas

- .NET 8
- ASP.NET Core Web API
- Entity Framework Core
- JWT Bearer Authentication
- Swagger/OpenAPI
- FluentValidation

## Como Executar Localmente

1. **Clone o repositório:**

2. **Configure as variáveis de ambiente:**
   - Edite o arquivo `appsettings.json` com as configurações do banco de dados e JWT (`JwtSettings:Secret`, `Issuer`, `Audience`).

3. **Restaure as dependências:**

4. **Atualize o banco de dados (se necessário):**

5. **Execute a aplicação:**

6. **Acesse a documentação da API:**
   - [http://localhost:5000/swagger](http://localhost:5000/swagger) (ou porta configurada)

## Estrutura do Projeto

- `PreSystem.StockControl.WebApi/` - API principal e configurações
- `PreSystem.StockControl.Application/` - Serviços, DTOs e regras de negócio
- `PreSystem.StockControl.Domain/` - Entidades e interfaces de domínio
- `PreSystem.StockControl.Infrastructure/` - Persistência e repositórios

## Contribuição

Contribuições são bem-vindas! Siga os passos abaixo:

1. Fork este repositório
2. Crie uma branch: `git checkout -b minha-feature`
3. Faça suas alterações e commit: `git commit -m 'Minha nova feature'`
4. Envie para o repositório remoto: `git push origin minha-feature`
5. Abra um Pull Request
