# Adding a Workspace

Create a workspace for managing Terraform deployments. Define variables and secrets with the highest precedence over project and cloud account levels. Deploy configurations sourced from your linked Git repositories.

## Prerequisites
- An active project in CloudPie
- Cloud account to be associated in workspace is added to project
- Git repository containing Terraform configurations added to Project
- User with permissions to create workspaces

## Creating a Workspace

1. **Access the Project:**
   - Navigate to the **Dashboard**
   - Select your target project
   - Click **Create Workspace** in the sidebar

2. **Configure Workspace Settings:**
   - **Workspace Name** (required)
     Enter a unique identifier for your workspace
   
   - **Description** (optional)
     Add details about the workspace purpose

   - **Terraform Version**
     Specify the version (e.g., 1.5.7)

3. **Link Resources:**
   - **Git Repository**
     Select from available repositories containing Terraform code
   
   - **Cloud Account**
     Choose the target cloud account for deployments

4. **Add Variables (Optional):**
   - Click **Add Variable** to define workspace-specific variables
   - Variables defined here take precedence over project and cloud account variables

5. Click **Create Workspace** to finish setup

![Screenshot of Create Workspace form](images/add_workspace.png)

## Important Notes
- Workspace names must be unique within a project
- Git repository must contain valid Terraform configurations
- Variables are encrypted and securely stored
- State files are managed automatically
- Conflicts are prevented through state locking

---