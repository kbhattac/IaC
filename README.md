# Infra As Code
Infrastructure as Code deployments
- can be used e.g. through VSTS
- can be used to show incremental ARM deployments e.g. first remove the NSG before kicking of VSTS and then repeat after adding an NSG
- Deploy to Azure using Cloud Shell:

<code>git clone https://github.com/kbhattac/IaC/</code>

<code>az group create --location westeurope --name IaC</code>

<code>az group deployment create --resource-group IaC --template-file ./azuredeploy.json --parameters ./azuredeploy.parameters.json

