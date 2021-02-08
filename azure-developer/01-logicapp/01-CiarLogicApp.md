# Criando o Logic app no Azure

## Azure CLI

Logic App não é um subcomando nativo do az cli, para que você consiga interagir é necessário a adição de uma extensão através do seguinte comando.

```bash
az extension add --name logic
```

Para criar um logic app por linha de comando você precisa de um arquivo JSON com a definição do workflow.

Parametros necessários para a criação do Logic App:

* definition: local do arquivo JSON com a definição do workflow do logic app. JSON é gerado pela ferramenta de design 
* location: região do azure (az account list-locations)
* name: o nome do workflow
* resource group: o resource group utilizado para vinculação do recurso

Existem outros para a criação do logic app por linha de comando e isso pode ser consultado através do seguinte comando:

```bash
az logic workflow create --help
```

Um exemplo para a criação do logic app utilizando az cli seria:

```bash
az logic workflow create --resource-group testlogic --location "westus" --name "logicapp2" --definition "example.json"
```

## ARM com PowerShell

Já utilizando Azure Resource Manager é possível criar o logic app através deum arquivo de definição de recurso que no exemplo abaixo utiliza um pré definido.

```Powershell
$projectName = Read-Host -Prompt "Enter a project name to use for generating resource names"
$location = Read-Host -Prompt "Enter the location, such as 'westus'"
$templateUri = "https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/101-logic-app-create/azuredeploy.json"

$resourceGroupName = "${projectName}rg"

New-AzResourceGroup -Name $resourceGroupName -Location "$location"
New-AzResourceGroupDeployment -ResourceGroupName $resourceGroupName -TemplateUri $templateUri

Read-Host -Prompt "Press [ENTER] to continue ..."
```

[02 - Criando um Conector Personalizado ](02-CriarConnectorPersonalizado.md)