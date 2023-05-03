# AzureFunctions

  

### **1. Crear credencial azure para deploy con GitHub Actions**
```
az ad sp create-for-rbac --name "MyApplication" --role contributor --scopes /subscriptions/SubscriptionId/resourceGroups/MyApps --sdk-auth
```
```
 az ad sp create-for-rbac --name "MyFunctions" --role contributor --scopes /subscriptions/c8eb5574-f147-4230-978a-06596636cfee/resourceGroups/MyApps --sdk-auth
```

> **MyApplication** es el nombre de la aplicación a crear en Azure Active Directory
>
> **SuscriptionId**  es Id de la suscripción de Azure. Este valor se puede obtener con el comando az cli `az account list -o table`
> 
> **MyApps**  es el nombre del resource group.