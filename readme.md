1. datasset create : `az ml data create --file assets/data_assets.yml --resource-group ml-ops --workspace-name ml-ops`
2. create command job:  `az ml job create --file src/job.yml --resource-group mloperations --workspace-name mlops`
3. create SP azure cloudshell:   
                `az ad sp create-for-rbac --name "mlopssp" --role contributor --scopes /subscriptions/1536af98-c2ed-4a44-b30b-6f8119a30f58/resourceGroups/mloperations --sdk-auth`
