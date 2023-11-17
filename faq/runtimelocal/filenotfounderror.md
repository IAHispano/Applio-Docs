# FileNotFoundError
This error occurs because you have not added the runtime to the Windows PATH, to do this you have to edit the environment variables and add the path to the Applio-RVC-Fork/runtime/scripts folder at the top of the list.

![](../assets/filenotfounderror.png)

## Follow these steps:
To edit the Windows PATH variable and add the path to the `Applio-RVC-Fork/runtime/scripts` folder at the top of the list, follow these steps:

1. **Access Advanced System Settings:**
- In the Windows search bar enter "Advanced System Settings". The System Properties window will open.

2. **Environment Variables:**
- In the System Properties window, click on the "Environment Variables..." button at the bottom right.

3. **Edit User or System Variables (based on your preference):**
- In the Environment Variables window, you'll see two sections: "User variables" and "System variables."
- If you want to make the change available only to your user account, edit "User variables." If you want to make the change system-wide for all users, edit "System variables." Note that modifying system variables usually requires administrator privileges.

4. **Edit the PATH Variable:**
- In the appropriate section (User or System variables), locate the "Path" variable in the list of variables and select it.
- Click the "Edit..." button to make changes to the selected variable.

5. **Add the Path to the Applio-RVC-Fork Runtime Folder:**
- In the Edit Environment Variable window, click "New" to add a new entry.
- Enter the full path to the `Applio-RVC-Fork/runtime/scripts` folder. Make sure to use semicolons (;) to separate multiple entries if there are any already.
- For example, if the path is `C:\Program Files\Applio-RVC-Fork\runtime\scripts`, you would add this path to the list.

6. **Move the Added Path to the Top:**
- It's important to place the newly added path at the top of the list to ensure that it takes precedence over other conflicting paths.
- Use the "Move Up" button to move the selected path to the top of the list. Repeat this until it's at the top.

7. **Apply Changes and Close:**
- After adding and moving the path, click "OK" on all the open windows to save your changes and close them.

8. **Reopen Command Prompt:**
- To ensure the changes take effect, you may need to reopen the `go-applio.bat` file that were open before making these changes.

![](../assets/path_fix.png)

!!!
The PATH variable will now include the path to the `Applio-RVC-Fork/runtime/scripts` folder at the top, and you should no longer encounter the FileNotFoundError when running Applio!
!!!
