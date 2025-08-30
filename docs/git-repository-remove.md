# Remove Git Repositories linked to project 

Learn how to safely remove Git repositories from your CloudPie project.

## Prerequisites
- User with permissions to delete Git repositories
- Repository must not be in use by active workspaces

## Deletion Process

1. **Access Git Repositories:**
   - Navigate to the **Dashboard**
   - Select your target project
   - Click **View Git Repositories** in the left sidebar menu

2. **Initiate Deletion:**
   - Locate the repository you want to remove
   - Click the delete (trash) icon next to the repository

3. **Confirm Deletion:**
   - A confirmation dialog will appear
   - Type the exact repository name in the confirmation field
   - Check the "I understand this action is irreversible" box
   - Click **Delete** to permanently remove the repository

![Screenshot showing the repository deletion confirmation](Images/delete_git_repository.png)

## Important Notes
- Deletion cannot be undone
- Verify the repository is not used in:
  - Active workspaces
  - Pipeline configurations
  - Policy checks
- Repository deletion does not affect the remote Git repository
- All local configurations and settings will be removed
- Active workspaces using this repository must be deleted first

---