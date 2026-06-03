# Creating A New  User Accout in Active Directory

As a part of Onboarding activities , A new hire/Staff needs a new account for them to be able  tow  work effectively, That is the Task for today.
We will be creating a new User account For a New staff in the HR department , HR admin has provided us with the following information

       firstname : Johnny
       lastname  : Test
       Fullname  : Johnny Test

### Step 1 : Boot up the Server
once  the server is done booting, the ```Server Manager``` should automatically startup on its own , if not search and start it.
once it full loaded;
  - click on tools in the top right hand corner
  - click on "Active directory user and  computers"
  - Navigate to Department the user account needs to be added eg Human Resources/Users
  - right click on a empty space 
  - then hover above "New"
  - then select "User"
Enter the following info gotten from HR 
  - firstname : Johnny
  - Intitials(optional)
  - Lastname  : Test
  - fullname  : Johnny Test
  - User Logon name Johnny.Test

***Note***
- the user logon name : This is the name the user will see when they want to login 
- It is also important to Maintain a single naming convention when creating user account the above for constituency 
  For Example
   i.firstname.lastname@comapny.com
   ii.Lastname.firtname@comapny.com
   ii.Fullname@comapny.com

click "Next" 
Then create a password for this new account
check the box "user must change at next logon"
this make sure that the user changes this temp password when they log in again.
click "Next"  
Confirm the Details 
then click finish.
The account should be successfully created.
The user should login and change the temp password.



