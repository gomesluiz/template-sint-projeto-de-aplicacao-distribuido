# Instala os pacotes necessários para rodar a aplicação

## Entity Framework
dotnet add package Microsoft.EntityFrameworkCore
dotnet add package Microsoft.EntityFrameworkCore.Design
dotnet add package Microsoft.EntityFrameworkCore.Tools

## Sqlite
dotnet add package Microsoft.EntityFrameworkCore.Sqlite

## Sqlserver
dotnet add package Microsoft.EntityFrameworkCore.SqlServer

# Criar os migrations de banco de dados
dotnet ef migrations add InitialCreate --context TodoContext --output-dir Data/Migrations
dotnet ef database update --context TodoContext
