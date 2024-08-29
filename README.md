# snowflake_learning

End to End Project with SnowPark - 
<https://www.youtube.com/watch?v=1jC98XQwBZw&list=PLba2xJ7yxHB6W0XT7gxeY1HbJ39FMWoUF&index=1>

Prerequisites
Snowflake Free Trial
Snowpark Python Connector
VS Code

Python version 3.8*
Higher versions of Python are not supported by Snowflake Connectors

Instructions to uninstall and install different Python versions on mac

Run these on Terminal

python_version_number=3.10
sudo rm -rf /Library/Frameworks/Python.framework/Versions/${python_version_number}/
sudo rm -rf "/Applications/Python ${python_version_number}/"
cd /usr/local/bin && ls -l | grep "/Library/Frameworks/Python.framework/Versions/${python_version_number}" | awk '{print $9}' | sudo xargs rm

Download the version you need from <https://www.python.org/downloads/macos/>
Install it manually or can also be installed using homebrew on Terminal

After installing check the output of 
echo $PATH
in terminal.
If it still contains a reference to the older version of Python, then look for ~/.zshrc or ~/.zprofile or .bash_profile in your Users Folder.
Remove the reference to the previous version if you see two versions of Python.

Relaunch terminal and rerun the "echo $PATH" command.
It should have updated to the correct version.

If you still receive errors when you try to run Python command on Terminal, use the alias command -
alias python=/usr/bin/python3
