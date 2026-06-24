# Temp User Account issue





### solution
Recommended Approach for AD
- follow this AD-Safe Checklist:

- Check the Server First: Before touching the registry on the client, log in to your File Server and check the user's profile share.

- If the folder exists, rename it to Username.old (or add .bck to the end).
- This forces Windows to treat the server copy as "new" and create a fresh one.
- Fix the Local Registry (The Video Method):

- Rename the local C:\Users\Username folder to Username.old.
- Run the registry fix (rename .bak entries) as shown in the video.
- Crucial: Ensure the State value in the registry is 0 and RefCount is 0.
- Verify Permissions:

- Right-click the new C:\Users\Username folder -> Properties -> Security.
- Ensure the User and SYSTEM have Full Control. If the user is a new AD object, you might need to remove the old SID and add the new one explicitly.
- Test Logon/Logoff:

- Log in as the user.
- Make a small change (e.g., change wallpaper).
- Log off.
- Log back in immediately. If the wallpaper remains, the fix worked. If it resets, the server copy is still corrupt.
