# Adding Cloud Credentials

Cloud credentials allow you to securely connect your project with multiple cloud provider accounts (Azure, AWS, GCP). By managing credentials at the project level, you can easily share and reuse authentication across different cloud accounts.

## Prerequisites
- An active project in CloudPie
- Valid credentials for your cloud provider(s)
- User with roles that has permissions to create Cloud Credentials

## Supported Cloud Providers and Authentication Methods

| Provider | Supported Authentication Method(s) |
|----------|---------------------|
| Azure    | Service Principal   |
| AWS      | Certificate Authority, Key Pair |
| GCP      | Service Account JSON |

## Step-by-Step Guide

### 1. Navigate to Credentials Section
1. Open the **Dashboard**
2. Select your target project
3. Find **Add Cloud Credential** in the left sidebar menu

### 2. Configure Cloud Settings
1. Click **Add Cloud Credential**
2. Select your cloud provider (Azure, AWS, or GCP)
3. Choose the appropriate authentication method
4. Enter the required credentials

### 3. Set Permissions
Ensure your credentials include the following permissions:

- **Terraform Deployments**: Administrative-level permissions to:
  - Create, modify, and delete cloud resources
  - Manage resource groups/projects
  - Configure network settings
  - Manage access controls

- **Cloud Queries (Steampipe/Powerpipe)**: Read-level permissions to:
  - List and describe resources
  - Access configuration settings
  - View compliance data
  - Read monitoring metrics

> Note: The exact permission sets vary by cloud provider. Refer to your provider's documentation for detailed permission requirements.

### 4. Complete Setup
1. Review all entered information
2. Click **Submit** to save your credentials
3. Verify the connection status

![Screenshot showing the Add Cloud Credential form](images/add_cloud_credential.png)

## Important Notes
- Credentials are encrypted and stored securely
- One set of credentials can be used across multiple cloud accounts
- You can add multiple credentials to a single project
- Authentication requirements vary by cloud provider

---