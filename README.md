
# **Project 7: CI Validation for Terraform**

## **Description**

Automated Terraform formatting and validation using GitHub Actions. Configured a CI pipeline to check Terraform code on every push and pull request.

## **Objectives**

- Automate Terraform formatting checks.
- Validate Terraform configuration automatically.
- Integrate GitHub Actions for continuous integration.
- Display workflow status using a GitHub Actions badge.

## **Technologies Used**

- AWS (not required for deployment)
- Terraform
- GitHub Actions
- YAML
- Git and GitHub

## **Project Structure**

```text
project-7-terraform-ci-validation/
│
├── .github/
│   └── workflows/
│       └── terraform-ci.yml
│
├── main.tf
├── README.md
└── .gitignore
```

## **GitHub Actions Workflow**

The CI pipeline performs the following steps:

1. Checks out the GitHub repository.
2. Installs the required Terraform version.
3. Checks Terraform formatting using `terraform fmt -check -recursive`.
4. Initializes Terraform using `terraform init -backend=false`.
5. Validates the configuration using `terraform validate`.

The workflow automatically runs on every push and pull request targeting the `main` branch.

## **Run Locally**

Run the following commands to validate the Terraform configuration locally:

```bash
terraform version
terraform fmt -recursive
terraform init -backend=false
terraform validate
```

## **Expected Result**

The GitHub Actions workflow should complete successfully with all Terraform validation checks passing.

## **GitHub Repository**

[Paste GitHub Repository URL]

## **Screenshots**

### GitHub Actions Pipeline

[Add Pipeline Screenshot Here]

### Workflow Badge

[Add README Badge Screenshot Here]

## **Learning Outcomes**

- Understanding Continuous Integration (CI).
- Automating Terraform validation.
- Working with GitHub Actions workflows.
- Integrating Infrastructure as Code checks into a development workflow.

