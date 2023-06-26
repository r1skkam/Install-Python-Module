# Install-Python-Module
To add a Python module in Python 3, you typically need to follow these steps:

![image](https://github.com/r1skkam/Install-Python-Module/assets/58542375/0fe92cfb-caf4-4f45-8b94-aa73679db25d)

```
pip3 install requests
```

```
pip3 show requests
```

```
pip3 list |grep requests
```

![image](https://github.com/r1skkam/Install-Python-Module/assets/58542375/0f0ec0ed-4209-4c39-b338-e5bbe8fa8e5c)

When you install a Python module, the module's executable files are typically placed in the system's default binary directory for Python packages. However, if you encounter an issue where the module's executable is not found or not recognized in your environment, you may need to add the module's installation path to the system's PATH variable.

Here's how you can add the installation path of a Python module to the PATH variable:

1. Determine the installation path: After installing the module, you need to identify the directory where the module's executable files are located. You can usually find this information in the output of the pip show <module-name> or pip3 show <module-name> command. Look for the Location field, which indicates the installation directory.
2. Add the installation path to PATH:
- On Windows:

  - Open the Start menu and search for "Environment Variables" or go to Control Panel > System > Advanced system settings > Environment Variables.  
  - In the System Variables section, find the Path variable and click on "Edit".  
  - Add the full path to the module's installation directory at the end of the variable value, separated by a semicolon (;).
  - Click "OK" to save the changes.
  
- On Linux/macOS:
  - Open a terminal window.
  - Edit the shell profile file (~/.bashrc, ~/.bash_profile, or ~/.zshrc, depending on your setup) using a text editor.
  - Add the following line at the end of the file, replacing <module-path> with the actual path to the module's installation directory:
    `export PATH="<module-path>:$PATH"`
  - Save the file and close the text editor.
  - Run source ~/.bashrc (or source ~/.bash_profile or source ~/.zshrc) to apply the changes to the current session.
3. Verify the PATH update: Open a new terminal window and run the module's executable file or import the module in a Python script. If the PATH has been updated correctly, the module should be recognized and accessible.

By adding the module's installation path to the PATH variable, you ensure that the system can locate and execute the module's files when needed.

![image](https://github.com/r1skkam/Install-Python-Module/assets/58542375/3f2cdd91-1f4e-456c-ae43-07d81b7d53c7)

https://github-production-user-asset-6210df.s3.amazonaws.com/58542375/248603669-3f2cdd91-1f4e-456c-ae43-07d81b7d53c7.png

