# cisco-vpn-auto-login
Apple Script to auto login to your Cisco AnyConnect VPN Client.
Works only on macOS

1. Clone the repository and open the script `wmvpn.scpt` with AppleScript Editor. 
2. Search for `"YOUR_PASSWORD_HERE"` and replace it with your password. 
3. Go to file and export it as an application marking it "Run Only"
4. Give Accessibility permissions to this app from System Preferences > Security > Privacy > Accessibility. Click on add, browse for application and select it.
5. Run the application to automatically login to your VPN.  

**PS:** Do a manual login for the first time after installing the application to set the defaults.   

**Note:** 
* Your password is safe with the application and is not exposed. But in the script, you will have to explicitly remove the password. The script is anyways not needed after the export unless you want to update the password. 
* Make sure you make a successful login through the Cisco AnyConnect manually before using automated script so that the username is set and you know everything needed is working fine.  

**ToDo:**
* Failure handling - to close while loops after certain tries to avoid memory clogging. 
* Handlilng cases when AnyConnect is not installed or is already logged in. 
