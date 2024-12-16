# url-shortner
Let's Build It: Url Shortner Course

# Infrastructure as Code

### Log Into Azure
```bash
az login
https://learn.microsoft.com/en-us/cli/azure/
```

### Create Resource Group 
```bash
az group create --name urlshortner-dev --location westus2
```

### Create User for GitHub Actions
```bash
az ad sp create-for-rbac --name "GitHub-Actions-SP"
                         --role contributor
                         --scopes /subscriptions/5dfba529-06b2-47fe-9044-f201549de733
                         --sdk-auth
```

### Configure a federated identity credentials on an app
https://learn.microsoft.com/en-us/entra/workload-id/workload-identity-federation-create-trust?pivots=identity-wif-apps-methods-azp#configure-a-federated-identity-credential-on-an-app

