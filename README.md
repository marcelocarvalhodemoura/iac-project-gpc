# IAC Project GPC 

## About The Project

This Infrastructure as Code (IaC) project automates the deployment and management of Google Cloud Platform resources using Terraform. The infrastructure is version-controlled, maintainable, and follows security best practices.

## Features

- Automated GCP infrastructure deployment
- Modular and reusable Terraform configurations
- State management with remote backend
- IAM and security policies management
- Network infrastructure setup
- Compute resources provisioning

## Technologies Used

- Terraform v1.x
- Google Cloud Platform (GCP)
- Google Cloud SDK
- Git for version control

## Prerequisites

- Google Cloud Platform Account with billing enabled
- Google Cloud SDK installed and configured
- Terraform installed (version 1.0 or higher)
- Git installed
- GCP Project with required APIs enabled:
  - Compute Engine API
  - Cloud Resource Manager API
  - Identity and Access Management (IAM) API
  - [Add other required APIs]

## Getting Started

1. Clone the repository
```bash
git clone https://github.com/marcelocarvalhodemoura/iac-project-gpc.git
cd iac-project-gpc
```

2. Configure GCP credentials
```bash
gcloud auth application-default login
export GOOGLE_PROJECT="your-project-id"
```

3. Initialize Terraform
```bash
terraform init
```

4. Deploy infrastructure
```bash
terraform plan
terraform apply
```

## Documentation

Detailed documentation about the project structure, modules, and configuration options can be found in the `/docs` directory.

## Project Structure

```
iac-project-gpc/
├── main.tf           # Main Terraform configuration
├── variables.tf      # Input variables
├── outputs.tf        # Output values
├── provider.tf       # Provider configuration
├── modules/          # Reusable Terraform modules
│   ├── networking/   # Network configuration
│   ├── compute/      # Compute resources
│   └── storage/      # Storage resources
└── environments/     # Environment-specific configurations
    ├── dev/
    ├── staging/
    └── prod/
```

## Infrastructure Components

- **Network Infrastructure**
  - VPC Network
  - Subnets
  - Firewall Rules
  - NAT Gateway

- **Compute Resources**
  - Compute Instances
  - Instance Templates
  - Managed Instance Groups
  - Load Balancers

- **Storage**
  - Cloud Storage Buckets
  - Persistent Disks

- **Security**
  - IAM Roles and Permissions
  - Service Accounts
  - Security Policies

## Security

This project implements security best practices including:
- Principle of least privilege for IAM roles
- Network security with proper firewall rules
- Encrypted storage and communication
- Regular security audits and updates

## Best Practices

- Use of Terraform workspaces for environment management
- State file stored in remote backend
- Code modularity and reusability
- Consistent resource naming conventions
- Regular infrastructure updates and maintenance

## Contributing

Contributions are welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Authors

- Marcelo Carvalho - [@marcelocarvalhodemoura](https://github.com/marcelocarvalhodemoura)

## Project Status

Project is actively maintained and in development. Current focus:
- Implementing additional security features
- Optimizing resource configurations
- Adding more automation capabilities

## Contact

- Email: marcelo@devwev.com.br
- GitHub: [marcelocarvalhodemoura](https://github.com/marcelocarvalhodemoura)

Project Link: [https://github.com/marcelocarvalhodemoura/iac-project-gpc](https://github.com/marcelocarvalhodemoura/iac-project-gpc)
