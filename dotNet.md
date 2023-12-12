# Entity Framework Migration

dotnet ef migrations add initial -- X.DataAccess(DbContext bulunan projeniz) --startup-project X.API

dotnet ef database update --project X.DataAccess --startup-project X.API

************************************************************************
