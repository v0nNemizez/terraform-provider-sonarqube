# terraform-provider-sonarqube
Terraform provider for managing Sonarqube configuration

## Installation
Download the binary from the [Releases](https://github.com/jdamata/terraform-provider-sonarqube/releases/latest) page and place it in: ```~/.terraform.d/plugins``` or ```%APPDATA%\terraform.d\plugins```

## Usage
[example.tf](example.tf) contains a sample of how to use this provider.

Consult the docs below for more details.

## Docs
[Provider configuration](docs/provider.md)

Resources:
- [sonarqube_group](docs/sonarqube_group.md)
- [sonarqube_permissions](docs/sonarqube_permissions.md)
- [sonarqube_permission_template](docs/sonarqube_permission_template.md)
- [sonarqube_plugin](docs/sonarqube_plugin.md)
- [sonarqube_project](docs/sonarqube_project.md)
- [sonarqube_qualitygate](docs/sonarqube_qualitygate.md)
- [sonarqube_qualitygate_condition](docs/sonarqube_qualitygate_condition.md)
- [sonarqube_qualitygate_project_association](docs/sonarqube_qualitygate_project_association.md)
- [sonarqube_user](docs/sonarqube_user.md)
- [sonarqube_user_token](docs/sonarqube_user_token.md)

TODO:
- quality profiles
- rules
- settings
- users
- webhooks

## Development
```bash
docker run -d -p 9000:9000 sonarqube:latest
make run
```
