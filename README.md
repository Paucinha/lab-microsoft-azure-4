# Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure

![GitHub](https://img.shields.io/github/license/Paucinha/api-ecommerce-dio?style=flat-square)

Neste projeto você entenderá na prática os conceitos sobre redes virtuais, balanceamento de carga e muito mais.

**Azure | Full-Stack | Básico**

Resumo do que aprendi durante o lab:

- Tipos de computação, instâncias de contêiner, máquinas virtuais e funções.

- Opções de hospedagem de aplicativos, Aplicativos Web do Azure, contêineres e máquinas virtuais.

- Redes virtuais, sub-redes,  emparelhamento, DNS, do Gateway de VPN e do ExpressRoute.

- [Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure](https://portal.azure.com/#browse/Microsoft.Compute%2FVirtualMachines)

```json
{
    "name": "machine01",
    "id": "/subscriptions/f5f6088e-679a-4fc3-9a5d-600dcca616e6/resourceGroups/AZ-900_Lab_DIO/providers/Microsoft.Compute/virtualMachines/machine01",
    "type": "Microsoft.Compute/virtualMachines",
    "location": "westus2",
    "properties": {
        "hardwareProfile": {
            "vmSize": "Standard_D2s_v3"
        },
        "provisioningState": "Succeeded",
        "vmId": "06be33c9-ef89-4c58-98e4-c0adc6697ded",
        "additionalCapabilities": {
            "hibernationEnabled": false
        },
        "storageProfile": {
            "imageReference": {
                "publisher": "canonical",
                "offer": "ubuntu-24_04-lts",
                "sku": "server",
                "version": "latest",
                "exactVersion": "24.04.202502040"
            },
            "osDisk": {
                "osType": "Linux",
                "name": "machine01_OsDisk_1_aa80787e07244f9f88193a0490b4d5fb",
                "createOption": "FromImage",
                "caching": "ReadWrite",
                "managedDisk": {
                    "storageAccountType": "Premium_LRS",
                    "id": "/subscriptions/f5f6088e-679a-4fc3-9a5d-600dcca616e6/resourceGroups/AZ-900_Lab_DIO/providers/Microsoft.Compute/disks/machine01_OsDisk_1_aa80787e07244f9f88193a0490b4d5fb"
                },
                "deleteOption": "Delete",
                "diskSizeGB": 30
            },
            "dataDisks": []
        },
        "osProfile": {
            "computerName": "machine01",
            "adminUsername": "azureuser",
            "linuxConfiguration": {
                "disablePasswordAuthentication": true,
                "ssh": {
                    "publicKeys": [
                        {
                            "path": "/home/azureuser/.ssh/authorized_keys",
                            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDXoSXcCXhWEajtdtPPXYymt2NXMa7lCoH4S70/3wZ9KlN/SOmagl/9AtbnI1NNSrHBRVmu8Z5HQ6TbivhGqN82KNaICnW6ZiPA85cjo9gjYQBp6qty6CtKBI9/2TQocywWUf248mx7HqU7EppYLAL8Bq2e55KzkF86rHGZZ2aiZyFoFBzE49BhsP+ZTAUuKptwGDLy95ufkGY5jdj783m7QONOuOhY6xufLpsxiHkPwkxtnpqhDv81I6CfN9Yoyw0Zami1pjGpDLMr8A8OQTeKNqlVJHnRUGS+iJ/N6Ktcarc3wPLsV0QOzm5Io8rblkqOTqVXP2sjBABtaKHgv/3Pcq7ylseji4oEHM7YN99UA6pkMh/MSUOXKC0bXPrq3UoXvpbb6Ag9hSssN5Myr14OXwRet8T0ZzgCfwbz282oK7snkEGDonRuoUaM2l9lKr80QUYmosktbaNRxjol71Pdbna57Se6Wv9I8aczC/YzZotuezXZGZPjzPzvFxysY2k= generated-by-azure"
                        }
                    ]
                },
                "provisionVMAgent": true,
                "patchSettings": {
                    "patchMode": "ImageDefault",
                    "assessmentMode": "ImageDefault"
                }
            },
            "secrets": [],
            "allowExtensionOperations": true,
            "requireGuestProvisionSignal": true
        },
        "securityProfile": {
            "uefiSettings": {
                "secureBootEnabled": true,
                "vTpmEnabled": true
            },
            "securityType": "TrustedLaunch"
        },
        "networkProfile": {
            "networkInterfaces": [
                {
                    "id": "/subscriptions/f5f6088e-679a-4fc3-9a5d-600dcca616e6/resourceGroups/AZ-900_Lab_DIO/providers/Microsoft.Network/networkInterfaces/machine01704",
                    "properties": {
                        "deleteOption": "Delete"
                    }
                }
            ]
        }
    },
    "apiVersion": "2021-03-01"
}
```

##

Projeto desenvolvido durante o [**Bootcamp Bradesco - Java Cloud Native**](https://www.dio.me/bootcamp/bradesco-java-cloud-native), fornecido pela [**DIO**](https://www.dio.me/)

##

- [By Páucinha](https://github.com/Paucinha)
