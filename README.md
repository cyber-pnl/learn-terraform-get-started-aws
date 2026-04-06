# learn-terraform-get-started-aws

Un repository pour apprendre **Terraform** et déployer une infrastructure sur **AWS**.

##  Description

Ce repository contient des configurations Terraform pour débuter avec l'Infrastructure as Code (IaC) sur Amazon Web Services (AWS). Il permet d'apprendre les concepts fondamentaux de Terraform tout en provisionnant des ressources AWS de manière automatisée.

##  Objectifs

- Apprendre les bases de Terraform
- Comprendre la gestion de l'infrastructure as code
- Déployer des ressources AWS de manière reproductible
- Mettre en pratique les bonnes pratiques DevOps

##  Structure du Projet

```
.
├── main.tf           # Configuration principale des ressources AWS
├── variables.tf      # Déclaration des variables
├── outputs.tf        # Déclaration des outputs
├── terraform.tfvars  # Valeurs des variables (à adapter)
└── README.md         # Ce fichier
```

##  Prérequis

- [Terraform](https://www.terraform.io/downloads.html) (v1.0+)
- [AWS CLI](https://aws.amazon.com/cli/) configurée
- Compte AWS avec les permissions nécessaires
- Clés d'accès AWS configurées en tant que variables d'environnement ou dans `~/.aws/credentials`

## Installation et Utilisation

### 1. Cloner le repository
```bash
git clone https://github.com/cyber-pnl/learn-terraform-get-started-aws.git
cd learn-terraform-get-started-aws
```

### 2. Initialiser Terraform
```bash
terraform init
```

### 3. Vérifier le plan
```bash
terraform plan
```

### 4. Appliquer la configuration
```bash
terraform apply
```

### 5. Détruire les ressources (optionnel)
```bash
terraform destroy
```

##  Configuration

Modifie le fichier `terraform.tfvars` pour adapter les variables selon tes besoins :
```hcl
region = "eu-west-1"
# Ajoute d'autres variables selon ta configuration
```

##  Sécurité

-  **Ne commite jamais** les fichiers contenant des données sensibles (fichiers `.tfstate`, clés d'accès, etc.)
- Utilise un fichier `.gitignore` pour exclure les fichiers sensibles
- Considère l'utilisation de [Terraform Cloud](https://cloud.hashicorp.com/) ou [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/) pour gérer les secrets

##  Ressources Utiles

- [Documentation officielle Terraform](https://www.terraform.io/docs)
- [Documentation AWS Provider pour Terraform](https://registry.terraform.io/providers/hashicorp/aws/latest)
- [Guide AWS pour débuter](https://aws.amazon.com/getting-started/)
- [Terraform Best Practices](https://www.terraform.io/docs/cloud/guides/recommended-practices.html)

##  Contribution

Les contributions sont bienvenues ! N'hésite pas à :
- Signaler des bugs via les [Issues](https://github.com/cyber-pnl/learn-terraform-get-started-aws/issues)
- Proposer des améliorations
- Soumettre des Pull Requests

