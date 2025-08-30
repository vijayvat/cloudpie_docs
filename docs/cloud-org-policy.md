# Organization Policy Configuration

Configure organization-wide policies to automatically check for violations during Terraform runs.

## Accessing Policy Configuration
1. Open the **Dashboard**
2. Click **Manage Org Policy** in the sidebar menu

## Configuration Settings

## Prerequisites
- An active project in CloudPie
- User with roles that has permissions to Update Org Policy Settings

### Repository Details
- **Repository URL** (Required)  
  URL of the Git repository containing your policy files  
  Example: `https://github.com/organization/policy-repo.git`

- **Branch Name** (Optional)  
  Specific branch to use for policies  
  Default: `main`

- **Policy Path** (Optional)  
  Directory path where .rego files are located  
  Example: `/org_policies`

### Policy Engine Settings
- **Conftest Version** (Optional)  
  Version of Conftest to use for policy evaluation  
  Default: `latest`

- **Repository Token** (Optional)  
  Required only for private repositories  
  Example: Personal Access Token with repo access

![Screenshot of Organization Policy Configuration](images/org_policy_config.png)

## Policy Files
- Policies must be written in Rego language
- Files must have `.rego` extension
- Policies are automatically evaluated during Terraform runs
- For policy language reference, visit [Open Policy Agent Documentation](https://www.openpolicyagent.org/docs/policy-language)

## Important Notes
- Changes to policy configuration take effect immediately
- All subsequent Terraform runs will use updated policies
- Invalid policies may block Terraform operations
- Keep policy files well-documented