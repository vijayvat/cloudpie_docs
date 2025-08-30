# Viewing and Editing Cloud Credentials

View and manage cloud credentials associated with your CloudPie project.

## Prerequisites
- User with roles to Edit Cloud Credentials
- The credential is not in use by active deployments

## Accessing Your Credentials

1. Open the **Dashboard**
2. Select your target project
3. Click **View Credentials** in the left sidebar menu

## Managing Credentials

### Viewing Credentials
You can view all credentials in a sortable list:
- Use the provider filter to sort by cloud provider (AWS, Azure, GCP)
- Use the search bar to find specific credentials by name
- Each credential shows its name, provider type, and authentication method

![Screenshot showing the credentials list view](images/credentials_list_view.png)

### Editing Credentials

1. Locate the credential you want to modify
2. Click the edit (pencil) icon next to the credential
3. In the edit form, you can modify:
   - Authentication type
   - Credential details
   
   > Note: Credential name and cloud provider type cannot be changed after creation

4. Click **Submit** to update the changes

![Screenshot showing the edit credential form](images/edit_credential_form.png)

## Important Notes
- Credentials are encrypted and stored securely
- Changes to credentials take effect immediately
- Editing credentials may temporarily affect running deployments
- Keep your credential details up to date to ensure uninterrupted service

---