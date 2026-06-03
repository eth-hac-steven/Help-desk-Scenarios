# Creating A New  User Accout in Active Directory

As a part of Onboarding activities , A new hire/Staff needs a new account for them to be able  tow  work effectively, That is the Task for today.
We will be creating a new User account For a New staff in the HR department , HR admin has provided us with the following information

       firstname : Johnny
       lastname  : Test
       Fullname  : Johnny Test

### Boot up the Server
once  the server is done booting, the ```Server Manager``` should automatically startup on its own , if not search and start it.
once it full loaded

### Creating A User Account 
  - click on ```tools``` in the top right hand corner
  - click on ```Active directory user and  computers```
  - Navigate to Department the user account needs to be added e.g ```Human Resources/Users```
  - right click on a empty space 
  - then hover above ```New```
  - then select ```User```
Enter the following info gotten from HR 
  - firstname : Johnny
  - Intitials(optional)
  - Lastname  : Test
  - fullname  : Johnny Test
  - User Logon name Johnny.Test

***Note***
- the user logon name : This is the name the user will see when they want to login 
- It is also important to Maintain a single naming convention when creating user account the above for constituency.For Example
  - i.firstname.lastname@comapny.com
  - ii.Lastname.firtname@comapny.com
  - ii.Fullname@comapny.com

click "Next" 

### Creating a Password for the Account

- Enter a password for this new account
- check the box ```User Must Change At Next Logon```
  
This make sure that the user changes this temp password when they log in again.

- Click "Next"  
- Confirm the Details 
- Click finish.
  
The account should be successfully created.
The user should login and change the temp password.



