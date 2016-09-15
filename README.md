
# Deploying from a Windows machine
1. Install the Azure CLI tools for Powershell
2. run `azure login`
3. run `Login-AzureRmStorageAccount`

```powershell
cd Scripts
.\Deploy-AzureResourceGroup.ps1 -UploadArtifacts -ResourceGroupLocation westus -ResourceGroupName "irvingchefbackend" -StorageAccountName "chefirvingpremiumstorage" -ArtifactStagingDirectory "..\CustomScripts"  -TemplateFile ..\Templates\ChefServer.json -TemplateParametersFile ..\Templates\ChefServer.parameters.json
```
