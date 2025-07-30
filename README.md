# SiyuanOrg GitHub Organization Templates

This repository contains organization-wide workflow templates and configuration for the siyuanorg GitHub organization.

## Repository Structure

```
.github/
├── profile/
│   └── README.md              # Organization profile README
├── workflow-templates/
│   ├── security-paranoia-bot.yml     # Security scanning workflow
│   ├── security-paranoia-bot.properties.json  # Workflow metadata
│   └── security-paranoia-bot.svg     # Workflow icon
└── FUNDING.yml               # Organization-wide funding configuration
```

## Available Workflow Templates

### Security Paranoia Bot

Automatic security vulnerability scanning for pull requests.

**Features:**
- 🔍 Scans code changes for security vulnerabilities
- 💬 Comments directly on PR with findings
- 🎯 Supports multiple languages and frameworks
- ⚡ Fast analysis with GitHub Actions

## Setup Instructions

### For Repository Maintainers

1. Go to your repository's Actions tab
2. Click "New workflow"
3. Search for "Security Paranoia Bot"
4. Click "Configure"
5. Review and commit the workflow file

### For Organization Admins

To update or add new workflow templates:

1. Clone this repository
2. Add/modify files in `.github/workflow-templates/`
3. Include a `.properties.json` file with metadata
4. Optionally add an `.svg` icon (24x24 recommended)
5. Push changes to the main branch

## Workflow Template Guidelines

### Naming Convention
- Use kebab-case for workflow files: `my-workflow.yml`
- Match the properties file name: `my-workflow.properties.json`
- Match the icon file name: `my-workflow.svg`

### Properties File Format
```json
{
  "name": "Workflow Display Name",
  "description": "Brief description of what the workflow does",
  "iconName": "workflow-icon",
  "categories": ["category1", "category2"],
  "filePatterns": ["package.json", "*.js"]
}
```

### Categories
- `automation`: General automation workflows
- `ci`: Continuous Integration
- `code-quality`: Code quality and linting
- `deployment`: Deployment workflows
- `dependency-management`: Dependency updates
- `monitoring`: Monitoring and alerts
- `security`: Security scanning and checks

## Contributing

To contribute new workflow templates:

1. Fork this repository
2. Create a new branch
3. Add your workflow template files
4. Submit a pull request

## Support

For questions or issues with workflow templates, please:
- Open an issue in this repository
- Contact the organization administrators

## License

All workflow templates in this repository are available under the MIT License.