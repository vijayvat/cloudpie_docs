To add a cloud account, follow these steps:

1. **Access the Project:**
   - Navigate to the **Dashboard** and select the project where you want to create the cloud account.
   - Once inside the project, locate the **"Add Cloud Account"** menu in the sidebar (this menu is only visible when a project is selected).

2. **Open the Add Cloud Account Form:**
   - Click on the **"Add Cloud Account"** menu to open the form.

3. **Fill Out the Form:**
   - **Select the Cloud Platform:** Choose from the currently supported platforms:
     - **AWS**: Example account IDs: `123456789012`, `987654321098`
     - **GCP**: Example project IDs: `123456789012`, `564738291234`
     - **Azure**: Example subscription IDs: `11111111-2222-3333-4444-555555555555`
   - **Specify the Cloud Account ID:** Enter the account/project/subscription ID corresponding to the platform.

4. **Select Authentication Type:**
   - Choose an authentication type from the list available in dropdown.
   - Provide the required credentials or inputs for the selected authentication type.

   > **Note:** The provided credentials must have the necessary permissions to deploy resources and read cloud data. These will be used for:
   - **Terraform Deployments**
   - **Cloud Query Runs** (using Steampipe/Powerpipe)

5. **Add Variables and Secrets (Optional):**
   - You can add custom variables and secrets that will be injected into the workspace during runs.
   - If a variable is marked as a **secret**, it will be encrypted, securely stored, and decrypted **just in time** during the runs.

6. **Submit the Form:**
   - Review the details and click **Submit** to add the cloud account to the project.

***Example Image: Add Cloud Account***

![Screenshot of Add Cloud Account Form](images/add_cloud_account.png)

---