# azure-utilities
Utilities requried for retrieving Azure cloud billing, cost as well as scripts for cleaning up resources 

![Azure Cloud CLI](images/Azure-CLI-Azure%20-%20CLI.jpg)

## Caution!

Be aware that *Azure Cloud Nuke* is a very destructive tool, be very careful while using it. Otherwise you might delete production data. **Do NOT run this application on an Azure Cloud account where you cannot afford to lose all resources.**

## Install CLI 

The Azure CLI is available to install in Windows, macOS and Linux environments. It can also be run in a Docker container and Azure Cloud Shell.

Refer the install instructions for Azure CLI - https://docs.microsoft.com/en-us/cli/azure/install-azure-cli

## Azure CLI Sign in interactively
For this release, we are using Azure CLI's default authentication method for logins uses a web browser and access token to sign in.


## CLI options

| BOM ID | Name                                                                       | Description          | Run Time |
|--------|----------------------------------------------------------------------------|----------------------|----------|
| 315    | [315 - Cloud Pak for Data - DB2 Warehouse](./315-cloud-pak-for-data-db2wh) | Deploy DB2 Warehouse | 15 Mins   |
| 320    | [315 - Cloud Pak for Data - DB2 OLTP](./320-cloud-pak-for-data-db2oltp)    | Deploy DB2 OLTP      | 15 Mins   |


## Using the CLI

1. Clone the repo.

   ```bash
   git clone
   ```


2. Run the CLI.

   Perform a dry run:

   ```bash
   ./listaccount.sh
   ```

    ```bash
   ./listresourcegroup.sh
   ```

   Delete all resources within ResourceGroup ():

   ```bash
   ./deleteresourcegroup {ResourceGroup}
   ```
## TODO

1. The project needs support for deleting the following types of resources:
2. The project needs support for deleting with skipping certain resoruces.

## References
- Manage Resource Group : https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-cli
- Manage Resources : https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resources-cli
