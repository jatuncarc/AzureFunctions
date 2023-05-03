
# AzureFunctions

  

### **1. Crear credencial azure para deploy con GitHub Actions**
```
az ad sp create-for-rbac --name "AppName" --role contributor --scopes /subscriptions/SuscriptionId/resourceGroups/RSBootcamp --sdk-auth

```

> **AppName** es el nombre de la aplicación a crear en Azure Active Directory
> **SuscriptionId**  es Id de la suscripción de Azure. Este valor se puede obtener con el comando az cli `az account list -o table`