# Offboarding A User Account in Active Directory

### Scenario
As we welcome Mr.Johnny Test we must sadly say goodbye to Susan Test (no relation of course 😏), An oustanding employee.Now that she is leaving the company all access she had to file, has to be removed from the network.

### Here's how to do it:

### Prerequisites
- Access to Active Directory Users and Computers
- Administrative credentials
- Knowledge of the user's department location

### Step 1: Opening Active Directory
- Click on Tools in the top right-hand corner
- Click on Active Directory Users and Computers

![Active Directory Tools Menu](Disabling%20User%20Account%20Images/Active-directory-step-1.png)
   
### Step 2: Locating the Right Account
- You can use the search option to find the user account, but if you already know the location, navigate directly
- Important: Verify you have the correct account to avoid affecting another user with the same name
- Navigate to the department where the account was created: ACCOUNTING > Users

### Step 3 : Disabling The Account 
- Right click on the account to be disabled (Susan test)
- Click Disable account 
- Click finish

![Disabling User Account - Right Click Menu](Disabling%20User%20Account%20Images/Disabling-user-account-step3.png)

![Disabling User Account - Process](Disabling%20User%20Account%20Images/Disabling-user-account-step4.png)

![Disabling User Account - Confirmation](Disabling%20User%20Account%20Images/Disabling-user-account-step5.png)

This disables the account NOT delete as it can enabled again.
