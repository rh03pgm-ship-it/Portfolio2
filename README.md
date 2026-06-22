## Azure Lab Environment

```mermaid
graph TD

    A[Azure Subscription]

    A --> B[RG-AVD-LAB]

    B --> C[VNet-AVD<br>10.0.0.0/16]

    C --> D1[default<br>10.0.0.0/24]
    C --> D2[Management<br>10.0.1.0/24]
    C --> D3[AVD<br>10.0.2.0/24]

    B --> E[NSG-AVD]

    E --> E1[Allow HTTP<br>TCP 80]
    E --> E2[Allow HTTPS<br>TCP 443]
    E --> E3[Allow RDP<br>TCP 3389]

    B --> F[Storage Account<br>stlab20260618]

    B --> G[Recovery Services Vault<br>RSV-LAB]

    B --> H[Azure Virtual Desktop]

    H --> I[Host Pool<br>test]

    H --> J[Application Group<br>test-DAG]

    A --> K[Microsoft Entra ID]

    K --> L[RBAC]

    K --> M[Conditional Access<br>Concept Learning]
```

## Learning Objectives

* Azure Networking (VNet / Subnet / NSG)
* Azure Virtual Desktop (AVD)
* Microsoft Entra ID
* RBAC
* Conditional Access
* Azure Storage Account
* Azure Backup (Recovery Services Vault)
* Azure PowerShell (Az Module)
* Terraform (Infrastructure as Code)

## Technologies Used

### Cloud

* Microsoft Azure

### Infrastructure

* Azure Virtual Network (VNet)
* Network Security Group (NSG)
* Azure Virtual Desktop (AVD)
* Storage Account
* Recovery Services Vault

### Identity

* Microsoft Entra ID
* RBAC
* Conditional Access

### Automation / IaC

* Azure PowerShell
* Terraform

## Key Learning Outcomes

* Azureリソースの設計・作成・管理
* VNetおよびSubnet設計
* NSGによる通信制御
* Azure Virtual Desktop構成の理解
* Azure Backup構成の理解
* Azure PowerShellによるリソース管理
* TerraformによるInfrastructure as Code実践
* Microsoft Entra IDによるアクセス制御の理解

```
```

