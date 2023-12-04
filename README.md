# Creating resources by using the Microsoft .NET SDK v3

## Prerequisites
* Azure CLI
* C# Extension for VsCode
* .NET 6 target framework
```
az login
az group create --location <myLocation> --name az204-cosmos-rg
az cosmosdb create --name <myCosmosDBacct> --resource-group az204-cosmos-rg
# Retrieve the primary key
az cosmosdb keys list --name <myCosmosDBacct> --resource-group az204-cosmos-rg
```
Install ```dotnet add package Microsoft.Azure.Cosmos```

Run:
```
dotnet build
dotnet run
```

To clean the Resources execute:
`az group delete --name az204-cosmos-rg --no-wait`

Happy Coding :shipit: