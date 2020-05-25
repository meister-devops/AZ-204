# Implement solutions that use virtual machines

## Azure CLI

[Azure CLI Reference](https://docs.microsoft.com/en-us/cli/azure/reference-index?view=azure-cli-latest)

[Azure CLI Query](https://docs.microsoft.com/en-us/cli/azure/query-azure-cli?view=azure-cli-latest)

[JMESPath Documentation](http://jmespath.org/)

Log In:

```bash
az login
```

Try at cmd - use ctrl + d to exit:

```
az interactive
```

> Note: You can also use: `F1 - Open Bash in Cloud Shell` using Azure Account Extension

![open](_images/azure-open.png)

List available extensions:

```bash
az extension list-available --output table
az extension add --name <extension-name>
```

Another Example:

```bash
rnd=$RANDOM
grp=az204-appservice-$rnd
appPlan=appservice-$rnd
web=foodweb-$rnd
loc=westeurope

# create a resource group
az group create -n $grp -l $loc

# create an App Service plan
az appservice plan create -n $appPlan -g $grp --sku B2
```

## Extensions

[Azure Account](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azure-account)

[Azure CLI Tools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli)
