# Adding Git Repositories

Connect your Git repositories to CloudPie projects for managing infrastructure code and policies.

## Prerequisites
- An active project in CloudPie
- User with permissions to add Git repositories
- Valid Git repository URL
- Repository access token (if repository is private)

## Step-by-Step Guide

1. **Access the Project:**
   - Navigate to the **Dashboard**
   - Select your target project
   - Click **Add Git Repository** in the left sidebar menu

2. **Configure Repository Settings:**
   - **Repository URL** (Required)
     Enter the complete HTTPS URL of your Git repository
     Example: `https://github.com/username/repository.git`

   - **Branch Name** (Optional)
     Specify the branch to use
     Default: `main`

3. **Set Configuration Paths:** (All Optional)
   - **Terraform Configuration Path**
     Directory containing Terraform configurations
     Example: `/terraform`

   - **Steampipe Queries Path**
     Location of Steampipe/Powerpipe queries
     Example: `/queries`

   - **Custom Powerpipe Benchmark Path**
     Directory for custom benchmarks
     Example: `/benchmarks`

   - **Policy Governance Path**
     Location of policy files
     Example: `/policies`

4. **Add Authentication:** (Optional)
   - **Repository Token**
     Required only for private repositories
     Example: Personal Access Token with repo access

5. **Submit:**
   - Review all entered information
   - Click **Submit** to add the repository

![Screenshot showing Add Git Repository form](images/add_git_repo.png)

## Important Notes
- Repository name is automatically generated from the URL
- All path configurations are optional
- Invalid paths may cause pipeline failures
- Token is required for private repository access
- Changes take effect immediately after submission

---