# Creating a New User Account in Active Directory

As part of onboarding activities, a new hire or staff member needs a new account to work effectively. This is the task for today.

We will be creating a new user account for a new staff member in the HR department. The HR admin has provided us with the following information:

| Field | Value |
|-------|-------|
| First Name | Johnny |
| Last Name | Test |
| Full Name | Johnny Test |

## Boot up the Server

Once the server is done booting, the `Server Manager` should automatically start up on its own. If not, search for and start it.

Once it is fully loaded, proceed to the next section.

## Creating a User Account

1. Click on `Tools` in the top right-hand corner
2. Click on `Active Directory Users and Computers`
3. Navigate to the department where the user account needs to be added (e.g., `Human Resources/Users`)
4. Right-click on an empty space
5. Hover above `New`
6. Select `User`

Enter the following information provided by HR:

| Field | Value |
|-------|-------|
| First Name | Johnny |
| Initials | (optional) |
| Last Name | Test |
| Full Name | Johnny Test |
| User Logon Name | Johnny.Test |

Click **Next**

### Important Notes

- **User Logon Name**: This is the name the user will see when they log in
- **Naming Convention**: It is important to maintain a consistent naming convention when creating user accounts. Examples:
  - `firstname.lastname@company.com`
  - `lastname.firstname@company.com`
  - `fullname@company.com`

## Creating a Password for the Account

1. Enter a password for the new account
2. Check the box `User Must Change At Next Logon`
   - This ensures that the user changes this temporary password when they log in again
3. Click **Next**
4. Confirm the details
5. Click **Finish**

The account should now be successfully created. The user should log in and change the temporary password.
