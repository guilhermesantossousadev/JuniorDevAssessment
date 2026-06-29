# Junior Dev Assessment

Projeto de avaliacao tecnica para desenvolvedor junior com backend .NET, banco SQLite e frontend Vue/Vite.

## Arquitetura

```text
API/                  API ASP.NET Core
Core/                 Servicos, repositorios e acesso a dados
Entidades/            Modelos de dominio
FrontEnd/ProvaDev/    Interface Vue 3 com Vite
ProvaDevJr.sln        Solucao .NET
```

## Tecnologias

- .NET 6.
- ASP.NET Core Web API.
- Swagger/OpenAPI.
- SQLite.
- Dapper e Dapper.Contrib.
- Vue 3.
- Vite.

## Como rodar a API

Na raiz do repositorio:

```bash
dotnet restore
dotnet run --project API/API.csproj
```

Em ambiente de desenvolvimento, a documentacao Swagger fica disponivel no endereco exibido pelo terminal, geralmente:

```text
https://localhost:7000/swagger
```

## Como rodar o frontend

```bash
cd FrontEnd/ProvaDev
npm install
npm run dev
```

## Banco de dados

O projeto usa SQLite. O arquivo `API/Enterprise.db` e usado pela aplicacao durante o desenvolvimento.

## Limpeza de repositorio

Pastas geradas por IDE ou build, como `.vs/`, `bin/`, `obj/` e `node_modules/`, nao devem ser versionadas. Elas podem ser recriadas localmente pelos comandos de build e restore.
